# Update Admin
    
> see https://aka.ms/autorest

This is the AutoRest configuration file for Update Admin.

---
## Getting Started 
To build the SDK for Update Admin, simply [Install AutoRest](https://aka.ms/autorest/install) and in this folder, run:

> `autorest`

To see additional help and options, run:

> `autorest --help`
---

## Configuration

### Basic Information 
These are the global settings for the Update API.

``` yaml
title: UpdateAdminClient
description: Update Admin Client
openapi-type: arm
tag: package-2016-05-01
```

### Tag: package-2016-05-01

These settings apply only when `--tag=package-2016-05-01` is specified on the command line.

``` yaml $(tag) == 'package-2016-05-01'
input-file:
    - "Microsoft.Update.Admin/2016-05-01/Update.json"
    - "Microsoft.Update.Admin/2016-05-01/Updates.json"
    - "Microsoft.Update.Admin/2016-05-01/UpdateLocations.json"
    - "Microsoft.Update.Admin/2016-05-01/UpdateRuns.json"
```

---
# Code Generation

## C# 

These settings apply only when `--csharp` is specified on the command line.
Please also specify `--csharp-sdks-folder=<path to "SDKs" directory of your azure-sdk-for-net clone>`.

``` yaml $(csharp)
csharp:
  azure-arm: true
  license-header: MICROSOFT_MIT_NO_VERSION
  namespace: Microsoft.AzureStack.Management.Update.Admin
  payload-flattening-threshold: 1
  output-folder: $(csharp-sdks-folder)/Update/Update.Admin/Generated
  clear-output-folder: true
```

## Python

These settings apply only when `--python` is specified on the command line.

``` yaml $(python)
python:
  # override the default output folder
  output-folder: $(output-folder)/python
  license-header: MICROSOFT_MIT_NO_VERSION
  payload-flattening-threshold: 2
```

### Tag: package-2016-05-01 and python

These settings apply only when `--tag=package-2016-05-01 --python` is specified on the command line.

``` yaml $(tag) == 'package-2016-05-01' && $(python)
namespace: azure.mgmt.update.admin.v2016_05_01
```
