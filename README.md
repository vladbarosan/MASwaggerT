# MASwaggerT

> see https://aka.ms/autorest

MA swagger test

### Basic Information
These are the global settings for the test API.

``` yaml
title: Test Foo Bar
description: Test Foo Bar
openapi-type: arm
tag: 2018-08-14-preview

directive:
  - where:
    - $.paths
  - suppress:
    - OperationsAPIImplementation

```

``` yaml
title: Microwaves
description: Microwaves
openapi-type: arm
tag: 2018-09-14-preview

directive:
  - where:
    - $.paths
  - suppress:
    - OperationsAPIImplementation
    
```

### Tag: 2018-08-14-preview

These settings apply only when `--tag=2018-08-14-preview` is specified on the command line.

``` yaml $(tag) == '2018-08-14-preview'
input-file:
- 2018-08-14-preview/mycoolaction.json
```
### Tag: 2018-09-14-preview

These settings apply only when `--tag=2018-09-14-preview` is specified on the command line.

``` yaml $(tag) == '2018-08-14-preview'
input-file:
- 2018-09-14-preview/microwaves.json
```
