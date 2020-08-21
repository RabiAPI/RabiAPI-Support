# RabiAPI User Guide

## Requirements

- JRE Installed
- Write *Javadoc* above your code, not *Comment*

### Javadoc 

```java
/**
 * this is javadoc format
 */
```

### Comment

```java
// this is inline comment

/* this is block comment */
```

## Attention

RabiAPI using static analysis your source code, so **dependency** will not be processed yet.

Class from jar dependency will not appear in RabiAPI.

Manually dependency adding will coming in next few version.

## Supported Frameworks

### Java Interface Support (RPC Service)

- All Java Primitive Types
- Java Container Types, List/Set/Map/Array
- Java Date Types
- Generic & Inheritance Support
- Recursive Support
- Enumeration Support
- Inner Class Support

### Spring Restful Controller Support

- @RestController
- @GetMapping @PostingMapping @PutMapping @DeleteMapping
- @RequestMapping


### Jax-RS Annotation Support


## Add New Project

We support java project build by Gradle or Maven, 

## Add New Branch

RabiAPI support git project and will list all local branches for you, click one to add, after complete, you can switch between different branches.

**You still need to run `git pull` manually, because we promise offline using**

## Refresh Current Branch

Before click refresh button, it's better to run `git pull` to check if has any update, or run `git status` to check if there is any uncommited codes.

RabiAPI will show error message after run `git checkout` failed.

## Delete Project Or Branch

Demo project cannot be deleted.

Click the **dot** menu in project selector or branch selector then click **DELETE** button.

## Handle Project Deleted, Moved Or Renamed

RabiAPI cannot read file path after you do such things, so just delete the current project then re-add it from new path. 


## Multiple Module Support

Module witch has no API will be ignored, click module selector under **Local Repository** to switch between modules.

## Services & Structs Support

//TODO

## Copy JSON Template

Click *Show JSON* button behind the parameters or response subtitle, 
