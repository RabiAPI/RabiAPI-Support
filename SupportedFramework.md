# 已支持的框架和注解

## Spring Boot

### @RestController

使用该注解的class会作为Spring的HTTP接口进行解析。

### @RequestMapping

所有Mapping相关的注解，参数和请求头匹配(params, headers属性)尚未支持。

- @RequestMapping
- @GetMapping
- @PostMapping
- @PutMapping
- @DeleteMapping
- @PatchMapping

### @RequestParam

所有请求参数相关注解，下列是已支持的

- @RequestParam，在GET请求中会作为Query参数，在其它请求中会为作Form参数。
- @RequestBody，作为Body参数，Content-Type一般为application/json
- @RequestPart，作为Form参数，Content-Type为multipart/form-data
- @RequestHeader，作为Header参数
- @PathVariable，作为Path参数
- @CookieValue，作为Cookie参数

### @Validated

和校验注解一起使用，用于分组校验功能。

## JAX-RS

### @Path

## Swagger

Swagger 2.0 旧版注解支持，最新版本为1.6.2。目前鉴权相关的注解暂不支持。

### @Api

存在该注解的class或interface会作为Swagger格式的HTTP接口进行解析。

### @ApiOperation

### @ApiImplicitParams & @ApiImplicitParam

请求参数没有写在方法定义上的时候，可以使用这两个注解标注请求参数，例如通过`HttpServletRequest`直接在方法体内部获取请求参数。

### @ApiResponses & @ApiResponse





