# \PlatformsAPI

All URIs are relative to *https://api.spatio.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AddPlatformProviderAccount**](PlatformsAPI.md#AddPlatformProviderAccount) | **Post** /v1/platforms/{platformId}/providers/{provider}/accounts | Add a connected account for a platform/provider pair.
[**CreateOrUpdatePlatformSecret**](PlatformsAPI.md#CreateOrUpdatePlatformSecret) | **Post** /v1/platforms/{platformId}/secrets | Create or update a secret value.
[**DeletePlatformSecret**](PlatformsAPI.md#DeletePlatformSecret) | **Delete** /v1/platforms/{platformId}/secrets/{name} | Delete a secret.
[**ExecPlatformData**](PlatformsAPI.md#ExecPlatformData) | **Post** /v1/platforms/{platformId}/exec | Run an INSERT/UPDATE/DELETE statement against a platform&#39;s store.
[**ExportPlatformSecrets**](PlatformsAPI.md#ExportPlatformSecrets) | **Get** /v1/platforms/{platformId}/secrets/export | Export all secrets for a platform (values included). Caller must be the platform owner. 
[**GeneratePlatformBackendToken**](PlatformsAPI.md#GeneratePlatformBackendToken) | **Post** /v1/platforms/{platformId}/backend-token | Generate a short-lived backend JWT a platform&#39;s worker can use to call back into platform-service. 
[**GetPlatformCatalog**](PlatformsAPI.md#GetPlatformCatalog) | **Get** /v1/catalog/platforms | List the global platform catalog — every platform that exists, not just the ones the caller has installed. 
[**GetPlatformManifest**](PlatformsAPI.md#GetPlatformManifest) | **Get** /v1/platforms/{platformId}/manifest | Fetch a platform&#39;s manifest (capabilities, schema, UI metadata).
[**ListPlatformAccounts**](PlatformsAPI.md#ListPlatformAccounts) | **Get** /v1/platforms/{platformId}/accounts | List accounts the caller has connected for a platform.
[**ListPlatformProviders**](PlatformsAPI.md#ListPlatformProviders) | **Get** /v1/platforms/{platformId}/providers | Discover supported providers + capabilities for a platform.
[**ListPlatformSecrets**](PlatformsAPI.md#ListPlatformSecrets) | **Get** /v1/platforms/{platformId}/secrets | List secret keys (values redacted).
[**ListPlatformTables**](PlatformsAPI.md#ListPlatformTables) | **Get** /v1/platforms/{platformId}/tables | List tables in a platform&#39;s data store.
[**ListPlatforms**](PlatformsAPI.md#ListPlatforms) | **Get** /v1/platforms | List installed platforms for the sidebar.
[**QueryPlatformData**](PlatformsAPI.md#QueryPlatformData) | **Post** /v1/platforms/{platformId}/query | Run a SELECT query against a platform&#39;s data store.
[**RunPlatformMigrations**](PlatformsAPI.md#RunPlatformMigrations) | **Post** /v1/platforms/{platformId}/migrate | Run pending migrations for a platform.



## AddPlatformProviderAccount

> map[string]interface{} AddPlatformProviderAccount(ctx, platformId, provider).RequestBody(requestBody).Execute()

Add a connected account for a platform/provider pair.

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/spatio-labs/spatio-go"
)

func main() {
	platformId := "platformId_example" // string | 
	provider := "provider_example" // string | 
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PlatformsAPI.AddPlatformProviderAccount(context.Background(), platformId, provider).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PlatformsAPI.AddPlatformProviderAccount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AddPlatformProviderAccount`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `PlatformsAPI.AddPlatformProviderAccount`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**platformId** | **string** |  | 
**provider** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiAddPlatformProviderAccountRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **requestBody** | **map[string]interface{}** |  | 

### Return type

**map[string]interface{}**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateOrUpdatePlatformSecret

> map[string]interface{} CreateOrUpdatePlatformSecret(ctx, platformId).RequestBody(requestBody).Execute()

Create or update a secret value.

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/spatio-labs/spatio-go"
)

func main() {
	platformId := "platformId_example" // string | 
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PlatformsAPI.CreateOrUpdatePlatformSecret(context.Background(), platformId).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PlatformsAPI.CreateOrUpdatePlatformSecret``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateOrUpdatePlatformSecret`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `PlatformsAPI.CreateOrUpdatePlatformSecret`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**platformId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateOrUpdatePlatformSecretRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **requestBody** | **map[string]interface{}** |  | 

### Return type

**map[string]interface{}**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeletePlatformSecret

> DeletePlatformSecret(ctx, platformId, name).Execute()

Delete a secret.

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/spatio-labs/spatio-go"
)

func main() {
	platformId := "platformId_example" // string | 
	name := "name_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.PlatformsAPI.DeletePlatformSecret(context.Background(), platformId, name).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PlatformsAPI.DeletePlatformSecret``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**platformId** | **string** |  | 
**name** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeletePlatformSecretRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

 (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ExecPlatformData

> map[string]interface{} ExecPlatformData(ctx, platformId).RequestBody(requestBody).Execute()

Run an INSERT/UPDATE/DELETE statement against a platform's store.

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/spatio-labs/spatio-go"
)

func main() {
	platformId := "platformId_example" // string | 
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PlatformsAPI.ExecPlatformData(context.Background(), platformId).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PlatformsAPI.ExecPlatformData``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExecPlatformData`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `PlatformsAPI.ExecPlatformData`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**platformId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiExecPlatformDataRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **requestBody** | **map[string]interface{}** |  | 

### Return type

**map[string]interface{}**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ExportPlatformSecrets

> map[string]interface{} ExportPlatformSecrets(ctx, platformId).Execute()

Export all secrets for a platform (values included). Caller must be the platform owner. 

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/spatio-labs/spatio-go"
)

func main() {
	platformId := "platformId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PlatformsAPI.ExportPlatformSecrets(context.Background(), platformId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PlatformsAPI.ExportPlatformSecrets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExportPlatformSecrets`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `PlatformsAPI.ExportPlatformSecrets`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**platformId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiExportPlatformSecretsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**map[string]interface{}**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GeneratePlatformBackendToken

> map[string]interface{} GeneratePlatformBackendToken(ctx, platformId).Execute()

Generate a short-lived backend JWT a platform's worker can use to call back into platform-service. 

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/spatio-labs/spatio-go"
)

func main() {
	platformId := "platformId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PlatformsAPI.GeneratePlatformBackendToken(context.Background(), platformId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PlatformsAPI.GeneratePlatformBackendToken``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GeneratePlatformBackendToken`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `PlatformsAPI.GeneratePlatformBackendToken`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**platformId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGeneratePlatformBackendTokenRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**map[string]interface{}**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetPlatformCatalog

> map[string]interface{} GetPlatformCatalog(ctx).Execute()

List the global platform catalog — every platform that exists, not just the ones the caller has installed. 

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/spatio-labs/spatio-go"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PlatformsAPI.GetPlatformCatalog(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PlatformsAPI.GetPlatformCatalog``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetPlatformCatalog`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `PlatformsAPI.GetPlatformCatalog`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetPlatformCatalogRequest struct via the builder pattern


### Return type

**map[string]interface{}**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetPlatformManifest

> map[string]interface{} GetPlatformManifest(ctx, platformId).Execute()

Fetch a platform's manifest (capabilities, schema, UI metadata).

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/spatio-labs/spatio-go"
)

func main() {
	platformId := "platformId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PlatformsAPI.GetPlatformManifest(context.Background(), platformId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PlatformsAPI.GetPlatformManifest``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetPlatformManifest`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `PlatformsAPI.GetPlatformManifest`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**platformId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetPlatformManifestRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**map[string]interface{}**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListPlatformAccounts

> map[string]interface{} ListPlatformAccounts(ctx, platformId).Execute()

List accounts the caller has connected for a platform.

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/spatio-labs/spatio-go"
)

func main() {
	platformId := "platformId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PlatformsAPI.ListPlatformAccounts(context.Background(), platformId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PlatformsAPI.ListPlatformAccounts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListPlatformAccounts`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `PlatformsAPI.ListPlatformAccounts`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**platformId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListPlatformAccountsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**map[string]interface{}**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListPlatformProviders

> map[string]interface{} ListPlatformProviders(ctx, platformId).Execute()

Discover supported providers + capabilities for a platform.

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/spatio-labs/spatio-go"
)

func main() {
	platformId := "platformId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PlatformsAPI.ListPlatformProviders(context.Background(), platformId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PlatformsAPI.ListPlatformProviders``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListPlatformProviders`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `PlatformsAPI.ListPlatformProviders`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**platformId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListPlatformProvidersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**map[string]interface{}**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListPlatformSecrets

> map[string]interface{} ListPlatformSecrets(ctx, platformId).Execute()

List secret keys (values redacted).

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/spatio-labs/spatio-go"
)

func main() {
	platformId := "platformId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PlatformsAPI.ListPlatformSecrets(context.Background(), platformId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PlatformsAPI.ListPlatformSecrets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListPlatformSecrets`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `PlatformsAPI.ListPlatformSecrets`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**platformId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListPlatformSecretsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**map[string]interface{}**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListPlatformTables

> map[string]interface{} ListPlatformTables(ctx, platformId).Execute()

List tables in a platform's data store.

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/spatio-labs/spatio-go"
)

func main() {
	platformId := "platformId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PlatformsAPI.ListPlatformTables(context.Background(), platformId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PlatformsAPI.ListPlatformTables``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListPlatformTables`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `PlatformsAPI.ListPlatformTables`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**platformId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListPlatformTablesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**map[string]interface{}**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListPlatforms

> map[string]interface{} ListPlatforms(ctx).Execute()

List installed platforms for the sidebar.

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/spatio-labs/spatio-go"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PlatformsAPI.ListPlatforms(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PlatformsAPI.ListPlatforms``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListPlatforms`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `PlatformsAPI.ListPlatforms`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListPlatformsRequest struct via the builder pattern


### Return type

**map[string]interface{}**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## QueryPlatformData

> map[string]interface{} QueryPlatformData(ctx, platformId).RequestBody(requestBody).Execute()

Run a SELECT query against a platform's data store.

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/spatio-labs/spatio-go"
)

func main() {
	platformId := "platformId_example" // string | 
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PlatformsAPI.QueryPlatformData(context.Background(), platformId).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PlatformsAPI.QueryPlatformData``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `QueryPlatformData`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `PlatformsAPI.QueryPlatformData`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**platformId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiQueryPlatformDataRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **requestBody** | **map[string]interface{}** |  | 

### Return type

**map[string]interface{}**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RunPlatformMigrations

> map[string]interface{} RunPlatformMigrations(ctx, platformId).Execute()

Run pending migrations for a platform.

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/spatio-labs/spatio-go"
)

func main() {
	platformId := "platformId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PlatformsAPI.RunPlatformMigrations(context.Background(), platformId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PlatformsAPI.RunPlatformMigrations``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RunPlatformMigrations`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `PlatformsAPI.RunPlatformMigrations`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**platformId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRunPlatformMigrationsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**map[string]interface{}**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

