# \NativeDMAPI

All URIs are relative to *https://api.spatio.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AddNativeDMReaction**](NativeDMAPI.md#AddNativeDMReaction) | **Post** /v1/native/dm/messages/{messageId}/reactions | Add a reaction to a DM message.
[**AttachToNativeDMMessage**](NativeDMAPI.md#AttachToNativeDMMessage) | **Post** /v1/native/dm/messages/{messageId}/attachments | Attach a file to a DM message.
[**DeleteNativeDMMessage**](NativeDMAPI.md#DeleteNativeDMMessage) | **Delete** /v1/native/dm/{dmId}/messages/{messageId} | Delete a DM message.
[**ForwardNativeDMMessage**](NativeDMAPI.md#ForwardNativeDMMessage) | **Post** /v1/native/dm/messages/{messageId}/forward | Forward a DM message to another conversation.
[**ListNativeDMChannels**](NativeDMAPI.md#ListNativeDMChannels) | **Get** /v1/native/dm | List the caller&#39;s DM channels.
[**ListNativeDMConversations**](NativeDMAPI.md#ListNativeDMConversations) | **Get** /v1/native/dm/conversations | List DM conversations with metadata (last message, unread count, etc.).
[**ListNativeDMMessages**](NativeDMAPI.md#ListNativeDMMessages) | **Get** /v1/native/dm/{dmId}/messages | List messages in a DM.
[**ListNativeDMPinnedMessages**](NativeDMAPI.md#ListNativeDMPinnedMessages) | **Get** /v1/native/dm/{dmId}/pinned | List pinned messages in a DM.
[**ListNativeDMThreadReplies**](NativeDMAPI.md#ListNativeDMThreadReplies) | **Get** /v1/native/dm/{dmId}/messages/{messageId}/replies | List threaded replies on a message.
[**MarkNativeDMRead**](NativeDMAPI.md#MarkNativeDMRead) | **Post** /v1/native/dm/{dmId}/read | Mark a DM as read.
[**MuteNativeDM**](NativeDMAPI.md#MuteNativeDM) | **Post** /v1/native/dm/{dmId}/mute | Mute a DM.
[**PinNativeDMConversation**](NativeDMAPI.md#PinNativeDMConversation) | **Post** /v1/native/dm/{dmId}/pin | Pin a DM conversation in the sidebar.
[**PinNativeDMMessage**](NativeDMAPI.md#PinNativeDMMessage) | **Post** /v1/native/dm/messages/{messageId}/pin | Pin a DM message.
[**PostNativeDMMessage**](NativeDMAPI.md#PostNativeDMMessage) | **Post** /v1/native/dm | Post a DM message (top-level entry).
[**PostNativeDMThreadReply**](NativeDMAPI.md#PostNativeDMThreadReply) | **Post** /v1/native/dm/{dmId}/messages/{messageId}/replies | Post a threaded reply.
[**RemoveNativeDMReaction**](NativeDMAPI.md#RemoveNativeDMReaction) | **Delete** /v1/native/dm/messages/{messageId}/reactions/{emoji} | Remove a reaction.
[**SearchNativeDMMessages**](NativeDMAPI.md#SearchNativeDMMessages) | **Get** /v1/native/dm/search | Search DM messages.
[**SetNativeDMDraft**](NativeDMAPI.md#SetNativeDMDraft) | **Put** /v1/native/dm/{dmId}/draft | Save a draft on a DM conversation.
[**UnpinNativeDMConversation**](NativeDMAPI.md#UnpinNativeDMConversation) | **Delete** /v1/native/dm/{dmId}/pin | Unpin a DM conversation.
[**UnpinNativeDMMessage**](NativeDMAPI.md#UnpinNativeDMMessage) | **Delete** /v1/native/dm/messages/{messageId}/pin | Unpin a DM message.
[**UpdateNativeDMMessage**](NativeDMAPI.md#UpdateNativeDMMessage) | **Patch** /v1/native/dm/{dmId}/messages/{messageId} | Update a DM message body.



## AddNativeDMReaction

> map[string]interface{} AddNativeDMReaction(ctx, messageId).RequestBody(requestBody).Execute()

Add a reaction to a DM message.

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
	messageId := "messageId_example" // string | 
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NativeDMAPI.AddNativeDMReaction(context.Background(), messageId).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NativeDMAPI.AddNativeDMReaction``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AddNativeDMReaction`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `NativeDMAPI.AddNativeDMReaction`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**messageId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiAddNativeDMReactionRequest struct via the builder pattern


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


## AttachToNativeDMMessage

> map[string]interface{} AttachToNativeDMMessage(ctx, messageId).RequestBody(requestBody).Execute()

Attach a file to a DM message.

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
	messageId := "messageId_example" // string | 
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NativeDMAPI.AttachToNativeDMMessage(context.Background(), messageId).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NativeDMAPI.AttachToNativeDMMessage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AttachToNativeDMMessage`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `NativeDMAPI.AttachToNativeDMMessage`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**messageId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiAttachToNativeDMMessageRequest struct via the builder pattern


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


## DeleteNativeDMMessage

> DeleteNativeDMMessage(ctx, dmId, messageId).Execute()

Delete a DM message.

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
	dmId := "dmId_example" // string | 
	messageId := "messageId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.NativeDMAPI.DeleteNativeDMMessage(context.Background(), dmId, messageId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NativeDMAPI.DeleteNativeDMMessage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dmId** | **string** |  | 
**messageId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteNativeDMMessageRequest struct via the builder pattern


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


## ForwardNativeDMMessage

> map[string]interface{} ForwardNativeDMMessage(ctx, messageId).RequestBody(requestBody).Execute()

Forward a DM message to another conversation.

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
	messageId := "messageId_example" // string | 
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NativeDMAPI.ForwardNativeDMMessage(context.Background(), messageId).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NativeDMAPI.ForwardNativeDMMessage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ForwardNativeDMMessage`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `NativeDMAPI.ForwardNativeDMMessage`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**messageId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiForwardNativeDMMessageRequest struct via the builder pattern


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


## ListNativeDMChannels

> map[string]interface{} ListNativeDMChannels(ctx).Execute()

List the caller's DM channels.

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
	resp, r, err := apiClient.NativeDMAPI.ListNativeDMChannels(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NativeDMAPI.ListNativeDMChannels``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListNativeDMChannels`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `NativeDMAPI.ListNativeDMChannels`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListNativeDMChannelsRequest struct via the builder pattern


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


## ListNativeDMConversations

> map[string]interface{} ListNativeDMConversations(ctx).Execute()

List DM conversations with metadata (last message, unread count, etc.).

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
	resp, r, err := apiClient.NativeDMAPI.ListNativeDMConversations(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NativeDMAPI.ListNativeDMConversations``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListNativeDMConversations`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `NativeDMAPI.ListNativeDMConversations`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListNativeDMConversationsRequest struct via the builder pattern


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


## ListNativeDMMessages

> map[string]interface{} ListNativeDMMessages(ctx, dmId).Execute()

List messages in a DM.

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
	dmId := "dmId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NativeDMAPI.ListNativeDMMessages(context.Background(), dmId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NativeDMAPI.ListNativeDMMessages``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListNativeDMMessages`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `NativeDMAPI.ListNativeDMMessages`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dmId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListNativeDMMessagesRequest struct via the builder pattern


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


## ListNativeDMPinnedMessages

> map[string]interface{} ListNativeDMPinnedMessages(ctx, dmId).Execute()

List pinned messages in a DM.

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
	dmId := "dmId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NativeDMAPI.ListNativeDMPinnedMessages(context.Background(), dmId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NativeDMAPI.ListNativeDMPinnedMessages``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListNativeDMPinnedMessages`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `NativeDMAPI.ListNativeDMPinnedMessages`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dmId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListNativeDMPinnedMessagesRequest struct via the builder pattern


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


## ListNativeDMThreadReplies

> map[string]interface{} ListNativeDMThreadReplies(ctx, dmId, messageId).Execute()

List threaded replies on a message.

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
	dmId := "dmId_example" // string | 
	messageId := "messageId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NativeDMAPI.ListNativeDMThreadReplies(context.Background(), dmId, messageId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NativeDMAPI.ListNativeDMThreadReplies``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListNativeDMThreadReplies`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `NativeDMAPI.ListNativeDMThreadReplies`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dmId** | **string** |  | 
**messageId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListNativeDMThreadRepliesRequest struct via the builder pattern


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


## MarkNativeDMRead

> MarkNativeDMRead(ctx, dmId).Execute()

Mark a DM as read.

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
	dmId := "dmId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.NativeDMAPI.MarkNativeDMRead(context.Background(), dmId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NativeDMAPI.MarkNativeDMRead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dmId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiMarkNativeDMReadRequest struct via the builder pattern


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


## MuteNativeDM

> MuteNativeDM(ctx, dmId).RequestBody(requestBody).Execute()

Mute a DM.

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
	dmId := "dmId_example" // string | 
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.NativeDMAPI.MuteNativeDM(context.Background(), dmId).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NativeDMAPI.MuteNativeDM``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dmId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiMuteNativeDMRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **requestBody** | **map[string]interface{}** |  | 

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


## PinNativeDMConversation

> PinNativeDMConversation(ctx, dmId).Execute()

Pin a DM conversation in the sidebar.

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
	dmId := "dmId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.NativeDMAPI.PinNativeDMConversation(context.Background(), dmId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NativeDMAPI.PinNativeDMConversation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dmId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPinNativeDMConversationRequest struct via the builder pattern


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


## PinNativeDMMessage

> PinNativeDMMessage(ctx, messageId).Execute()

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
	messageId := "messageId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.NativeDMAPI.PinNativeDMMessage(context.Background(), messageId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NativeDMAPI.PinNativeDMMessage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**messageId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPinNativeDMMessageRequest struct via the builder pattern


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


## PostNativeDMMessage

> map[string]interface{} PostNativeDMMessage(ctx).RequestBody(requestBody).Execute()

Post a DM message (top-level entry).

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
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NativeDMAPI.PostNativeDMMessage(context.Background()).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NativeDMAPI.PostNativeDMMessage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PostNativeDMMessage`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `NativeDMAPI.PostNativeDMMessage`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiPostNativeDMMessageRequest struct via the builder pattern


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


## PostNativeDMThreadReply

> map[string]interface{} PostNativeDMThreadReply(ctx, dmId, messageId).RequestBody(requestBody).Execute()

Post a threaded reply.

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
	dmId := "dmId_example" // string | 
	messageId := "messageId_example" // string | 
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NativeDMAPI.PostNativeDMThreadReply(context.Background(), dmId, messageId).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NativeDMAPI.PostNativeDMThreadReply``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PostNativeDMThreadReply`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `NativeDMAPI.PostNativeDMThreadReply`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dmId** | **string** |  | 
**messageId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPostNativeDMThreadReplyRequest struct via the builder pattern


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


## RemoveNativeDMReaction

> RemoveNativeDMReaction(ctx, messageId, emoji).Execute()

Remove a reaction.

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
	messageId := "messageId_example" // string | 
	emoji := "emoji_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.NativeDMAPI.RemoveNativeDMReaction(context.Background(), messageId, emoji).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NativeDMAPI.RemoveNativeDMReaction``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**messageId** | **string** |  | 
**emoji** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRemoveNativeDMReactionRequest struct via the builder pattern


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


## SearchNativeDMMessages

> map[string]interface{} SearchNativeDMMessages(ctx).Q(q).Execute()

Search DM messages.

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
	q := "q_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NativeDMAPI.SearchNativeDMMessages(context.Background()).Q(q).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NativeDMAPI.SearchNativeDMMessages``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SearchNativeDMMessages`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `NativeDMAPI.SearchNativeDMMessages`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSearchNativeDMMessagesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** |  | 

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


## SetNativeDMDraft

> SetNativeDMDraft(ctx, dmId).RequestBody(requestBody).Execute()

Save a draft on a DM conversation.

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
	dmId := "dmId_example" // string | 
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.NativeDMAPI.SetNativeDMDraft(context.Background(), dmId).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NativeDMAPI.SetNativeDMDraft``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dmId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiSetNativeDMDraftRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **requestBody** | **map[string]interface{}** |  | 

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


## UnpinNativeDMConversation

> UnpinNativeDMConversation(ctx, dmId).Execute()

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
	dmId := "dmId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.NativeDMAPI.UnpinNativeDMConversation(context.Background(), dmId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NativeDMAPI.UnpinNativeDMConversation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dmId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUnpinNativeDMConversationRequest struct via the builder pattern


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


## UnpinNativeDMMessage

> UnpinNativeDMMessage(ctx, messageId).Execute()

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
	messageId := "messageId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.NativeDMAPI.UnpinNativeDMMessage(context.Background(), messageId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NativeDMAPI.UnpinNativeDMMessage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**messageId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUnpinNativeDMMessageRequest struct via the builder pattern


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


## UpdateNativeDMMessage

> map[string]interface{} UpdateNativeDMMessage(ctx, dmId, messageId).RequestBody(requestBody).Execute()

Update a DM message body.

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
	dmId := "dmId_example" // string | 
	messageId := "messageId_example" // string | 
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NativeDMAPI.UpdateNativeDMMessage(context.Background(), dmId, messageId).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NativeDMAPI.UpdateNativeDMMessage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateNativeDMMessage`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `NativeDMAPI.UpdateNativeDMMessage`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dmId** | **string** |  | 
**messageId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateNativeDMMessageRequest struct via the builder pattern


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

