
### V1.2.0

【接口批量导出和筛选】

1. 右上角新增『导出文档』按钮，支持批量导出所有接口文档
2. 支持导出为Markdown, Asciidoc, Swagger, OpenAPI 四种格式
3. 支持筛选期望导出的模块和服务
4. 支持导出参数约束条件

Swagger、OpenAPI格式仅支持HTTP类型的接口，Java Interface类型暂不支持。

Markdown、Asciidoc格式支持所有类型的接口。

Swagger、OpenAPI格式的导出对于框架类型没有限制，旧版Swagger注解同样可以导出到新版OpenAPI格式，新版OpenAPI注解也可以降级到旧版Swagger格式，这中间可能会做一些兼容性处理，详见Github中的说明。


【新增注解支持】

1. 增加对于Swagger 2.0注解的支持
2. 增加对于OpenAPI 3.0注解的支持

使用了Swagger 2.0旧版注解(如@ApiOperation)或者OpenAPI 3.0新版注解(如@Operation)的项目现在都可以正常生成文档。

支持了大部分如请求信息，参数，响应相关的常用注解，具体支持列表见Github。

允许Swagger注解与其它框架混用，例如同一个项目的部分接口使用Swagger注解标注，其它接口使用Spring和javadoc标注，同样可以正常展示，同样允许批量导出。

RabiAPI到目前为止总共可以为五种写法生成接口文档

1. 直接以Java Interface作为接口的RPC服务，例如Apache Dubbo
2. 使用@RestController注解的Spring MVC服务
3. 使用@Path注解的Jax-RS服务
4. 使用@Api和@ApiOperation注解的旧版Swagger服务
5. 使用@Operation注解的新版OpenAPI服务


【文档解析功能优化】

1. 支持静态变量，静态变量会被替换为实际值，例如 BASE_PATH + "/pet"
2. 支持默认值展示，如果存在默认值，会展示在字段名称右侧
3. 支持展示Content-Type，默认为application/json

【JSR303校验支持优化】

1. JSR303注解校验展示为Json Schema格式, 如maxLength, minLength等
2. 支持部分Hibernate校验注解, @Length/@Range/@Size

### v1.1.6

功能优化

1. 支持通过Mac菜单栏添加项目
2. 修复部分项目生成时的空指针异常问题
3. 修复添加项目发生异常时，弹窗空白的问题
