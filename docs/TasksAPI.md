# \TasksAPI

All URIs are relative to *https://api.spatio.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**BulkDeleteTasks**](TasksAPI.md#BulkDeleteTasks) | **Post** /v1/tasks/delete | Delete multiple tasks in one call.
[**BulkUpdateTasks**](TasksAPI.md#BulkUpdateTasks) | **Post** /v1/tasks/bulk-update | Apply the same update to multiple tasks.
[**CompleteTask**](TasksAPI.md#CompleteTask) | **Post** /v1/tasks/{id}/complete | Mark a task complete.
[**CreateTask**](TasksAPI.md#CreateTask) | **Post** /v1/tasks | Create a task.
[**CreateTaskComment**](TasksAPI.md#CreateTaskComment) | **Post** /v1/tasks/{id}/comments | Create a comment.
[**DeleteTask**](TasksAPI.md#DeleteTask) | **Delete** /v1/tasks/{id} | Delete a task.
[**DeleteTaskComment**](TasksAPI.md#DeleteTaskComment) | **Delete** /v1/tasks/{id}/comments/{commentId} | Delete a task comment.
[**GetTask**](TasksAPI.md#GetTask) | **Get** /v1/tasks/{id} | Fetch one task.
[**ListTaskComments**](TasksAPI.md#ListTaskComments) | **Get** /v1/tasks/{id}/comments | List comments on a task.
[**ListTaskProviders**](TasksAPI.md#ListTaskProviders) | **Get** /v1/tasks/providers | List supported task providers.
[**ListTasks**](TasksAPI.md#ListTasks) | **Get** /v1/tasks | List tasks across connected accounts.
[**UpdateTask**](TasksAPI.md#UpdateTask) | **Patch** /v1/tasks/{id} | Update a task (partial).
[**UpdateTaskComment**](TasksAPI.md#UpdateTaskComment) | **Patch** /v1/tasks/{id}/comments/{commentId} | Edit a task comment.
[**WorkspaceCompleteTask**](TasksAPI.md#WorkspaceCompleteTask) | **Post** /v1/organizations/{org}/workspaces/{workspace}/tasks/{id}/complete | 
[**WorkspaceCompleteTaskAlias**](TasksAPI.md#WorkspaceCompleteTaskAlias) | **Post** /v1/organizations/{org}/workspaces/{workspace}/tasks/complete/task | Renderer-compat alias for /tasks/{id}/complete.
[**WorkspaceCreateTask**](TasksAPI.md#WorkspaceCreateTask) | **Post** /v1/organizations/{org}/workspaces/{workspace}/tasks | 
[**WorkspaceCreateTaskAlias**](TasksAPI.md#WorkspaceCreateTaskAlias) | **Post** /v1/organizations/{org}/workspaces/{workspace}/tasks/task | Renderer-compat alias for POST /tasks.
[**WorkspaceDeleteTask**](TasksAPI.md#WorkspaceDeleteTask) | **Delete** /v1/organizations/{org}/workspaces/{workspace}/tasks/{id} | 
[**WorkspaceGetTask**](TasksAPI.md#WorkspaceGetTask) | **Get** /v1/organizations/{org}/workspaces/{workspace}/tasks/{id} | 
[**WorkspaceListTaskProviders**](TasksAPI.md#WorkspaceListTaskProviders) | **Get** /v1/organizations/{org}/workspaces/{workspace}/tasks/providers | 
[**WorkspaceListTasks**](TasksAPI.md#WorkspaceListTasks) | **Get** /v1/organizations/{org}/workspaces/{workspace}/tasks | 
[**WorkspaceListTasksAlias**](TasksAPI.md#WorkspaceListTasksAlias) | **Get** /v1/organizations/{org}/workspaces/{workspace}/tasks/tasks | Renderer-compat alias for /tasks.
[**WorkspaceUpdateTask**](TasksAPI.md#WorkspaceUpdateTask) | **Patch** /v1/organizations/{org}/workspaces/{workspace}/tasks/{id} | 
[**WorkspaceUpdateTaskAlias**](TasksAPI.md#WorkspaceUpdateTaskAlias) | **Put** /v1/organizations/{org}/workspaces/{workspace}/tasks/task/{id} | Renderer-compat alias for PATCH /tasks/{id}.



## BulkDeleteTasks

> BulkDeleteTasksResponse BulkDeleteTasks(ctx).BulkDeleteTasksRequest(bulkDeleteTasksRequest).Execute()

Delete multiple tasks in one call.



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
	bulkDeleteTasksRequest := *openapiclient.NewBulkDeleteTasksRequest() // BulkDeleteTasksRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TasksAPI.BulkDeleteTasks(context.Background()).BulkDeleteTasksRequest(bulkDeleteTasksRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TasksAPI.BulkDeleteTasks``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BulkDeleteTasks`: BulkDeleteTasksResponse
	fmt.Fprintf(os.Stdout, "Response from `TasksAPI.BulkDeleteTasks`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBulkDeleteTasksRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **bulkDeleteTasksRequest** | [**BulkDeleteTasksRequest**](BulkDeleteTasksRequest.md) |  | 

### Return type

[**BulkDeleteTasksResponse**](BulkDeleteTasksResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BulkUpdateTasks

> BulkUpdateTasksResponse BulkUpdateTasks(ctx).BulkUpdateTasksRequest(bulkUpdateTasksRequest).Execute()

Apply the same update to multiple tasks.



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
	bulkUpdateTasksRequest := *openapiclient.NewBulkUpdateTasksRequest([]string{"TaskIds_example"}, *openapiclient.NewUpdateTaskRequest()) // BulkUpdateTasksRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TasksAPI.BulkUpdateTasks(context.Background()).BulkUpdateTasksRequest(bulkUpdateTasksRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TasksAPI.BulkUpdateTasks``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BulkUpdateTasks`: BulkUpdateTasksResponse
	fmt.Fprintf(os.Stdout, "Response from `TasksAPI.BulkUpdateTasks`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBulkUpdateTasksRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **bulkUpdateTasksRequest** | [**BulkUpdateTasksRequest**](BulkUpdateTasksRequest.md) |  | 

### Return type

[**BulkUpdateTasksResponse**](BulkUpdateTasksResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CompleteTask

> SuccessFlag CompleteTask(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Mark a task complete.



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
	id := "id_example" // string | Task id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TasksAPI.CompleteTask(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TasksAPI.CompleteTask``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CompleteTask`: SuccessFlag
	fmt.Fprintf(os.Stdout, "Response from `TasksAPI.CompleteTask`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Task id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCompleteTaskRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**SuccessFlag**](SuccessFlag.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateTask

> Task CreateTask(ctx).CreateTaskRequest(createTaskRequest).AccountId(accountId).Provider(provider).XWorkspaceID(xWorkspaceID).Execute()

Create a task.



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
	createTaskRequest := *openapiclient.NewCreateTaskRequest("Title_example") // CreateTaskRequest | 
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	provider := "provider_example" // string | Provider id (e.g. `native-notes`, `notion`). Selects every connected account for the provider. Mutually exclusive with `accountId`.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TasksAPI.CreateTask(context.Background()).CreateTaskRequest(createTaskRequest).AccountId(accountId).Provider(provider).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TasksAPI.CreateTask``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateTask`: Task
	fmt.Fprintf(os.Stdout, "Response from `TasksAPI.CreateTask`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateTaskRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createTaskRequest** | [**CreateTaskRequest**](CreateTaskRequest.md) |  | 
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **provider** | **string** | Provider id (e.g. &#x60;native-notes&#x60;, &#x60;notion&#x60;). Selects every connected account for the provider. Mutually exclusive with &#x60;accountId&#x60;.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**Task**](Task.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateTaskComment

> TaskCommentMutationResponse CreateTaskComment(ctx, id).TaskCommentRequest(taskCommentRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Create a comment.

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
	id := "id_example" // string | Task id.
	taskCommentRequest := *openapiclient.NewTaskCommentRequest("Content_example") // TaskCommentRequest | 
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TasksAPI.CreateTaskComment(context.Background(), id).TaskCommentRequest(taskCommentRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TasksAPI.CreateTaskComment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateTaskComment`: TaskCommentMutationResponse
	fmt.Fprintf(os.Stdout, "Response from `TasksAPI.CreateTaskComment`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Task id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateTaskCommentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **taskCommentRequest** | [**TaskCommentRequest**](TaskCommentRequest.md) |  | 
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**TaskCommentMutationResponse**](TaskCommentMutationResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteTask

> SuccessFlag DeleteTask(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Delete a task.

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
	id := "id_example" // string | Task id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TasksAPI.DeleteTask(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TasksAPI.DeleteTask``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteTask`: SuccessFlag
	fmt.Fprintf(os.Stdout, "Response from `TasksAPI.DeleteTask`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Task id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteTaskRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**SuccessFlag**](SuccessFlag.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteTaskComment

> SuccessFlag DeleteTaskComment(ctx, id, commentId).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Delete a task comment.



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
	id := "id_example" // string | Task id.
	commentId := "commentId_example" // string | Comment id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TasksAPI.DeleteTaskComment(context.Background(), id, commentId).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TasksAPI.DeleteTaskComment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteTaskComment`: SuccessFlag
	fmt.Fprintf(os.Stdout, "Response from `TasksAPI.DeleteTaskComment`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Task id. | 
**commentId** | **string** | Comment id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteTaskCommentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**SuccessFlag**](SuccessFlag.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetTask

> Task GetTask(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Fetch one task.

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
	id := "id_example" // string | Task id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TasksAPI.GetTask(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TasksAPI.GetTask``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetTask`: Task
	fmt.Fprintf(os.Stdout, "Response from `TasksAPI.GetTask`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Task id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetTaskRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**Task**](Task.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListTaskComments

> TaskCommentList ListTaskComments(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

List comments on a task.



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
	id := "id_example" // string | Task id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TasksAPI.ListTaskComments(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TasksAPI.ListTaskComments``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListTaskComments`: TaskCommentList
	fmt.Fprintf(os.Stdout, "Response from `TasksAPI.ListTaskComments`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Task id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListTaskCommentsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**TaskCommentList**](TaskCommentList.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListTaskProviders

> TaskProvidersInfo ListTaskProviders(ctx).Execute()

List supported task providers.



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
	resp, r, err := apiClient.TasksAPI.ListTaskProviders(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TasksAPI.ListTaskProviders``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListTaskProviders`: TaskProvidersInfo
	fmt.Fprintf(os.Stdout, "Response from `TasksAPI.ListTaskProviders`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListTaskProvidersRequest struct via the builder pattern


### Return type

[**TaskProvidersInfo**](TaskProvidersInfo.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListTasks

> TaskListEnvelope ListTasks(ctx).AccountId(accountId).Provider(provider).XWorkspaceID(xWorkspaceID).Completed(completed).Labels(labels).ParentTaskId(parentTaskId).Type_(type_).SourcePlatform(sourcePlatform).SourceId(sourceId).Limit(limit).Offset(offset).Execute()

List tasks across connected accounts.



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
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	provider := "provider_example" // string | Provider id (e.g. `native-notes`, `notion`). Selects every connected account for the provider. Mutually exclusive with `accountId`.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)
	completed := true // bool | Include completed tasks. Default `false` (active tasks only).  (optional) (default to false)
	labels := []string{"Inner_example"} // []string | Repeatable. Filter to tasks carrying every label listed. (optional)
	parentTaskId := "parentTaskId_example" // string | Filter to subtasks of this parent. (optional)
	type_ := "type__example" // string | Discriminator filter (`todo`, `reminder`, `issue`).  (optional)
	sourcePlatform := "sourcePlatform_example" // string | Filter to tasks linked to a given source platform. (optional)
	sourceId := "sourceId_example" // string | Filter to tasks linked to a specific source artifact id. Pair with `sourcePlatform` for an exact match.  (optional)
	limit := int32(56) // int32 |  (optional) (default to 50)
	offset := int32(56) // int32 |  (optional) (default to 0)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TasksAPI.ListTasks(context.Background()).AccountId(accountId).Provider(provider).XWorkspaceID(xWorkspaceID).Completed(completed).Labels(labels).ParentTaskId(parentTaskId).Type_(type_).SourcePlatform(sourcePlatform).SourceId(sourceId).Limit(limit).Offset(offset).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TasksAPI.ListTasks``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListTasks`: TaskListEnvelope
	fmt.Fprintf(os.Stdout, "Response from `TasksAPI.ListTasks`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListTasksRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **provider** | **string** | Provider id (e.g. &#x60;native-notes&#x60;, &#x60;notion&#x60;). Selects every connected account for the provider. Mutually exclusive with &#x60;accountId&#x60;.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 
 **completed** | **bool** | Include completed tasks. Default &#x60;false&#x60; (active tasks only).  | [default to false]
 **labels** | **[]string** | Repeatable. Filter to tasks carrying every label listed. | 
 **parentTaskId** | **string** | Filter to subtasks of this parent. | 
 **type_** | **string** | Discriminator filter (&#x60;todo&#x60;, &#x60;reminder&#x60;, &#x60;issue&#x60;).  | 
 **sourcePlatform** | **string** | Filter to tasks linked to a given source platform. | 
 **sourceId** | **string** | Filter to tasks linked to a specific source artifact id. Pair with &#x60;sourcePlatform&#x60; for an exact match.  | 
 **limit** | **int32** |  | [default to 50]
 **offset** | **int32** |  | [default to 0]

### Return type

[**TaskListEnvelope**](TaskListEnvelope.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateTask

> Task UpdateTask(ctx, id).UpdateTaskRequest(updateTaskRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Update a task (partial).

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
	id := "id_example" // string | Task id.
	updateTaskRequest := *openapiclient.NewUpdateTaskRequest() // UpdateTaskRequest | 
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TasksAPI.UpdateTask(context.Background(), id).UpdateTaskRequest(updateTaskRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TasksAPI.UpdateTask``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateTask`: Task
	fmt.Fprintf(os.Stdout, "Response from `TasksAPI.UpdateTask`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Task id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateTaskRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateTaskRequest** | [**UpdateTaskRequest**](UpdateTaskRequest.md) |  | 
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**Task**](Task.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateTaskComment

> TaskCommentMutationResponse UpdateTaskComment(ctx, id, commentId).TaskCommentRequest(taskCommentRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Edit a task comment.



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
	id := "id_example" // string | Task id.
	commentId := "commentId_example" // string | Comment id.
	taskCommentRequest := *openapiclient.NewTaskCommentRequest("Content_example") // TaskCommentRequest | 
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TasksAPI.UpdateTaskComment(context.Background(), id, commentId).TaskCommentRequest(taskCommentRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TasksAPI.UpdateTaskComment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateTaskComment`: TaskCommentMutationResponse
	fmt.Fprintf(os.Stdout, "Response from `TasksAPI.UpdateTaskComment`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Task id. | 
**commentId** | **string** | Comment id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateTaskCommentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **taskCommentRequest** | [**TaskCommentRequest**](TaskCommentRequest.md) |  | 
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**TaskCommentMutationResponse**](TaskCommentMutationResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## WorkspaceCompleteTask

> map[string]interface{} WorkspaceCompleteTask(ctx, org, workspace, id).Execute()



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
	resp, r, err := apiClient.TasksAPI.WorkspaceCompleteTask(context.Background(), org, workspace, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TasksAPI.WorkspaceCompleteTask``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceCompleteTask`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `TasksAPI.WorkspaceCompleteTask`: %v\n", resp)
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

Other parameters are passed through a pointer to a apiWorkspaceCompleteTaskRequest struct via the builder pattern


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


## WorkspaceCompleteTaskAlias

> map[string]interface{} WorkspaceCompleteTaskAlias(ctx, org, workspace).RequestBody(requestBody).Execute()

Renderer-compat alias for /tasks/{id}/complete.

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
	resp, r, err := apiClient.TasksAPI.WorkspaceCompleteTaskAlias(context.Background(), org, workspace).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TasksAPI.WorkspaceCompleteTaskAlias``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceCompleteTaskAlias`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `TasksAPI.WorkspaceCompleteTaskAlias`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceCompleteTaskAliasRequest struct via the builder pattern


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


## WorkspaceCreateTask

> map[string]interface{} WorkspaceCreateTask(ctx, org, workspace).RequestBody(requestBody).Execute()



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
	resp, r, err := apiClient.TasksAPI.WorkspaceCreateTask(context.Background(), org, workspace).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TasksAPI.WorkspaceCreateTask``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceCreateTask`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `TasksAPI.WorkspaceCreateTask`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceCreateTaskRequest struct via the builder pattern


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


## WorkspaceCreateTaskAlias

> map[string]interface{} WorkspaceCreateTaskAlias(ctx, org, workspace).RequestBody(requestBody).Execute()

Renderer-compat alias for POST /tasks.

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
	resp, r, err := apiClient.TasksAPI.WorkspaceCreateTaskAlias(context.Background(), org, workspace).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TasksAPI.WorkspaceCreateTaskAlias``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceCreateTaskAlias`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `TasksAPI.WorkspaceCreateTaskAlias`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceCreateTaskAliasRequest struct via the builder pattern


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


## WorkspaceDeleteTask

> WorkspaceDeleteTask(ctx, org, workspace, id).Execute()



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
	r, err := apiClient.TasksAPI.WorkspaceDeleteTask(context.Background(), org, workspace, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TasksAPI.WorkspaceDeleteTask``: %v\n", err)
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

Other parameters are passed through a pointer to a apiWorkspaceDeleteTaskRequest struct via the builder pattern


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


## WorkspaceGetTask

> map[string]interface{} WorkspaceGetTask(ctx, org, workspace, id).Execute()



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
	resp, r, err := apiClient.TasksAPI.WorkspaceGetTask(context.Background(), org, workspace, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TasksAPI.WorkspaceGetTask``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceGetTask`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `TasksAPI.WorkspaceGetTask`: %v\n", resp)
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

Other parameters are passed through a pointer to a apiWorkspaceGetTaskRequest struct via the builder pattern


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


## WorkspaceListTaskProviders

> map[string]interface{} WorkspaceListTaskProviders(ctx, org, workspace).Execute()



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
	resp, r, err := apiClient.TasksAPI.WorkspaceListTaskProviders(context.Background(), org, workspace).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TasksAPI.WorkspaceListTaskProviders``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceListTaskProviders`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `TasksAPI.WorkspaceListTaskProviders`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceListTaskProvidersRequest struct via the builder pattern


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


## WorkspaceListTasks

> map[string]interface{} WorkspaceListTasks(ctx, org, workspace).Execute()



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
	resp, r, err := apiClient.TasksAPI.WorkspaceListTasks(context.Background(), org, workspace).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TasksAPI.WorkspaceListTasks``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceListTasks`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `TasksAPI.WorkspaceListTasks`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceListTasksRequest struct via the builder pattern


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


## WorkspaceListTasksAlias

> map[string]interface{} WorkspaceListTasksAlias(ctx, org, workspace).Execute()

Renderer-compat alias for /tasks.

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
	resp, r, err := apiClient.TasksAPI.WorkspaceListTasksAlias(context.Background(), org, workspace).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TasksAPI.WorkspaceListTasksAlias``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceListTasksAlias`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `TasksAPI.WorkspaceListTasksAlias`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceListTasksAliasRequest struct via the builder pattern


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


## WorkspaceUpdateTask

> map[string]interface{} WorkspaceUpdateTask(ctx, org, workspace, id).RequestBody(requestBody).Execute()



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
	resp, r, err := apiClient.TasksAPI.WorkspaceUpdateTask(context.Background(), org, workspace, id).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TasksAPI.WorkspaceUpdateTask``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceUpdateTask`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `TasksAPI.WorkspaceUpdateTask`: %v\n", resp)
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

Other parameters are passed through a pointer to a apiWorkspaceUpdateTaskRequest struct via the builder pattern


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


## WorkspaceUpdateTaskAlias

> map[string]interface{} WorkspaceUpdateTaskAlias(ctx, org, workspace, id).RequestBody(requestBody).Execute()

Renderer-compat alias for PATCH /tasks/{id}.

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
	resp, r, err := apiClient.TasksAPI.WorkspaceUpdateTaskAlias(context.Background(), org, workspace, id).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TasksAPI.WorkspaceUpdateTaskAlias``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceUpdateTaskAlias`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `TasksAPI.WorkspaceUpdateTaskAlias`: %v\n", resp)
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

Other parameters are passed through a pointer to a apiWorkspaceUpdateTaskAliasRequest struct via the builder pattern


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

