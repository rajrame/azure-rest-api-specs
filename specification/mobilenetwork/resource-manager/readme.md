# mobilenetwork

> see https://aka.ms/autorest

This is the AutoRest configuration file for mobilenetwork.

## Getting Started

To build the SDKs for My API, simply install AutoRest via `npm` (`npm install -g autorest`) and then run:

> `autorest readme.md`

To see additional help and options, run:

> `autorest --help`

For other options on installation see [Installing AutoRest](https://aka.ms/autorest/install) on the AutoRest github page.

---

## Configuration

### Basic Information

These are the global settings for the mobilenetwork.

```yaml
openapi-type: arm
openapi-subtype: rpaas
tag: package-2022-01-01-preview
```

### Tag: package-2022-01-01-preview

These settings apply only when `--tag=package-2022-01-01-preview` is specified on the command line.

```yaml $(tag) == 'package-2022-01-01-preview'
input-file:
  - Microsoft.MobileNetwork/preview/2022-01-01-preview/attachedDataNetwork.json
  - Microsoft.MobileNetwork/preview/2022-01-01-preview/common.json
  - Microsoft.MobileNetwork/preview/2022-01-01-preview/dataNetwork.json
  - Microsoft.MobileNetwork/preview/2022-01-01-preview/mobileNetwork.json
  - Microsoft.MobileNetwork/preview/2022-01-01-preview/operation.json
  - Microsoft.MobileNetwork/preview/2022-01-01-preview/packetCoreControlPlane.json
  - Microsoft.MobileNetwork/preview/2022-01-01-preview/packetCoreDataPlane.json
  - Microsoft.MobileNetwork/preview/2022-01-01-preview/service.json
  - Microsoft.MobileNetwork/preview/2022-01-01-preview/simPolicy.json
  - Microsoft.MobileNetwork/preview/2022-01-01-preview/slice.json
  - Microsoft.MobileNetwork/preview/2022-01-01-preview/ts29571.json
```

---

# Code Generation

## Swagger to SDK

This section describes what SDK should be generated by the automatic system.
This is not used by Autorest itself.

```yaml $(swagger-to-sdk)
swagger-to-sdk:
  - repo: azure-sdk-for-python
  - repo: azure-sdk-for-java
  - repo: azure-sdk-for-go
  - repo: azure-sdk-for-js
  - repo: azure-sdk-for-ruby
    after_scripts:
      - bundle install && rake arm:regen_all_profiles['azure_mgmt_mobilenetwork']
```

## Go

See configuration in [readme.go.md](./readme.go.md)

## Python

See configuration in [readme.python.md](./readme.python.md)

## Ruby

See configuration in [readme.ruby.md](./readme.ruby.md)

## TypeScript

See configuration in [readme.typescript.md](./readme.typescript.md)

## CSharp

See configuration in [readme.csharp.md](./readme.csharp.md)