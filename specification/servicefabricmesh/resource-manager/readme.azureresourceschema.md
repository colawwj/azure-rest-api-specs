## AzureResourceSchema

These settings apply only when `--azureresourceschema` is specified on the command line.

### AzureResourceSchema multi-api

``` yaml $(azureresourceschema) && $(multiapi)
# include the azure profile definitions from the standard location
require: ../../../profiles/readme.md

output-folder: $(azureresourceschema-folder)/schemas

# all the input files across all versions
input-file:
  - Microsoft.ServiceFabricMesh/preview/2018-09-01-preview/servicefabricmesh.json
  - Microsoft.ServiceFabricMesh/preview/2018-07-01-preview/servicefabricmesh.json

```