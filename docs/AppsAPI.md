# \AppsAPI

All URIs are relative to *https://api.spatio.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateApp**](AppsAPI.md#CreateApp) | **Post** /v1/apps | Register a prototype app (project_path is the on-disk root).
[**DeleteApp**](AppsAPI.md#DeleteApp) | **Delete** /v1/apps/{id} | Delete an app.
[**DeleteAppFile**](AppsAPI.md#DeleteAppFile) | **Delete** /v1/apps/{id}/file | Delete one file inside the app&#39;s project directory.
[**GetApp**](AppsAPI.md#GetApp) | **Get** /v1/apps/{id} | Fetch an app.
[**ListAppFiles**](AppsAPI.md#ListAppFiles) | **Get** /v1/apps/{id}/files | List files inside the app&#39;s project directory.
[**ListApps**](AppsAPI.md#ListApps) | **Get** /v1/apps | List the caller&#39;s prototype apps.
[**ReadAppFile**](AppsAPI.md#ReadAppFile) | **Get** /v1/apps/{id}/file | Read one file inside the app&#39;s project directory. Path is traversal-checked; returns 400 if it escapes project root. 
[**UpdateApp**](AppsAPI.md#UpdateApp) | **Patch** /v1/apps/{id} | Update an app.
[**WorkspaceCreateApp**](AppsAPI.md#WorkspaceCreateApp) | **Post** /v1/organizations/{org}/workspaces/{workspace}/apps | 
[**WorkspaceDeleteApp**](AppsAPI.md#WorkspaceDeleteApp) | **Delete** /v1/organizations/{org}/workspaces/{workspace}/apps/{id} | 
[**WorkspaceGetApp**](AppsAPI.md#WorkspaceGetApp) | **Get** /v1/organizations/{org}/workspaces/{workspace}/apps/{id} | 
[**WorkspaceListApps**](AppsAPI.md#WorkspaceListApps) | **Get** /v1/organizations/{org}/workspaces/{workspace}/apps | 
[**WorkspaceUpdateApp**](AppsAPI.md#WorkspaceUpdateApp) | **Patch** /v1/organizations/{org}/workspaces/{workspace}/apps/{id} | 
[**WriteAppFile**](AppsAPI.md#WriteAppFile) | **Post** /v1/apps/{id}/file | Write one file inside the app&#39;s project directory.



## CreateApp

> App CreateApp(ctx).CreateAppRequest(createAppRequest).Execute()

Register a prototype app (project_path is the on-disk root).

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
	createAppRequest := *openapiclient.NewCreateAppRequest("Name_example") // CreateAppRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AppsAPI.CreateApp(context.Background()).CreateAppRequest(createAppRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppsAPI.CreateApp``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateApp`: App
	fmt.Fprintf(os.Stdout, "Response from `AppsAPI.CreateApp`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateAppRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createAppRequest** | [**CreateAppRequest**](CreateAppRequest.md) |  | 

### Return type

[**App**](App.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteApp

> DeleteApp(ctx, id).Execute()

Delete an app.

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
	id := "id_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.AppsAPI.DeleteApp(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppsAPI.DeleteApp``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteAppRequest struct via the builder pattern


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


## DeleteAppFile

> DeleteAppFile(ctx, id).Path(path).Execute()

Delete one file inside the app's project directory.

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
	id := "id_example" // string | 
	path := "path_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.AppsAPI.DeleteAppFile(context.Background(), id).Path(path).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppsAPI.DeleteAppFile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteAppFileRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **path** | **string** |  | 

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


## GetApp

> App GetApp(ctx, id).Execute()

Fetch an app.

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
	id := "id_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AppsAPI.GetApp(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppsAPI.GetApp``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetApp`: App
	fmt.Fprintf(os.Stdout, "Response from `AppsAPI.GetApp`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetAppRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**App**](App.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListAppFiles

> AppFileListResponse ListAppFiles(ctx, id).Path(path).Execute()

List files inside the app's project directory.

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
	id := "id_example" // string | 
	path := "path_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AppsAPI.ListAppFiles(context.Background(), id).Path(path).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppsAPI.ListAppFiles``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListAppFiles`: AppFileListResponse
	fmt.Fprintf(os.Stdout, "Response from `AppsAPI.ListAppFiles`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListAppFilesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **path** | **string** |  | 

### Return type

[**AppFileListResponse**](AppFileListResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListApps

> AppListResponse ListApps(ctx).Execute()

List the caller's prototype apps.

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
	resp, r, err := apiClient.AppsAPI.ListApps(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppsAPI.ListApps``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListApps`: AppListResponse
	fmt.Fprintf(os.Stdout, "Response from `AppsAPI.ListApps`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListAppsRequest struct via the builder pattern


### Return type

[**AppListResponse**](AppListResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ReadAppFile

> AppFileContentResponse ReadAppFile(ctx, id).Path(path).Execute()

Read one file inside the app's project directory. Path is traversal-checked; returns 400 if it escapes project root. 

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
	id := "id_example" // string | 
	path := "path_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AppsAPI.ReadAppFile(context.Background(), id).Path(path).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppsAPI.ReadAppFile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ReadAppFile`: AppFileContentResponse
	fmt.Fprintf(os.Stdout, "Response from `AppsAPI.ReadAppFile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiReadAppFileRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **path** | **string** |  | 

### Return type

[**AppFileContentResponse**](AppFileContentResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateApp

> App UpdateApp(ctx, id).UpdateAppRequest(updateAppRequest).Execute()

Update an app.

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
	id := "id_example" // string | 
	updateAppRequest := *openapiclient.NewUpdateAppRequest() // UpdateAppRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AppsAPI.UpdateApp(context.Background(), id).UpdateAppRequest(updateAppRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppsAPI.UpdateApp``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateApp`: App
	fmt.Fprintf(os.Stdout, "Response from `AppsAPI.UpdateApp`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateAppRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateAppRequest** | [**UpdateAppRequest**](UpdateAppRequest.md) |  | 

### Return type

[**App**](App.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## WorkspaceCreateApp

> map[string]interface{} WorkspaceCreateApp(ctx, org, workspace).RequestBody(requestBody).Execute()



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
	org := "org_example" // string | 
	workspace := "workspace_example" // string | 
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AppsAPI.WorkspaceCreateApp(context.Background(), org, workspace).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppsAPI.WorkspaceCreateApp``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceCreateApp`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `AppsAPI.WorkspaceCreateApp`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceCreateAppRequest struct via the builder pattern


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


## WorkspaceDeleteApp

> WorkspaceDeleteApp(ctx, org, workspace, id).Execute()



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
	org := "org_example" // string | 
	workspace := "workspace_example" // string | 
	id := "id_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.AppsAPI.WorkspaceDeleteApp(context.Background(), org, workspace, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppsAPI.WorkspaceDeleteApp``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceDeleteAppRequest struct via the builder pattern


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


## WorkspaceGetApp

> map[string]interface{} WorkspaceGetApp(ctx, org, workspace, id).Execute()



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
	org := "org_example" // string | 
	workspace := "workspace_example" // string | 
	id := "id_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AppsAPI.WorkspaceGetApp(context.Background(), org, workspace, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppsAPI.WorkspaceGetApp``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceGetApp`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `AppsAPI.WorkspaceGetApp`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceGetAppRequest struct via the builder pattern


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


## WorkspaceListApps

> map[string]interface{} WorkspaceListApps(ctx, org, workspace).Execute()



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
	org := "org_example" // string | 
	workspace := "workspace_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AppsAPI.WorkspaceListApps(context.Background(), org, workspace).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppsAPI.WorkspaceListApps``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceListApps`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `AppsAPI.WorkspaceListApps`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceListAppsRequest struct via the builder pattern


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


## WorkspaceUpdateApp

> map[string]interface{} WorkspaceUpdateApp(ctx, org, workspace, id).RequestBody(requestBody).Execute()



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
	org := "org_example" // string | 
	workspace := "workspace_example" // string | 
	id := "id_example" // string | 
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AppsAPI.WorkspaceUpdateApp(context.Background(), org, workspace, id).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppsAPI.WorkspaceUpdateApp``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceUpdateApp`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `AppsAPI.WorkspaceUpdateApp`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceUpdateAppRequest struct via the builder pattern


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


## WriteAppFile

> WriteAppFile(ctx, id).WriteAppFileRequest(writeAppFileRequest).Execute()

Write one file inside the app's project directory.

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
	id := "id_example" // string | 
	writeAppFileRequest := *openapiclient.NewWriteAppFileRequest("Path_example", "Content_example") // WriteAppFileRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.AppsAPI.WriteAppFile(context.Background(), id).WriteAppFileRequest(writeAppFileRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppsAPI.WriteAppFile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWriteAppFileRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **writeAppFileRequest** | [**WriteAppFileRequest**](WriteAppFileRequest.md) |  | 

### Return type

 (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

