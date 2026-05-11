# \FoldersAPI

All URIs are relative to *https://api.spatio.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateEmailFolder**](FoldersAPI.md#CreateEmailFolder) | **Post** /v1/folders | Create an email folder.
[**DeleteEmailFolder**](FoldersAPI.md#DeleteEmailFolder) | **Delete** /v1/folders/{id} | Delete an email folder.
[**ListEmailFolders**](FoldersAPI.md#ListEmailFolders) | **Get** /v1/folders | List the caller&#39;s email folders.
[**ListFolderEmails**](FoldersAPI.md#ListFolderEmails) | **Get** /v1/folders/{id}/emails | List emails inside a folder.
[**MoveEmailsToFolder**](FoldersAPI.md#MoveEmailsToFolder) | **Post** /v1/folders/{id}/emails | Move emails into a folder.
[**UpdateEmailFolder**](FoldersAPI.md#UpdateEmailFolder) | **Put** /v1/folders/{id} | Update an email folder.



## CreateEmailFolder

> EmailFolder CreateEmailFolder(ctx).CreateEmailFolderRequest(createEmailFolderRequest).Execute()

Create an email folder.

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
	createEmailFolderRequest := *openapiclient.NewCreateEmailFolderRequest("Name_example") // CreateEmailFolderRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FoldersAPI.CreateEmailFolder(context.Background()).CreateEmailFolderRequest(createEmailFolderRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FoldersAPI.CreateEmailFolder``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateEmailFolder`: EmailFolder
	fmt.Fprintf(os.Stdout, "Response from `FoldersAPI.CreateEmailFolder`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateEmailFolderRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createEmailFolderRequest** | [**CreateEmailFolderRequest**](CreateEmailFolderRequest.md) |  | 

### Return type

[**EmailFolder**](EmailFolder.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteEmailFolder

> DeleteEmailFolder(ctx, id).Execute()

Delete an email folder.

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
	r, err := apiClient.FoldersAPI.DeleteEmailFolder(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FoldersAPI.DeleteEmailFolder``: %v\n", err)
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

Other parameters are passed through a pointer to a apiDeleteEmailFolderRequest struct via the builder pattern


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


## ListEmailFolders

> EmailFolderListResponse ListEmailFolders(ctx).Execute()

List the caller's email folders.

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
	resp, r, err := apiClient.FoldersAPI.ListEmailFolders(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FoldersAPI.ListEmailFolders``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListEmailFolders`: EmailFolderListResponse
	fmt.Fprintf(os.Stdout, "Response from `FoldersAPI.ListEmailFolders`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListEmailFoldersRequest struct via the builder pattern


### Return type

[**EmailFolderListResponse**](EmailFolderListResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListFolderEmails

> map[string]interface{} ListFolderEmails(ctx, id).Execute()

List emails inside a folder.

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
	resp, r, err := apiClient.FoldersAPI.ListFolderEmails(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FoldersAPI.ListFolderEmails``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListFolderEmails`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `FoldersAPI.ListFolderEmails`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListFolderEmailsRequest struct via the builder pattern


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


## MoveEmailsToFolder

> map[string]interface{} MoveEmailsToFolder(ctx, id).MoveEmailsRequest(moveEmailsRequest).Execute()

Move emails into a folder.

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
	moveEmailsRequest := *openapiclient.NewMoveEmailsRequest([]string{"MessageIds_example"}) // MoveEmailsRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FoldersAPI.MoveEmailsToFolder(context.Background(), id).MoveEmailsRequest(moveEmailsRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FoldersAPI.MoveEmailsToFolder``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MoveEmailsToFolder`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `FoldersAPI.MoveEmailsToFolder`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiMoveEmailsToFolderRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **moveEmailsRequest** | [**MoveEmailsRequest**](MoveEmailsRequest.md) |  | 

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


## UpdateEmailFolder

> EmailFolder UpdateEmailFolder(ctx, id).UpdateEmailFolderRequest(updateEmailFolderRequest).Execute()

Update an email folder.

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
	updateEmailFolderRequest := *openapiclient.NewUpdateEmailFolderRequest() // UpdateEmailFolderRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FoldersAPI.UpdateEmailFolder(context.Background(), id).UpdateEmailFolderRequest(updateEmailFolderRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FoldersAPI.UpdateEmailFolder``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateEmailFolder`: EmailFolder
	fmt.Fprintf(os.Stdout, "Response from `FoldersAPI.UpdateEmailFolder`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateEmailFolderRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateEmailFolderRequest** | [**UpdateEmailFolderRequest**](UpdateEmailFolderRequest.md) |  | 

### Return type

[**EmailFolder**](EmailFolder.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

