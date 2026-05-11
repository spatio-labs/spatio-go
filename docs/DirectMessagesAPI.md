# \DirectMessagesAPI

All URIs are relative to *https://api.spatio.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AddDMReaction**](DirectMessagesAPI.md#AddDMReaction) | **Post** /v1/direct-messages/messages/{messageId}/reactions | React to a DM message.
[**AttachToDMMessage**](DirectMessagesAPI.md#AttachToDMMessage) | **Post** /v1/direct-messages/messages/{messageId}/attachments | Attach a file/image/etc. to an existing DM message.
[**ExecuteDMAction**](DirectMessagesAPI.md#ExecuteDMAction) | **Post** /v1/direct-messages/execute | Dispatch a DM action by id.
[**ForwardDMMessage**](DirectMessagesAPI.md#ForwardDMMessage) | **Post** /v1/direct-messages/messages/{messageId}/forward | Forward a DM message to another DM or channel.
[**GetDMUser**](DirectMessagesAPI.md#GetDMUser) | **Get** /v1/direct-messages/users/{id} | Fetch one chat user.
[**ListDMActions**](DirectMessagesAPI.md#ListDMActions) | **Get** /v1/direct-messages/actions | Discover the action catalog for DirectMessages.
[**ListDMPinnedMessages**](DirectMessagesAPI.md#ListDMPinnedMessages) | **Get** /v1/direct-messages/{dmId}/pinned | List pinned messages in a DM conversation.
[**ListDMThreadReplies**](DirectMessagesAPI.md#ListDMThreadReplies) | **Get** /v1/direct-messages/{dmId}/messages/{messageId}/replies | List replies in a DM message thread.
[**ListDMUsers**](DirectMessagesAPI.md#ListDMUsers) | **Get** /v1/direct-messages/users | List chat users (DM contacts) across connected accounts.
[**ListDirectConversationsEnriched**](DirectMessagesAPI.md#ListDirectConversationsEnriched) | **Get** /v1/direct-messages/conversations | Enriched DM conversation list with unread + pin + draft state.
[**ListDirectMessageConversations**](DirectMessagesAPI.md#ListDirectMessageConversations) | **Get** /v1/direct-messages | List 1:1 and group DM conversations.
[**ListDirectMessages**](DirectMessagesAPI.md#ListDirectMessages) | **Get** /v1/direct-messages/messages | List messages in a DM conversation.
[**MarkDMRead**](DirectMessagesAPI.md#MarkDMRead) | **Post** /v1/direct-messages/{dmId}/read | Mark a DM message read.
[**MuteDM**](DirectMessagesAPI.md#MuteDM) | **Post** /v1/direct-messages/{dmId}/mute | Mute a DM conversation (until a time, or forever).
[**PinDMConversation**](DirectMessagesAPI.md#PinDMConversation) | **Post** /v1/direct-messages/{dmId}/pin | Pin a DM conversation to the top of the sidebar.
[**PinDMMessage**](DirectMessagesAPI.md#PinDMMessage) | **Post** /v1/direct-messages/messages/{messageId}/pin | Pin a DM message.
[**PostDMThreadReply**](DirectMessagesAPI.md#PostDMThreadReply) | **Post** /v1/direct-messages/{dmId}/messages/{messageId}/replies | Reply in a DM message thread.
[**RemoveDMReaction**](DirectMessagesAPI.md#RemoveDMReaction) | **Delete** /v1/direct-messages/messages/{messageId}/reactions/{emoji} | Remove a DM message reaction.
[**SearchDirectMessages**](DirectMessagesAPI.md#SearchDirectMessages) | **Get** /v1/direct-messages/search | Search across DM messages.
[**SendDirectMessage**](DirectMessagesAPI.md#SendDirectMessage) | **Post** /v1/direct-messages/messages | Send a DM.
[**SetDMDraft**](DirectMessagesAPI.md#SetDMDraft) | **Put** /v1/direct-messages/{dmId}/draft | Save the unsent draft text for a DM.
[**UnpinDMConversation**](DirectMessagesAPI.md#UnpinDMConversation) | **Delete** /v1/direct-messages/{dmId}/pin | Unpin a DM conversation.
[**UnpinDMMessage**](DirectMessagesAPI.md#UnpinDMMessage) | **Delete** /v1/direct-messages/messages/{messageId}/pin | Unpin a DM message.
[**WorkspaceExecuteDMAction**](DirectMessagesAPI.md#WorkspaceExecuteDMAction) | **Post** /v1/organizations/{org}/workspaces/{workspace}/direct-messages/execute | 
[**WorkspaceGetDMUser**](DirectMessagesAPI.md#WorkspaceGetDMUser) | **Get** /v1/organizations/{org}/workspaces/{workspace}/direct-messages/users/{id} | 
[**WorkspaceListDMActions**](DirectMessagesAPI.md#WorkspaceListDMActions) | **Get** /v1/organizations/{org}/workspaces/{workspace}/direct-messages/actions | 
[**WorkspaceListDMConversations**](DirectMessagesAPI.md#WorkspaceListDMConversations) | **Get** /v1/organizations/{org}/workspaces/{workspace}/direct-messages/conversations | 
[**WorkspaceListDMMessages**](DirectMessagesAPI.md#WorkspaceListDMMessages) | **Get** /v1/organizations/{org}/workspaces/{workspace}/direct-messages/messages | 
[**WorkspaceListDMUsers**](DirectMessagesAPI.md#WorkspaceListDMUsers) | **Get** /v1/organizations/{org}/workspaces/{workspace}/direct-messages/users | 
[**WorkspaceListDirectMessages**](DirectMessagesAPI.md#WorkspaceListDirectMessages) | **Get** /v1/organizations/{org}/workspaces/{workspace}/direct-messages | 
[**WorkspaceSendDirectMessage**](DirectMessagesAPI.md#WorkspaceSendDirectMessage) | **Post** /v1/organizations/{org}/workspaces/{workspace}/direct-messages/messages | 



## AddDMReaction

> DMReactionResponse AddDMReaction(ctx, messageId).DMReactionRequest(dMReactionRequest).Execute()

React to a DM message.

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
	messageId := "messageId_example" // string | Chat-message id.
	dMReactionRequest := *openapiclient.NewDMReactionRequest("Emoji_example") // DMReactionRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DirectMessagesAPI.AddDMReaction(context.Background(), messageId).DMReactionRequest(dMReactionRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.AddDMReaction``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AddDMReaction`: DMReactionResponse
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.AddDMReaction`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**messageId** | **string** | Chat-message id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiAddDMReactionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **dMReactionRequest** | [**DMReactionRequest**](DMReactionRequest.md) |  | 

### Return type

[**DMReactionResponse**](DMReactionResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AttachToDMMessage

> DMMessageEnvelope AttachToDMMessage(ctx, messageId).DMAttachRequest(dMAttachRequest).Execute()

Attach a file/image/etc. to an existing DM message.

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
	messageId := "messageId_example" // string | Chat-message id.
	dMAttachRequest := *openapiclient.NewDMAttachRequest("Kind_example", "Url_example") // DMAttachRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DirectMessagesAPI.AttachToDMMessage(context.Background(), messageId).DMAttachRequest(dMAttachRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.AttachToDMMessage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AttachToDMMessage`: DMMessageEnvelope
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.AttachToDMMessage`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**messageId** | **string** | Chat-message id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiAttachToDMMessageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **dMAttachRequest** | [**DMAttachRequest**](DMAttachRequest.md) |  | 

### Return type

[**DMMessageEnvelope**](DMMessageEnvelope.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ExecuteDMAction

> ExecuteChatActionResponse ExecuteDMAction(ctx).ExecuteChatActionRequest(executeChatActionRequest).Execute()

Dispatch a DM action by id.

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
	executeChatActionRequest := *openapiclient.NewExecuteChatActionRequest("ActionId_example") // ExecuteChatActionRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DirectMessagesAPI.ExecuteDMAction(context.Background()).ExecuteChatActionRequest(executeChatActionRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.ExecuteDMAction``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExecuteDMAction`: ExecuteChatActionResponse
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.ExecuteDMAction`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiExecuteDMActionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **executeChatActionRequest** | [**ExecuteChatActionRequest**](ExecuteChatActionRequest.md) |  | 

### Return type

[**ExecuteChatActionResponse**](ExecuteChatActionResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ForwardDMMessage

> DMMessageEnvelope ForwardDMMessage(ctx, messageId).DMForwardRequest(dMForwardRequest).Execute()

Forward a DM message to another DM or channel.

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
	messageId := "messageId_example" // string | Chat-message id.
	dMForwardRequest := *openapiclient.NewDMForwardRequest() // DMForwardRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DirectMessagesAPI.ForwardDMMessage(context.Background(), messageId).DMForwardRequest(dMForwardRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.ForwardDMMessage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ForwardDMMessage`: DMMessageEnvelope
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.ForwardDMMessage`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**messageId** | **string** | Chat-message id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiForwardDMMessageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **dMForwardRequest** | [**DMForwardRequest**](DMForwardRequest.md) |  | 

### Return type

[**DMMessageEnvelope**](DMMessageEnvelope.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetDMUser

> GetChatUserResponse GetDMUser(ctx, id).AccountId(accountId).Execute()

Fetch one chat user.

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
	id := "id_example" // string | Chat-user id (provider-scoped).
	accountId := "accountId_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DirectMessagesAPI.GetDMUser(context.Background(), id).AccountId(accountId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.GetDMUser``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetDMUser`: GetChatUserResponse
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.GetDMUser`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Chat-user id (provider-scoped). | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetDMUserRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **accountId** | **string** |  | 

### Return type

[**GetChatUserResponse**](GetChatUserResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListDMActions

> ChatActionsList ListDMActions(ctx).Execute()

Discover the action catalog for DirectMessages.

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
	resp, r, err := apiClient.DirectMessagesAPI.ListDMActions(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.ListDMActions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListDMActions`: ChatActionsList
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.ListDMActions`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListDMActionsRequest struct via the builder pattern


### Return type

[**ChatActionsList**](ChatActionsList.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListDMPinnedMessages

> DMPinnedList ListDMPinnedMessages(ctx, dmId).AccountId(accountId).Execute()

List pinned messages in a DM conversation.

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
	dmId := "dmId_example" // string | Direct-message conversation id.
	accountId := "accountId_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DirectMessagesAPI.ListDMPinnedMessages(context.Background(), dmId).AccountId(accountId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.ListDMPinnedMessages``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListDMPinnedMessages`: DMPinnedList
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.ListDMPinnedMessages`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dmId** | **string** | Direct-message conversation id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListDMPinnedMessagesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **accountId** | **string** |  | 

### Return type

[**DMPinnedList**](DMPinnedList.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListDMThreadReplies

> map[string]interface{} ListDMThreadReplies(ctx, dmId, messageId).AccountId(accountId).Execute()

List replies in a DM message thread.

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
	dmId := "dmId_example" // string | Direct-message conversation id.
	messageId := "messageId_example" // string | Chat-message id.
	accountId := "accountId_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DirectMessagesAPI.ListDMThreadReplies(context.Background(), dmId, messageId).AccountId(accountId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.ListDMThreadReplies``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListDMThreadReplies`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.ListDMThreadReplies`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dmId** | **string** | Direct-message conversation id. | 
**messageId** | **string** | Chat-message id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListDMThreadRepliesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **accountId** | **string** |  | 

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


## ListDMUsers

> ListChatUsersResponse ListDMUsers(ctx).AccountIds(accountIds).Providers(providers).XWorkspaceID(xWorkspaceID).Limit(limit).Cursor(cursor).Execute()

List chat users (DM contacts) across connected accounts.

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
	accountIds := []string{"Inner_example"} // []string | Repeatable. Restrict to these connected-account row ids. Mutually orthogonal to `providers` — when both are set the intersection is used.  (optional)
	providers := []string{"Inner_example"} // []string | Repeatable. Restrict to these provider ids (`gmail`, `outlook`). (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)
	limit := int32(56) // int32 |  (optional)
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DirectMessagesAPI.ListDMUsers(context.Background()).AccountIds(accountIds).Providers(providers).XWorkspaceID(xWorkspaceID).Limit(limit).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.ListDMUsers``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListDMUsers`: ListChatUsersResponse
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.ListDMUsers`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListDMUsersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accountIds** | **[]string** | Repeatable. Restrict to these connected-account row ids. Mutually orthogonal to &#x60;providers&#x60; — when both are set the intersection is used.  | 
 **providers** | **[]string** | Repeatable. Restrict to these provider ids (&#x60;gmail&#x60;, &#x60;outlook&#x60;). | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 
 **limit** | **int32** |  | 
 **cursor** | **string** |  | 

### Return type

[**ListChatUsersResponse**](ListChatUsersResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListDirectConversationsEnriched

> map[string]interface{} ListDirectConversationsEnriched(ctx).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Enriched DM conversation list with unread + pin + draft state.



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
	accountId := "accountId_example" // string |  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DirectMessagesAPI.ListDirectConversationsEnriched(context.Background()).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.ListDirectConversationsEnriched``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListDirectConversationsEnriched`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.ListDirectConversationsEnriched`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListDirectConversationsEnrichedRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accountId** | **string** |  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

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


## ListDirectMessageConversations

> ListChannelsResponse ListDirectMessageConversations(ctx).AccountIds(accountIds).Providers(providers).XWorkspaceID(xWorkspaceID).Limit(limit).Cursor(cursor).IncludeArchived(includeArchived).Execute()

List 1:1 and group DM conversations.



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
	accountIds := []string{"Inner_example"} // []string | Repeatable. Restrict to these connected-account row ids. Mutually orthogonal to `providers` — when both are set the intersection is used.  (optional)
	providers := []string{"Inner_example"} // []string | Repeatable. Restrict to these provider ids (`gmail`, `outlook`). (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)
	limit := int32(56) // int32 |  (optional)
	cursor := "cursor_example" // string |  (optional)
	includeArchived := true // bool |  (optional) (default to false)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DirectMessagesAPI.ListDirectMessageConversations(context.Background()).AccountIds(accountIds).Providers(providers).XWorkspaceID(xWorkspaceID).Limit(limit).Cursor(cursor).IncludeArchived(includeArchived).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.ListDirectMessageConversations``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListDirectMessageConversations`: ListChannelsResponse
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.ListDirectMessageConversations`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListDirectMessageConversationsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accountIds** | **[]string** | Repeatable. Restrict to these connected-account row ids. Mutually orthogonal to &#x60;providers&#x60; — when both are set the intersection is used.  | 
 **providers** | **[]string** | Repeatable. Restrict to these provider ids (&#x60;gmail&#x60;, &#x60;outlook&#x60;). | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 
 **limit** | **int32** |  | 
 **cursor** | **string** |  | 
 **includeArchived** | **bool** |  | [default to false]

### Return type

[**ListChannelsResponse**](ListChannelsResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListDirectMessages

> ListMessagesResponse ListDirectMessages(ctx).Channel(channel).AccountId(accountId).AccountIds(accountIds).Providers(providers).XWorkspaceID(xWorkspaceID).Limit(limit).Cursor(cursor).OldestFirst(oldestFirst).Execute()

List messages in a DM conversation.

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
	channel := "channel_example" // string | DM conversation id.
	accountId := "accountId_example" // string |  (optional)
	accountIds := []string{"Inner_example"} // []string | Repeatable. Restrict to these connected-account row ids. Mutually orthogonal to `providers` — when both are set the intersection is used.  (optional)
	providers := []string{"Inner_example"} // []string | Repeatable. Restrict to these provider ids (`gmail`, `outlook`). (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)
	limit := int32(56) // int32 |  (optional)
	cursor := "cursor_example" // string |  (optional)
	oldestFirst := true // bool |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DirectMessagesAPI.ListDirectMessages(context.Background()).Channel(channel).AccountId(accountId).AccountIds(accountIds).Providers(providers).XWorkspaceID(xWorkspaceID).Limit(limit).Cursor(cursor).OldestFirst(oldestFirst).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.ListDirectMessages``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListDirectMessages`: ListMessagesResponse
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.ListDirectMessages`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListDirectMessagesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **channel** | **string** | DM conversation id. | 
 **accountId** | **string** |  | 
 **accountIds** | **[]string** | Repeatable. Restrict to these connected-account row ids. Mutually orthogonal to &#x60;providers&#x60; — when both are set the intersection is used.  | 
 **providers** | **[]string** | Repeatable. Restrict to these provider ids (&#x60;gmail&#x60;, &#x60;outlook&#x60;). | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 
 **limit** | **int32** |  | 
 **cursor** | **string** |  | 
 **oldestFirst** | **bool** |  | 

### Return type

[**ListMessagesResponse**](ListMessagesResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MarkDMRead

> SuccessFlag MarkDMRead(ctx, dmId).DMMarkReadRequest(dMMarkReadRequest).Execute()

Mark a DM message read.

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
	dmId := "dmId_example" // string | Direct-message conversation id.
	dMMarkReadRequest := *openapiclient.NewDMMarkReadRequest("MessageId_example") // DMMarkReadRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DirectMessagesAPI.MarkDMRead(context.Background(), dmId).DMMarkReadRequest(dMMarkReadRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.MarkDMRead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MarkDMRead`: SuccessFlag
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.MarkDMRead`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dmId** | **string** | Direct-message conversation id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiMarkDMReadRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **dMMarkReadRequest** | [**DMMarkReadRequest**](DMMarkReadRequest.md) |  | 

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


## MuteDM

> DMMuteResponse MuteDM(ctx, dmId).DMMuteRequest(dMMuteRequest).Execute()

Mute a DM conversation (until a time, or forever).

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
	dmId := "dmId_example" // string | Direct-message conversation id.
	dMMuteRequest := *openapiclient.NewDMMuteRequest() // DMMuteRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DirectMessagesAPI.MuteDM(context.Background(), dmId).DMMuteRequest(dMMuteRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.MuteDM``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MuteDM`: DMMuteResponse
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.MuteDM`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dmId** | **string** | Direct-message conversation id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiMuteDMRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **dMMuteRequest** | [**DMMuteRequest**](DMMuteRequest.md) |  | 

### Return type

[**DMMuteResponse**](DMMuteResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PinDMConversation

> SuccessFlag PinDMConversation(ctx, dmId).AccountId(accountId).Execute()

Pin a DM conversation to the top of the sidebar.

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
	dmId := "dmId_example" // string | Direct-message conversation id.
	accountId := "accountId_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DirectMessagesAPI.PinDMConversation(context.Background(), dmId).AccountId(accountId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.PinDMConversation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PinDMConversation`: SuccessFlag
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.PinDMConversation`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dmId** | **string** | Direct-message conversation id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiPinDMConversationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **accountId** | **string** |  | 

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


## PinDMMessage

> SuccessFlag PinDMMessage(ctx, messageId).ChannelMembershipRequest(channelMembershipRequest).Execute()

Pin a DM message.

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
	messageId := "messageId_example" // string | Chat-message id.
	channelMembershipRequest := *openapiclient.NewChannelMembershipRequest() // ChannelMembershipRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DirectMessagesAPI.PinDMMessage(context.Background(), messageId).ChannelMembershipRequest(channelMembershipRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.PinDMMessage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PinDMMessage`: SuccessFlag
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.PinDMMessage`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**messageId** | **string** | Chat-message id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiPinDMMessageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **channelMembershipRequest** | [**ChannelMembershipRequest**](ChannelMembershipRequest.md) |  | 

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


## PostDMThreadReply

> DMMessageEnvelope PostDMThreadReply(ctx, dmId, messageId).DMThreadReplyRequest(dMThreadReplyRequest).AccountId(accountId).Execute()

Reply in a DM message thread.

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
	dmId := "dmId_example" // string | Direct-message conversation id.
	messageId := "messageId_example" // string | Chat-message id.
	dMThreadReplyRequest := *openapiclient.NewDMThreadReplyRequest("Content_example") // DMThreadReplyRequest | 
	accountId := "accountId_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DirectMessagesAPI.PostDMThreadReply(context.Background(), dmId, messageId).DMThreadReplyRequest(dMThreadReplyRequest).AccountId(accountId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.PostDMThreadReply``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PostDMThreadReply`: DMMessageEnvelope
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.PostDMThreadReply`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dmId** | **string** | Direct-message conversation id. | 
**messageId** | **string** | Chat-message id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiPostDMThreadReplyRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **dMThreadReplyRequest** | [**DMThreadReplyRequest**](DMThreadReplyRequest.md) |  | 
 **accountId** | **string** |  | 

### Return type

[**DMMessageEnvelope**](DMMessageEnvelope.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RemoveDMReaction

> DMReactionResponse RemoveDMReaction(ctx, messageId, emoji).AccountId(accountId).Execute()

Remove a DM message reaction.

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
	messageId := "messageId_example" // string | Chat-message id.
	emoji := "emoji_example" // string | Reaction emoji (e.g. `+1`, `eyes`, `pepper`).
	accountId := "accountId_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DirectMessagesAPI.RemoveDMReaction(context.Background(), messageId, emoji).AccountId(accountId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.RemoveDMReaction``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RemoveDMReaction`: DMReactionResponse
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.RemoveDMReaction`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**messageId** | **string** | Chat-message id. | 
**emoji** | **string** | Reaction emoji (e.g. &#x60;+1&#x60;, &#x60;eyes&#x60;, &#x60;pepper&#x60;). | 

### Other Parameters

Other parameters are passed through a pointer to a apiRemoveDMReactionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **accountId** | **string** |  | 

### Return type

[**DMReactionResponse**](DMReactionResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SearchDirectMessages

> DMSearchResults SearchDirectMessages(ctx).Q(q).Limit(limit).DmId(dmId).User(user).AccountId(accountId).Execute()

Search across DM messages.

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
	q := "q_example" // string | Free-form query string.
	limit := int32(56) // int32 |  (optional)
	dmId := "dmId_example" // string | Restrict to one conversation. (optional)
	user := "user_example" // string | Restrict to messages from this user id. (optional)
	accountId := "accountId_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DirectMessagesAPI.SearchDirectMessages(context.Background()).Q(q).Limit(limit).DmId(dmId).User(user).AccountId(accountId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.SearchDirectMessages``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SearchDirectMessages`: DMSearchResults
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.SearchDirectMessages`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSearchDirectMessagesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Free-form query string. | 
 **limit** | **int32** |  | 
 **dmId** | **string** | Restrict to one conversation. | 
 **user** | **string** | Restrict to messages from this user id. | 
 **accountId** | **string** |  | 

### Return type

[**DMSearchResults**](DMSearchResults.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SendDirectMessage

> SendChatMessageResponse SendDirectMessage(ctx).SendChatMessageRequest(sendChatMessageRequest).Execute()

Send a DM.

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
	sendChatMessageRequest := *openapiclient.NewSendChatMessageRequest("Channel_example", "Text_example") // SendChatMessageRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DirectMessagesAPI.SendDirectMessage(context.Background()).SendChatMessageRequest(sendChatMessageRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.SendDirectMessage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SendDirectMessage`: SendChatMessageResponse
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.SendDirectMessage`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSendDirectMessageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sendChatMessageRequest** | [**SendChatMessageRequest**](SendChatMessageRequest.md) |  | 

### Return type

[**SendChatMessageResponse**](SendChatMessageResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SetDMDraft

> SuccessFlag SetDMDraft(ctx, dmId).DMSetDraftRequest(dMSetDraftRequest).Execute()

Save the unsent draft text for a DM.

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
	dmId := "dmId_example" // string | Direct-message conversation id.
	dMSetDraftRequest := *openapiclient.NewDMSetDraftRequest("Text_example") // DMSetDraftRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DirectMessagesAPI.SetDMDraft(context.Background(), dmId).DMSetDraftRequest(dMSetDraftRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.SetDMDraft``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SetDMDraft`: SuccessFlag
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.SetDMDraft`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dmId** | **string** | Direct-message conversation id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiSetDMDraftRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **dMSetDraftRequest** | [**DMSetDraftRequest**](DMSetDraftRequest.md) |  | 

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


## UnpinDMConversation

> SuccessFlag UnpinDMConversation(ctx, dmId).AccountId(accountId).Execute()

Unpin a DM conversation.

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
	dmId := "dmId_example" // string | Direct-message conversation id.
	accountId := "accountId_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DirectMessagesAPI.UnpinDMConversation(context.Background(), dmId).AccountId(accountId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.UnpinDMConversation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UnpinDMConversation`: SuccessFlag
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.UnpinDMConversation`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dmId** | **string** | Direct-message conversation id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUnpinDMConversationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **accountId** | **string** |  | 

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


## UnpinDMMessage

> SuccessFlag UnpinDMMessage(ctx, messageId).AccountId(accountId).Execute()

Unpin a DM message.

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
	messageId := "messageId_example" // string | Chat-message id.
	accountId := "accountId_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DirectMessagesAPI.UnpinDMMessage(context.Background(), messageId).AccountId(accountId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.UnpinDMMessage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UnpinDMMessage`: SuccessFlag
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.UnpinDMMessage`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**messageId** | **string** | Chat-message id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUnpinDMMessageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **accountId** | **string** |  | 

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


## WorkspaceExecuteDMAction

> map[string]interface{} WorkspaceExecuteDMAction(ctx, org, workspace).RequestBody(requestBody).Execute()



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
	resp, r, err := apiClient.DirectMessagesAPI.WorkspaceExecuteDMAction(context.Background(), org, workspace).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.WorkspaceExecuteDMAction``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceExecuteDMAction`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.WorkspaceExecuteDMAction`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceExecuteDMActionRequest struct via the builder pattern


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


## WorkspaceGetDMUser

> map[string]interface{} WorkspaceGetDMUser(ctx, org, workspace, id).Execute()



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
	resp, r, err := apiClient.DirectMessagesAPI.WorkspaceGetDMUser(context.Background(), org, workspace, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.WorkspaceGetDMUser``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceGetDMUser`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.WorkspaceGetDMUser`: %v\n", resp)
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

Other parameters are passed through a pointer to a apiWorkspaceGetDMUserRequest struct via the builder pattern


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


## WorkspaceListDMActions

> map[string]interface{} WorkspaceListDMActions(ctx, org, workspace).Execute()



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
	resp, r, err := apiClient.DirectMessagesAPI.WorkspaceListDMActions(context.Background(), org, workspace).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.WorkspaceListDMActions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceListDMActions`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.WorkspaceListDMActions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceListDMActionsRequest struct via the builder pattern


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


## WorkspaceListDMConversations

> map[string]interface{} WorkspaceListDMConversations(ctx, org, workspace).Execute()



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
	resp, r, err := apiClient.DirectMessagesAPI.WorkspaceListDMConversations(context.Background(), org, workspace).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.WorkspaceListDMConversations``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceListDMConversations`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.WorkspaceListDMConversations`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceListDMConversationsRequest struct via the builder pattern


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


## WorkspaceListDMMessages

> map[string]interface{} WorkspaceListDMMessages(ctx, org, workspace).Execute()



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
	resp, r, err := apiClient.DirectMessagesAPI.WorkspaceListDMMessages(context.Background(), org, workspace).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.WorkspaceListDMMessages``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceListDMMessages`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.WorkspaceListDMMessages`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceListDMMessagesRequest struct via the builder pattern


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


## WorkspaceListDMUsers

> map[string]interface{} WorkspaceListDMUsers(ctx, org, workspace).Execute()



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
	resp, r, err := apiClient.DirectMessagesAPI.WorkspaceListDMUsers(context.Background(), org, workspace).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.WorkspaceListDMUsers``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceListDMUsers`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.WorkspaceListDMUsers`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceListDMUsersRequest struct via the builder pattern


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


## WorkspaceListDirectMessages

> map[string]interface{} WorkspaceListDirectMessages(ctx, org, workspace).Execute()



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
	resp, r, err := apiClient.DirectMessagesAPI.WorkspaceListDirectMessages(context.Background(), org, workspace).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.WorkspaceListDirectMessages``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceListDirectMessages`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.WorkspaceListDirectMessages`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceListDirectMessagesRequest struct via the builder pattern


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


## WorkspaceSendDirectMessage

> map[string]interface{} WorkspaceSendDirectMessage(ctx, org, workspace).RequestBody(requestBody).Execute()



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
	resp, r, err := apiClient.DirectMessagesAPI.WorkspaceSendDirectMessage(context.Background(), org, workspace).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DirectMessagesAPI.WorkspaceSendDirectMessage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceSendDirectMessage`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `DirectMessagesAPI.WorkspaceSendDirectMessage`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceSendDirectMessageRequest struct via the builder pattern


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

