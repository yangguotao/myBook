# mybatis-puls(知识点)
## *Mapper CRUD*接口（说明）
- 通常*crud*封装[BaseMapper](https://gitee.com/baomidou/mybatis-plus/blob/3.0/mybatis-plus-core/src/main/java/com/baomidou/mybatisplus/core/mapper/BaseMapper.java)接口，为*MyBatis-Plus*启动时自动转换实体表关系映射转换为Mybatis内部对象自动注入容器
- 泛型T为任意实体类对象
- 参数*Serializable*为任意型主键*_Mybatis-plus_*不推荐使用复合主键约定每张表都有自己的唯一***id***主键
- 对象*Wrapper*为条件构造器
## _Service CRUD_接口（说明）
- 通用*_Service CRUD_*封装[IService](https://gitee.com/baomidou/mybatis-plus/blob/3.0/mybatis-plus-extension/src/main/java/com/baomidou/mybatisplus/extension/service/IService.java)_接口，进一步封装CRUD采用**_get查询单行、remove删除、list结合查询、page分页_**前缀命名方式区分_Mapper_层避免混淆
- 泛型T为任意实体对象
- 建议如果存在自定义通用*Service*方法的可能，请创建自己的*IBaseService继承Mybatis-Plus*提供的基类
- 对象*Wrapper*为条件构造器
<!-- ``` 
function(){ var sex = 6 yers; }; 
``` -->
## 条件构造器（说明）
>- 以下出现的第一个入参*_Boolean condition_*表示该条件**是否**加入最后生成额*sql*
>- 以下代码块内的多个方法均从上往下补全个别*_Boolean_*类型的入参，默认值为*_true_*
>- 以下出现的泛型_param_均为_Wrapper_的子类实例（均具有_AbstractWrapper_的所有方法）
>- 以下方法在入参中出现的R为泛型,在普通_wrapper_中是_String_,在_LambdaWrapper_中是函数(例:_Entity::getId_,_Entity_为实体类,_getId_为字段***id***的_getMethod_)
>- 以下方法入参中的_R column_均表示数据库字段,当R具体类型为_String_时则为数据库字段名(字段名是数据库关键字的自己用转义符包裹!)!而不是实体类数据字段名!!!,另当R具体类型为_SFunction_时项目_runtime_***不***支持_eclipse_自家的编译器!!!
>- 以下举例均为使用普通_wrapper_,入参为_Map_和_List_的均以_json_形式表现!
>- 使用中如果入参的_Map_或者_List_为空,则不会加入最后生成的_sql_中!!!
### _AbstractWrapper(说明)_
QueryWrapper(LambdaQueryWrapper) 和 UpdateWrapper(LambdaUpdateWrapper) 的父类用于生成 sql 的 where 条件, entity 属性也用于生成 sql 的 where 条件注意: entity 生成的 where 条件与 使用各个 api 生成的 where 条件没有任何关联行为
- allEq(全部eq(或个别isNull))
> 个别参数说明:
> params : key为数据库字段名,value为字段值
> null2IsNull : 为true则在map的value为null时调用 isNull 方法,为false时则忽略value为null的
```
allEq(Map<R, V> params)
allEq(Map<R, V> params, boolean null2IsNull)
allEq(boolean condition, Map<R, V> params, boolean null2IsNull)
```
> 例1: allEq({id:1,name:"老王",age:null})--->id = 1 and name = '老王' and age is null
> 例2: allEq({id:1,name:"老王",age:null}, false)--->id = 1 and name = '老王'
- eq(等于)
> 等于 == 
> 例：eq("name","老王")--->name='老王'
```
eq(R columu,Object val)
eq(boolean condition,R column,Object val)
```
- ne(不等于)
> 不等于<>
> 例：ne("name","Marry")--->name<>'marry'
```
ne(R column,Object val)
ne(boolean condition,R column,Object val)
```
- gt
> 大于>
> 例：gt('age',18)--->age>18
```
gt(R column,Object val)
gt(boolean condition,R column,Object val)
```
- ge  (对于等于)>=
- lt （小于）<
- le （小于等于）<=
- between（在值A到值B间） BETWEEN 值1 AND 值2
> 例: between("age", 18, 30)--->age between 18 and 30
```
between(R column, Object val1, Object val2)
between(boolean condition, R column, Object val1, Object val2)
```
- notBetween (不在值A到值B间）NOT BETWEEN 值1 AND 值2
> 例: notBetween("age", 18, 30)--->age not between 18 and 30
```
notBetween(R column, Object val1, Object val2)
notBetween(boolean condition, R column, Object val1, Object val2)
```
- like (相似) LIKE '%值%'
> 例: like("name", "王")--->name like '%王%'
```
like(R column, Object val)
like(boolean condition, R column, Object val)
```
- notLike(不相似) NOT LIKE '%值%'
> 例: notLike("name", "王")--->name not like '%王%'
``` Java
notLike(R column, Object val)
notLike(boolean condition, R column, Object val)
```
- ·····[csdn案例](https://blog.csdn.net/xie19900123/article/details/81448299)

# 构造器详解
- MyBatis-plus 3.0版本基于JDK1.8，提供Lanbda形式的调用,要求使用jdk1.8以及以上版本。2.0一下可以使用jdk1.8一下版本
## 注解
- TableName 描述：表明注解
- TableId 描述：主键注解
- IdType 描述：主键属性参数 属性：AUTO 描述：数据库自增、INPUT 描述：自行输入、...
- TableFieId描述：字段注解（非主键） 属性 value 描述：字段名 类型：String 必须指定：否 默认值："" 
- ...[点击产看更多](https://mp.baomidou.com/guide/annotation.html#tablename)
## crud接口
### Mapper CRUD 接口
>
> 说明：
> - 通用CRUD封装BaseMapper接口，为Mybatis-Plus启动时自动解析实体表关系映射转换为MyBatis内部对象注入容器
> - 泛型 T 为实体对象
> - 参数 Serializable 为任意类型主键 Mybatis-Plus 不推荐使用复合主键约定没一张表都有自己唯一的 id 主键
> - 对象 Wrapper 为[条件构造器](https://mp.baomidou.com/guide/wrapper.html#abstractwrapper)
> 
- insert 插入一条数据
```
/**
 * return 插入成功记录数
 */
语法：int insert(T entity)
```
- deleteById
```
/**
 * @param id 主键Id
 * @param 删除成功的记录数
 */
int deleteById(Serializable id);
```
- deleteByMap
```

/**
 * 根据 columnMap 条件，删除记录
 * @param columnMap 表字段 map 对象
 * @return 删除成功记录数
 */
int deleteByMap(@param(Constants.COLUMN_MAP) Map<String,Object> columnMap);

```
- deleteBatchIds
```

/**
 * 删除（根据ID 批量删除）
 * @param idList 主键ID列表(不能为 null 以及 empty)
 * @return 删除成功记录数
 */
int deleteBatchIds(@Param(Constants.COLLECTION) Collection<? extends Serializable> idList);

```
- updateById
```

/**
 * <p>
 * 根据 ID 修改
 * </p>
 *
 * @param entity 实体对象
 * @return 修改成功记录数
 */
int updateById(@Param(Constants.ENTITY) T entity);

```
- update
```

/**
 * <p>
 * 根据 whereEntity 条件，更新记录
 * </p>
 *
 * @param entity        实体对象 (set 条件值,可为 null)
 * @param updateWrapper 实体对象封装操作类（可以为 null,里面的 entity 用于生成 where 语句）
 * @return 修改成功记录数
 */
int update(@Param(Constants.ENTITY) T entity, @Param(Constants.WRAPPER) Wrapper<T> updateWrapper);

```
- selectBatchIds
```
/**
 * <p>
 * 查询（根据ID 批量查询）
 * </p>
 *
 * @param idList 主键ID列表(不能为 null 以及 empty)
 * @return 实体集合
 */
List<T> selectBatchIds(@Param(Constants.COLLECTION) Collection<? extends Serializable> idList);

```
- selectByMap
```

/**
 * <p>
 * 查询（根据 columnMap 条件）
 * </p>
 *
 * @param columnMap 表字段 map 对象
 * @return 实体集合
 */
List<T> selectByMap(@Param(Constants.COLUMN_MAP) Map<String, Object> columnMap);

```
- selectPage
```

/**
 * <p>
 * 根据 entity 条件，查询全部记录（并翻页）
 * </p>
 *
 * @param page         分页查询条件（可以为 RowBounds.DEFAULT）
 * @param queryWrapper 实体对象封装操作类（可以为 null）
 * @return 实体分页对象
 */
IPage<T> selectPage(IPage<T> page, @Param(Constants.WRAPPER) Wrapper<T> queryWrapper);

```
- selectMapsPage
```

/**
 * <p>
 * 根据 Wrapper 条件，查询全部记录（并翻页）
 * </p>
 *
 * @param page         分页查询条件
 * @param queryWrapper 实体对象封装操作类
 * @return 字段映射对象 Map 分页对象
 */
IPage<Map<String, Object>> selectMapsPage(IPage<T> page, @Param(Constants.WRAPPER) Wrapper<T> queryWrapper);

```
## [Service CRUD接口](https://mp.baomidou.com/guide/crud-interface.html#service-crud-%E6%8E%A5%E5%8F%A3)
> 
> 说明：
> - 通用 Service CRUD 封装IService接口，进一步封装 CRUD 采用 get 查询单行 remove 删除 list 查询集合 page 分页 前缀命名方式区分 Mapper 层避免混淆，
> - 泛型 T 为任意实体对象
> - 建议如果存在自定义通用 Service 方法的可能，请创建自己的 IBaseService 继承 Mybatis-Plus 提供的基类
> - 对象 Wrapper 为 条件构造器
>
- getOne
```
/**
 * <p>
 * 根据 Wrapper，查询一条记录
 * </p>
 *
 * @param queryWrapper 实体对象封装操作类 {@link com.baomidou.mybatisplus.core.conditions.query.QueryWrapper}
 * @param throwEx      有多个 result 是否抛出异常
 */
T getOne(Wrapper<T> queryWrapper, boolean throwEx);

```
- pageMaps
```
/**
 * <p>
 * 翻页查询
 * </p>
 *
 * @param page         翻页对象
 * @param queryWrapper 实体对象封装操作类 {@link com.baomidou.mybatisplus.core.conditions.query.QueryWrapper}
 */
IPage<Map<String, Object>> pageMaps(IPage<T> page, Wrapper<T> queryWrapper);

```
