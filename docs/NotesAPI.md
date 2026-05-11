# \NotesAPI

All URIs are relative to *https://api.spatio.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateBlock**](NotesAPI.md#CreateBlock) | **Post** /v1/notes/{id}/blocks | Insert a block in a note.
[**CreateNote**](NotesAPI.md#CreateNote) | **Post** /v1/notes | Create a note.
[**CreateNoteComment**](NotesAPI.md#CreateNoteComment) | **Post** /v1/notes/{id}/comments | Create a comment or reply.
[**DeleteBlock**](NotesAPI.md#DeleteBlock) | **Delete** /v1/notes/blocks/{id} | Delete a block.
[**DeleteNote**](NotesAPI.md#DeleteNote) | **Delete** /v1/notes/{id} | Delete a note.
[**DeleteNoteComment**](NotesAPI.md#DeleteNoteComment) | **Delete** /v1/notes/{id}/comments/{commentId} | Soft-delete (native) or hard-delete (provider) a comment.
[**DisableNoteShare**](NotesAPI.md#DisableNoteShare) | **Delete** /v1/notes/{id}/share | Disable public sharing.
[**EnableNoteShare**](NotesAPI.md#EnableNoteShare) | **Post** /v1/notes/{id}/share | Enable (or update password on) public sharing.
[**GetBlock**](NotesAPI.md#GetBlock) | **Get** /v1/notes/blocks/{id} | Fetch one block.
[**GetNote**](NotesAPI.md#GetNote) | **Get** /v1/notes/{id} | Fetch one note.
[**GetNoteComment**](NotesAPI.md#GetNoteComment) | **Get** /v1/notes/{id}/comments/{commentId} | Fetch one comment.
[**GetNoteShareSettings**](NotesAPI.md#GetNoteShareSettings) | **Get** /v1/notes/{id}/share | Fetch share settings for a note.
[**GetPublicNote**](NotesAPI.md#GetPublicNote) | **Get** /public/notes/{token} | Fetch a publicly shared note.
[**ListBlocks**](NotesAPI.md#ListBlocks) | **Get** /v1/notes/{id}/blocks | List blocks under a note.
[**ListNoteComments**](NotesAPI.md#ListNoteComments) | **Get** /v1/notes/{id}/comments | List comments on a note.
[**ListNotes**](NotesAPI.md#ListNotes) | **Get** /v1/notes | List notes across connected accounts.
[**MoveBlock**](NotesAPI.md#MoveBlock) | **Post** /v1/notes/blocks/{id}/move | Reparent or reorder a block.
[**RotateNoteShareToken**](NotesAPI.md#RotateNoteShareToken) | **Post** /v1/notes/{id}/share/rotate | Rotate the share token, invalidating any outstanding URLs.
[**UpdateBlock**](NotesAPI.md#UpdateBlock) | **Patch** /v1/notes/blocks/{id} | Update a block (partial).
[**UpdateNote**](NotesAPI.md#UpdateNote) | **Patch** /v1/notes/{id} | Update a note (partial).
[**UpdateNoteComment**](NotesAPI.md#UpdateNoteComment) | **Patch** /v1/notes/{id}/comments/{commentId} | Edit a comment.
[**WorkspaceCreateNote**](NotesAPI.md#WorkspaceCreateNote) | **Post** /v1/organizations/{org}/workspaces/{workspace}/notes | 
[**WorkspaceCreateNoteBlock**](NotesAPI.md#WorkspaceCreateNoteBlock) | **Post** /v1/organizations/{org}/workspaces/{workspace}/notes/{id}/blocks | 
[**WorkspaceDeleteNote**](NotesAPI.md#WorkspaceDeleteNote) | **Delete** /v1/organizations/{org}/workspaces/{workspace}/notes/{id} | 
[**WorkspaceDeleteNoteBlock**](NotesAPI.md#WorkspaceDeleteNoteBlock) | **Delete** /v1/organizations/{org}/workspaces/{workspace}/notes/blocks/{id} | 
[**WorkspaceGetNote**](NotesAPI.md#WorkspaceGetNote) | **Get** /v1/organizations/{org}/workspaces/{workspace}/notes/{id} | 
[**WorkspaceGetNoteBlock**](NotesAPI.md#WorkspaceGetNoteBlock) | **Get** /v1/organizations/{org}/workspaces/{workspace}/notes/blocks/{id} | 
[**WorkspaceListNoteBlocks**](NotesAPI.md#WorkspaceListNoteBlocks) | **Get** /v1/organizations/{org}/workspaces/{workspace}/notes/{id}/blocks | 
[**WorkspaceListNotes**](NotesAPI.md#WorkspaceListNotes) | **Get** /v1/organizations/{org}/workspaces/{workspace}/notes | 
[**WorkspaceMoveNoteBlock**](NotesAPI.md#WorkspaceMoveNoteBlock) | **Post** /v1/organizations/{org}/workspaces/{workspace}/notes/blocks/{id}/move | 
[**WorkspaceUpdateNote**](NotesAPI.md#WorkspaceUpdateNote) | **Patch** /v1/organizations/{org}/workspaces/{workspace}/notes/{id} | 
[**WorkspaceUpdateNoteBlock**](NotesAPI.md#WorkspaceUpdateNoteBlock) | **Patch** /v1/organizations/{org}/workspaces/{workspace}/notes/blocks/{id} | 



## CreateBlock

> Block CreateBlock(ctx, id).CreateBlockRequest(createBlockRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Insert a block in a note.

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
	id := "id_example" // string | Note id.
	createBlockRequest := *openapiclient.NewCreateBlockRequest(openapiclient.BlockType("paragraph"), *openapiclient.NewBlockContent(), int32(123)) // CreateBlockRequest | 
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NotesAPI.CreateBlock(context.Background(), id).CreateBlockRequest(createBlockRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.CreateBlock``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateBlock`: Block
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.CreateBlock`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Note id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateBlockRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createBlockRequest** | [**CreateBlockRequest**](CreateBlockRequest.md) |  | 
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**Block**](Block.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateNote

> Note CreateNote(ctx).CreateNoteRequest(createNoteRequest).AccountId(accountId).Provider(provider).XWorkspaceID(xWorkspaceID).Execute()

Create a note.



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
	createNoteRequest := *openapiclient.NewCreateNoteRequest("Title_example") // CreateNoteRequest | 
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	provider := "provider_example" // string | Provider id (e.g. `native-notes`, `notion`). Selects every connected account for the provider. Mutually exclusive with `accountId`.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NotesAPI.CreateNote(context.Background()).CreateNoteRequest(createNoteRequest).AccountId(accountId).Provider(provider).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.CreateNote``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateNote`: Note
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.CreateNote`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateNoteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createNoteRequest** | [**CreateNoteRequest**](CreateNoteRequest.md) |  | 
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **provider** | **string** | Provider id (e.g. &#x60;native-notes&#x60;, &#x60;notion&#x60;). Selects every connected account for the provider. Mutually exclusive with &#x60;accountId&#x60;.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**Note**](Note.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateNoteComment

> CommentMutationResponse CreateNoteComment(ctx, id).CreateCommentRequest(createCommentRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Create a comment or reply.

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
	id := "id_example" // string | Note id.
	createCommentRequest := *openapiclient.NewCreateCommentRequest() // CreateCommentRequest | 
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NotesAPI.CreateNoteComment(context.Background(), id).CreateCommentRequest(createCommentRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.CreateNoteComment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateNoteComment`: CommentMutationResponse
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.CreateNoteComment`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Note id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateNoteCommentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createCommentRequest** | [**CreateCommentRequest**](CreateCommentRequest.md) |  | 
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**CommentMutationResponse**](CommentMutationResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteBlock

> SuccessFlag DeleteBlock(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Delete a block.

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
	id := "id_example" // string | Block id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NotesAPI.DeleteBlock(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.DeleteBlock``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteBlock`: SuccessFlag
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.DeleteBlock`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Block id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteBlockRequest struct via the builder pattern


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


## DeleteNote

> SuccessFlag DeleteNote(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Delete a note.

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
	id := "id_example" // string | Note id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NotesAPI.DeleteNote(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.DeleteNote``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteNote`: SuccessFlag
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.DeleteNote`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Note id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteNoteRequest struct via the builder pattern


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


## DeleteNoteComment

> SuccessFlag DeleteNoteComment(ctx, id, commentId).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Soft-delete (native) or hard-delete (provider) a comment.



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
	id := "id_example" // string | Note id.
	commentId := "commentId_example" // string | Comment id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NotesAPI.DeleteNoteComment(context.Background(), id, commentId).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.DeleteNoteComment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteNoteComment`: SuccessFlag
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.DeleteNoteComment`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Note id. | 
**commentId** | **string** | Comment id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteNoteCommentRequest struct via the builder pattern


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


## DisableNoteShare

> DisableNoteShare(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Disable public sharing.



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
	id := "id_example" // string | Note id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.NotesAPI.DisableNoteShare(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.DisableNoteShare``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Note id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDisableNoteShareRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

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


## EnableNoteShare

> ShareSettings EnableNoteShare(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).EnableShareRequest(enableShareRequest).Execute()

Enable (or update password on) public sharing.



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
	id := "id_example" // string | Note id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)
	enableShareRequest := *openapiclient.NewEnableShareRequest() // EnableShareRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NotesAPI.EnableNoteShare(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).EnableShareRequest(enableShareRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.EnableNoteShare``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `EnableNoteShare`: ShareSettings
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.EnableNoteShare`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Note id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiEnableNoteShareRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 
 **enableShareRequest** | [**EnableShareRequest**](EnableShareRequest.md) |  | 

### Return type

[**ShareSettings**](ShareSettings.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetBlock

> Block GetBlock(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Fetch one block.

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
	id := "id_example" // string | Block id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NotesAPI.GetBlock(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.GetBlock``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetBlock`: Block
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.GetBlock`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Block id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetBlockRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**Block**](Block.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetNote

> Note GetNote(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Fetch one note.

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
	id := "id_example" // string | Note id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NotesAPI.GetNote(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.GetNote``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetNote`: Note
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.GetNote`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Note id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetNoteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**Note**](Note.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetNoteComment

> CommentResponse GetNoteComment(ctx, id, commentId).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Fetch one comment.



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
	id := "id_example" // string | Note id.
	commentId := "commentId_example" // string | Comment id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NotesAPI.GetNoteComment(context.Background(), id, commentId).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.GetNoteComment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetNoteComment`: CommentResponse
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.GetNoteComment`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Note id. | 
**commentId** | **string** | Comment id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetNoteCommentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**CommentResponse**](CommentResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetNoteShareSettings

> ShareSettings GetNoteShareSettings(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Fetch share settings for a note.



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
	id := "id_example" // string | Note id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NotesAPI.GetNoteShareSettings(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.GetNoteShareSettings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetNoteShareSettings`: ShareSettings
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.GetNoteShareSettings`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Note id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetNoteShareSettingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**ShareSettings**](ShareSettings.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetPublicNote

> map[string]interface{} GetPublicNote(ctx, token).Password(password).Execute()

Fetch a publicly shared note.



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
	token := "token_example" // string | Opaque public-share token.
	password := "password_example" // string | Optional viewer password. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NotesAPI.GetPublicNote(context.Background(), token).Password(password).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.GetPublicNote``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetPublicNote`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.GetPublicNote`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**token** | **string** | Opaque public-share token. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetPublicNoteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **password** | **string** | Optional viewer password. | 

### Return type

**map[string]interface{}**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListBlocks

> BlockListResponse ListBlocks(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).ParentId(parentId).Limit(limit).Offset(offset).Execute()

List blocks under a note.



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
	id := "id_example" // string | Note id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)
	parentId := "parentId_example" // string | Filter to children of this block id. Omit to list root-level blocks.  (optional)
	limit := int32(56) // int32 |  (optional) (default to 100)
	offset := int32(56) // int32 |  (optional) (default to 0)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NotesAPI.ListBlocks(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).ParentId(parentId).Limit(limit).Offset(offset).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.ListBlocks``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListBlocks`: BlockListResponse
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.ListBlocks`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Note id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListBlocksRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 
 **parentId** | **string** | Filter to children of this block id. Omit to list root-level blocks.  | 
 **limit** | **int32** |  | [default to 100]
 **offset** | **int32** |  | [default to 0]

### Return type

[**BlockListResponse**](BlockListResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListNoteComments

> CommentListResponse ListNoteComments(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

List comments on a note.



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
	id := "id_example" // string | Note id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NotesAPI.ListNoteComments(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.ListNoteComments``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListNoteComments`: CommentListResponse
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.ListNoteComments`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Note id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListNoteCommentsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**CommentListResponse**](CommentListResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListNotes

> NoteListEnvelope ListNotes(ctx).AccountId(accountId).Provider(provider).XWorkspaceID(xWorkspaceID).Archived(archived).ParentId(parentId).Tags(tags).Limit(limit).Offset(offset).SortBy(sortBy).SortOrder(sortOrder).Execute()

List notes across connected accounts.



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
	archived := true // bool | When `true`, return archived notes instead of active ones. (optional) (default to false)
	parentId := "parentId_example" // string | Filter to notes nested under this parent note id. (optional)
	tags := []string{"Inner_example"} // []string | Repeatable. Filter to notes carrying every tag listed. (optional)
	limit := int32(56) // int32 | Max items to return. Defaults to 50. (optional) (default to 50)
	offset := int32(56) // int32 | Number of items to skip. (optional) (default to 0)
	sortBy := "sortBy_example" // string | Sort field. Provider-dependent; the native provider supports `updated_at`, `created_at`, `title`.  (optional) (default to "updated_at")
	sortOrder := "sortOrder_example" // string |  (optional) (default to "desc")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NotesAPI.ListNotes(context.Background()).AccountId(accountId).Provider(provider).XWorkspaceID(xWorkspaceID).Archived(archived).ParentId(parentId).Tags(tags).Limit(limit).Offset(offset).SortBy(sortBy).SortOrder(sortOrder).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.ListNotes``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListNotes`: NoteListEnvelope
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.ListNotes`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListNotesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **provider** | **string** | Provider id (e.g. &#x60;native-notes&#x60;, &#x60;notion&#x60;). Selects every connected account for the provider. Mutually exclusive with &#x60;accountId&#x60;.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 
 **archived** | **bool** | When &#x60;true&#x60;, return archived notes instead of active ones. | [default to false]
 **parentId** | **string** | Filter to notes nested under this parent note id. | 
 **tags** | **[]string** | Repeatable. Filter to notes carrying every tag listed. | 
 **limit** | **int32** | Max items to return. Defaults to 50. | [default to 50]
 **offset** | **int32** | Number of items to skip. | [default to 0]
 **sortBy** | **string** | Sort field. Provider-dependent; the native provider supports &#x60;updated_at&#x60;, &#x60;created_at&#x60;, &#x60;title&#x60;.  | [default to &quot;updated_at&quot;]
 **sortOrder** | **string** |  | [default to &quot;desc&quot;]

### Return type

[**NoteListEnvelope**](NoteListEnvelope.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MoveBlock

> SuccessFlag MoveBlock(ctx, id).MoveBlockRequest(moveBlockRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Reparent or reorder a block.

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
	id := "id_example" // string | Block id.
	moveBlockRequest := *openapiclient.NewMoveBlockRequest(int32(123)) // MoveBlockRequest | 
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NotesAPI.MoveBlock(context.Background(), id).MoveBlockRequest(moveBlockRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.MoveBlock``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MoveBlock`: SuccessFlag
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.MoveBlock`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Block id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiMoveBlockRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **moveBlockRequest** | [**MoveBlockRequest**](MoveBlockRequest.md) |  | 
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**SuccessFlag**](SuccessFlag.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RotateNoteShareToken

> ShareSettings RotateNoteShareToken(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Rotate the share token, invalidating any outstanding URLs.

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
	id := "id_example" // string | Note id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NotesAPI.RotateNoteShareToken(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.RotateNoteShareToken``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RotateNoteShareToken`: ShareSettings
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.RotateNoteShareToken`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Note id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRotateNoteShareTokenRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**ShareSettings**](ShareSettings.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateBlock

> Block UpdateBlock(ctx, id).UpdateBlockRequest(updateBlockRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Update a block (partial).

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
	id := "id_example" // string | Block id.
	updateBlockRequest := *openapiclient.NewUpdateBlockRequest() // UpdateBlockRequest | 
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NotesAPI.UpdateBlock(context.Background(), id).UpdateBlockRequest(updateBlockRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.UpdateBlock``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateBlock`: Block
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.UpdateBlock`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Block id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateBlockRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateBlockRequest** | [**UpdateBlockRequest**](UpdateBlockRequest.md) |  | 
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**Block**](Block.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateNote

> Note UpdateNote(ctx, id).UpdateNoteRequest(updateNoteRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Update a note (partial).

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
	id := "id_example" // string | Note id.
	updateNoteRequest := *openapiclient.NewUpdateNoteRequest() // UpdateNoteRequest | 
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NotesAPI.UpdateNote(context.Background(), id).UpdateNoteRequest(updateNoteRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.UpdateNote``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateNote`: Note
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.UpdateNote`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Note id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateNoteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateNoteRequest** | [**UpdateNoteRequest**](UpdateNoteRequest.md) |  | 
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**Note**](Note.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateNoteComment

> CommentMutationResponse UpdateNoteComment(ctx, id, commentId).UpdateCommentRequest(updateCommentRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Edit a comment.



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
	id := "id_example" // string | Note id.
	commentId := "commentId_example" // string | Comment id.
	updateCommentRequest := *openapiclient.NewUpdateCommentRequest() // UpdateCommentRequest | 
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NotesAPI.UpdateNoteComment(context.Background(), id, commentId).UpdateCommentRequest(updateCommentRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.UpdateNoteComment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateNoteComment`: CommentMutationResponse
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.UpdateNoteComment`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Note id. | 
**commentId** | **string** | Comment id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateNoteCommentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **updateCommentRequest** | [**UpdateCommentRequest**](UpdateCommentRequest.md) |  | 
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**CommentMutationResponse**](CommentMutationResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## WorkspaceCreateNote

> map[string]interface{} WorkspaceCreateNote(ctx, org, workspace).RequestBody(requestBody).Execute()



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
	resp, r, err := apiClient.NotesAPI.WorkspaceCreateNote(context.Background(), org, workspace).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.WorkspaceCreateNote``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceCreateNote`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.WorkspaceCreateNote`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceCreateNoteRequest struct via the builder pattern


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


## WorkspaceCreateNoteBlock

> map[string]interface{} WorkspaceCreateNoteBlock(ctx, org, workspace, id).RequestBody(requestBody).Execute()



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
	resp, r, err := apiClient.NotesAPI.WorkspaceCreateNoteBlock(context.Background(), org, workspace, id).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.WorkspaceCreateNoteBlock``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceCreateNoteBlock`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.WorkspaceCreateNoteBlock`: %v\n", resp)
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

Other parameters are passed through a pointer to a apiWorkspaceCreateNoteBlockRequest struct via the builder pattern


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


## WorkspaceDeleteNote

> WorkspaceDeleteNote(ctx, org, workspace, id).Execute()



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
	r, err := apiClient.NotesAPI.WorkspaceDeleteNote(context.Background(), org, workspace, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.WorkspaceDeleteNote``: %v\n", err)
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

Other parameters are passed through a pointer to a apiWorkspaceDeleteNoteRequest struct via the builder pattern


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


## WorkspaceDeleteNoteBlock

> WorkspaceDeleteNoteBlock(ctx, org, workspace, id).Execute()



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
	r, err := apiClient.NotesAPI.WorkspaceDeleteNoteBlock(context.Background(), org, workspace, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.WorkspaceDeleteNoteBlock``: %v\n", err)
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

Other parameters are passed through a pointer to a apiWorkspaceDeleteNoteBlockRequest struct via the builder pattern


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


## WorkspaceGetNote

> map[string]interface{} WorkspaceGetNote(ctx, org, workspace, id).Execute()



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
	resp, r, err := apiClient.NotesAPI.WorkspaceGetNote(context.Background(), org, workspace, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.WorkspaceGetNote``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceGetNote`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.WorkspaceGetNote`: %v\n", resp)
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

Other parameters are passed through a pointer to a apiWorkspaceGetNoteRequest struct via the builder pattern


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


## WorkspaceGetNoteBlock

> map[string]interface{} WorkspaceGetNoteBlock(ctx, org, workspace, id).Execute()



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
	resp, r, err := apiClient.NotesAPI.WorkspaceGetNoteBlock(context.Background(), org, workspace, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.WorkspaceGetNoteBlock``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceGetNoteBlock`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.WorkspaceGetNoteBlock`: %v\n", resp)
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

Other parameters are passed through a pointer to a apiWorkspaceGetNoteBlockRequest struct via the builder pattern


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


## WorkspaceListNoteBlocks

> map[string]interface{} WorkspaceListNoteBlocks(ctx, org, workspace, id).Execute()



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
	resp, r, err := apiClient.NotesAPI.WorkspaceListNoteBlocks(context.Background(), org, workspace, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.WorkspaceListNoteBlocks``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceListNoteBlocks`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.WorkspaceListNoteBlocks`: %v\n", resp)
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

Other parameters are passed through a pointer to a apiWorkspaceListNoteBlocksRequest struct via the builder pattern


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


## WorkspaceListNotes

> map[string]interface{} WorkspaceListNotes(ctx, org, workspace).Execute()



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
	resp, r, err := apiClient.NotesAPI.WorkspaceListNotes(context.Background(), org, workspace).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.WorkspaceListNotes``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceListNotes`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.WorkspaceListNotes`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceListNotesRequest struct via the builder pattern


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


## WorkspaceMoveNoteBlock

> map[string]interface{} WorkspaceMoveNoteBlock(ctx, org, workspace, id).RequestBody(requestBody).Execute()



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
	resp, r, err := apiClient.NotesAPI.WorkspaceMoveNoteBlock(context.Background(), org, workspace, id).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.WorkspaceMoveNoteBlock``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceMoveNoteBlock`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.WorkspaceMoveNoteBlock`: %v\n", resp)
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

Other parameters are passed through a pointer to a apiWorkspaceMoveNoteBlockRequest struct via the builder pattern


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


## WorkspaceUpdateNote

> map[string]interface{} WorkspaceUpdateNote(ctx, org, workspace, id).RequestBody(requestBody).Execute()



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
	resp, r, err := apiClient.NotesAPI.WorkspaceUpdateNote(context.Background(), org, workspace, id).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.WorkspaceUpdateNote``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceUpdateNote`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.WorkspaceUpdateNote`: %v\n", resp)
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

Other parameters are passed through a pointer to a apiWorkspaceUpdateNoteRequest struct via the builder pattern


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


## WorkspaceUpdateNoteBlock

> map[string]interface{} WorkspaceUpdateNoteBlock(ctx, org, workspace, id).RequestBody(requestBody).Execute()



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
	resp, r, err := apiClient.NotesAPI.WorkspaceUpdateNoteBlock(context.Background(), org, workspace, id).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NotesAPI.WorkspaceUpdateNoteBlock``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceUpdateNoteBlock`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `NotesAPI.WorkspaceUpdateNoteBlock`: %v\n", resp)
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

Other parameters are passed through a pointer to a apiWorkspaceUpdateNoteBlockRequest struct via the builder pattern


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

