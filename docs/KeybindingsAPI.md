# \KeybindingsAPI

All URIs are relative to *https://api.spatio.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**DeleteKeyBinding**](KeybindingsAPI.md#DeleteKeyBinding) | **Delete** /v1/keybindings/{id} | Reset a binding to its platform default.
[**GetDefaultKeyBindings**](KeybindingsAPI.md#GetDefaultKeyBindings) | **Get** /v1/keybindings/defaults | Platform default key bindings (no user customizations applied).
[**ListKeyBindings**](KeybindingsAPI.md#ListKeyBindings) | **Get** /v1/keybindings | User&#39;s merged key bindings (defaults + customizations).
[**ResetAllKeyBindings**](KeybindingsAPI.md#ResetAllKeyBindings) | **Post** /v1/keybindings/reset | Reset every customization to its platform default.
[**UpdateKeyBinding**](KeybindingsAPI.md#UpdateKeyBinding) | **Put** /v1/keybindings/{id} | Create or update a user key-binding customization.
[**ValidateKeyBinding**](KeybindingsAPI.md#ValidateKeyBinding) | **Post** /v1/keybindings/validate | Check whether a proposed binding conflicts with existing ones.



## DeleteKeyBinding

> DeleteKeyBinding(ctx, id).Execute()

Reset a binding to its platform default.

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
	r, err := apiClient.KeybindingsAPI.DeleteKeyBinding(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `KeybindingsAPI.DeleteKeyBinding``: %v\n", err)
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

Other parameters are passed through a pointer to a apiDeleteKeyBindingRequest struct via the builder pattern


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


## GetDefaultKeyBindings

> KeyBindingListResponse GetDefaultKeyBindings(ctx).Execute()

Platform default key bindings (no user customizations applied).

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
	resp, r, err := apiClient.KeybindingsAPI.GetDefaultKeyBindings(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `KeybindingsAPI.GetDefaultKeyBindings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetDefaultKeyBindings`: KeyBindingListResponse
	fmt.Fprintf(os.Stdout, "Response from `KeybindingsAPI.GetDefaultKeyBindings`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetDefaultKeyBindingsRequest struct via the builder pattern


### Return type

[**KeyBindingListResponse**](KeyBindingListResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListKeyBindings

> KeyBindingListResponse ListKeyBindings(ctx).Execute()

User's merged key bindings (defaults + customizations).

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
	resp, r, err := apiClient.KeybindingsAPI.ListKeyBindings(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `KeybindingsAPI.ListKeyBindings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListKeyBindings`: KeyBindingListResponse
	fmt.Fprintf(os.Stdout, "Response from `KeybindingsAPI.ListKeyBindings`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListKeyBindingsRequest struct via the builder pattern


### Return type

[**KeyBindingListResponse**](KeyBindingListResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ResetAllKeyBindings

> ResetAllKeyBindings(ctx).Execute()

Reset every customization to its platform default.

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
	r, err := apiClient.KeybindingsAPI.ResetAllKeyBindings(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `KeybindingsAPI.ResetAllKeyBindings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiResetAllKeyBindingsRequest struct via the builder pattern


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


## UpdateKeyBinding

> KeyBinding UpdateKeyBinding(ctx, id).UpdateKeyBindingRequest(updateKeyBindingRequest).Execute()

Create or update a user key-binding customization.

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
	updateKeyBindingRequest := *openapiclient.NewUpdateKeyBindingRequest("Key_example") // UpdateKeyBindingRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.KeybindingsAPI.UpdateKeyBinding(context.Background(), id).UpdateKeyBindingRequest(updateKeyBindingRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `KeybindingsAPI.UpdateKeyBinding``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateKeyBinding`: KeyBinding
	fmt.Fprintf(os.Stdout, "Response from `KeybindingsAPI.UpdateKeyBinding`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateKeyBindingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateKeyBindingRequest** | [**UpdateKeyBindingRequest**](UpdateKeyBindingRequest.md) |  | 

### Return type

[**KeyBinding**](KeyBinding.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ValidateKeyBinding

> ValidateKeyBindingResponse ValidateKeyBinding(ctx).ValidateKeyBindingRequest(validateKeyBindingRequest).Execute()

Check whether a proposed binding conflicts with existing ones.

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
	validateKeyBindingRequest := *openapiclient.NewValidateKeyBindingRequest("ActionId_example", "Key_example") // ValidateKeyBindingRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.KeybindingsAPI.ValidateKeyBinding(context.Background()).ValidateKeyBindingRequest(validateKeyBindingRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `KeybindingsAPI.ValidateKeyBinding``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ValidateKeyBinding`: ValidateKeyBindingResponse
	fmt.Fprintf(os.Stdout, "Response from `KeybindingsAPI.ValidateKeyBinding`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiValidateKeyBindingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **validateKeyBindingRequest** | [**ValidateKeyBindingRequest**](ValidateKeyBindingRequest.md) |  | 

### Return type

[**ValidateKeyBindingResponse**](ValidateKeyBindingResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

