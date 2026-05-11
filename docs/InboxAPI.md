# \InboxAPI

All URIs are relative to *https://api.spatio.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetInboxCounts**](InboxAPI.md#GetInboxCounts) | **Get** /v1/inbox/counts | Per-bucket unread counts.
[**ListInbox**](InboxAPI.md#ListInbox) | **Get** /v1/inbox | Unified inbox feed across mail, channel mentions, DMs, system notifications.
[**MarkInboxItemRead**](InboxAPI.md#MarkInboxItemRead) | **Patch** /v1/inbox/{id}/read | Mark a single inbox item as read.
[**WorkspaceGetInboxCounts**](InboxAPI.md#WorkspaceGetInboxCounts) | **Get** /v1/organizations/{org}/workspaces/{workspace}/inbox/counts | 
[**WorkspaceListInbox**](InboxAPI.md#WorkspaceListInbox) | **Get** /v1/organizations/{org}/workspaces/{workspace}/inbox | 
[**WorkspaceMarkInboxItemRead**](InboxAPI.md#WorkspaceMarkInboxItemRead) | **Patch** /v1/organizations/{org}/workspaces/{workspace}/inbox/{id}/read | 



## GetInboxCounts

> InboxCounts GetInboxCounts(ctx).Execute()

Per-bucket unread counts.

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
	resp, r, err := apiClient.InboxAPI.GetInboxCounts(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InboxAPI.GetInboxCounts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetInboxCounts`: InboxCounts
	fmt.Fprintf(os.Stdout, "Response from `InboxAPI.GetInboxCounts`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetInboxCountsRequest struct via the builder pattern


### Return type

[**InboxCounts**](InboxCounts.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListInbox

> InboxListResponse ListInbox(ctx).Category(category).UnreadOnly(unreadOnly).Limit(limit).Execute()

Unified inbox feed across mail, channel mentions, DMs, system notifications.

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
	category := "category_example" // string |  (optional)
	unreadOnly := true // bool |  (optional)
	limit := int32(56) // int32 |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InboxAPI.ListInbox(context.Background()).Category(category).UnreadOnly(unreadOnly).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InboxAPI.ListInbox``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListInbox`: InboxListResponse
	fmt.Fprintf(os.Stdout, "Response from `InboxAPI.ListInbox`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListInboxRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **category** | **string** |  | 
 **unreadOnly** | **bool** |  | 
 **limit** | **int32** |  | 

### Return type

[**InboxListResponse**](InboxListResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MarkInboxItemRead

> MarkInboxItemRead(ctx, id).Execute()

Mark a single inbox item as read.

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
	r, err := apiClient.InboxAPI.MarkInboxItemRead(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InboxAPI.MarkInboxItemRead``: %v\n", err)
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

Other parameters are passed through a pointer to a apiMarkInboxItemReadRequest struct via the builder pattern


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


## WorkspaceGetInboxCounts

> map[string]interface{} WorkspaceGetInboxCounts(ctx, org, workspace).Execute()



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
	resp, r, err := apiClient.InboxAPI.WorkspaceGetInboxCounts(context.Background(), org, workspace).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InboxAPI.WorkspaceGetInboxCounts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceGetInboxCounts`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `InboxAPI.WorkspaceGetInboxCounts`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceGetInboxCountsRequest struct via the builder pattern


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


## WorkspaceListInbox

> map[string]interface{} WorkspaceListInbox(ctx, org, workspace).Execute()



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
	resp, r, err := apiClient.InboxAPI.WorkspaceListInbox(context.Background(), org, workspace).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InboxAPI.WorkspaceListInbox``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceListInbox`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `InboxAPI.WorkspaceListInbox`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceListInboxRequest struct via the builder pattern


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


## WorkspaceMarkInboxItemRead

> WorkspaceMarkInboxItemRead(ctx, org, workspace, id).Execute()



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
	r, err := apiClient.InboxAPI.WorkspaceMarkInboxItemRead(context.Background(), org, workspace, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InboxAPI.WorkspaceMarkInboxItemRead``: %v\n", err)
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

Other parameters are passed through a pointer to a apiWorkspaceMarkInboxItemReadRequest struct via the builder pattern


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

