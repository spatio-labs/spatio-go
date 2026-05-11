# \SlidesAPI

All URIs are relative to *https://api.spatio.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreatePresentation**](SlidesAPI.md#CreatePresentation) | **Post** /v1/slides | Create a presentation.
[**CreateSlide**](SlidesAPI.md#CreateSlide) | **Post** /v1/slides/{id}/slides | Insert a slide.
[**CreateSlideElement**](SlidesAPI.md#CreateSlideElement) | **Post** /v1/slides/{id}/slides/{slideId}/elements | Add a canvas element (text/shape/image) to a slide.
[**DeletePresentation**](SlidesAPI.md#DeletePresentation) | **Delete** /v1/slides/{id} | Delete a presentation.
[**DeleteSlide**](SlidesAPI.md#DeleteSlide) | **Delete** /v1/slides/{id}/slides/{slideId} | Delete a slide.
[**DeleteSlideElement**](SlidesAPI.md#DeleteSlideElement) | **Delete** /v1/slides/{id}/slides/{slideId}/elements/{elementId} | Delete a slide element.
[**DisablePresentationShare**](SlidesAPI.md#DisablePresentationShare) | **Delete** /v1/slides/{id}/share | Disable public sharing.
[**EnablePresentationShare**](SlidesAPI.md#EnablePresentationShare) | **Post** /v1/slides/{id}/share | Enable (or update password on) public sharing.
[**ExportPresentationPdf**](SlidesAPI.md#ExportPresentationPdf) | **Post** /v1/slides/{id}/export/pdf | Render the presentation as a PDF.
[**ExportPresentationPptx**](SlidesAPI.md#ExportPresentationPptx) | **Post** /v1/slides/{id}/export/pptx | Render the presentation as a PowerPoint (.pptx) file.
[**GetPresentation**](SlidesAPI.md#GetPresentation) | **Get** /v1/slides/{id} | Fetch one presentation.
[**GetPresentationShareSettings**](SlidesAPI.md#GetPresentationShareSettings) | **Get** /v1/slides/{id}/share | Fetch share settings for a presentation.
[**GetPublicPresentation**](SlidesAPI.md#GetPublicPresentation) | **Get** /public/slides/{token} | Fetch a publicly shared presentation.
[**GetSlide**](SlidesAPI.md#GetSlide) | **Get** /v1/slides/{id}/slides/{slideId} | Fetch one slide.
[**GetSlideElement**](SlidesAPI.md#GetSlideElement) | **Get** /v1/slides/{id}/slides/{slideId}/elements/{elementId} | Fetch one slide element.
[**ListPresentations**](SlidesAPI.md#ListPresentations) | **Get** /v1/slides | List presentations across connected accounts.
[**ListSlideElements**](SlidesAPI.md#ListSlideElements) | **Get** /v1/slides/{id}/slides/{slideId}/elements | List the canvas elements on a slide.
[**ListSlidesInPresentation**](SlidesAPI.md#ListSlidesInPresentation) | **Get** /v1/slides/{id}/slides | List slides in a presentation.
[**RotatePresentationShareToken**](SlidesAPI.md#RotatePresentationShareToken) | **Post** /v1/slides/{id}/share/rotate | Rotate the share token, invalidating outstanding URLs.
[**UpdatePresentation**](SlidesAPI.md#UpdatePresentation) | **Patch** /v1/slides/{id} | Update presentation metadata (partial).
[**UpdateSlide**](SlidesAPI.md#UpdateSlide) | **Patch** /v1/slides/{id}/slides/{slideId} | Update a slide (partial).
[**UpdateSlideElement**](SlidesAPI.md#UpdateSlideElement) | **Patch** /v1/slides/{id}/slides/{slideId}/elements/{elementId} | Update a slide element (partial).



## CreatePresentation

> Presentation CreatePresentation(ctx).CreatePresentationRequest(createPresentationRequest).AccountId(accountId).Provider(provider).XWorkspaceID(xWorkspaceID).Execute()

Create a presentation.



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
	createPresentationRequest := *openapiclient.NewCreatePresentationRequest("Title_example") // CreatePresentationRequest | 
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	provider := "provider_example" // string | Provider id (e.g. `native-notes`, `notion`). Selects every connected account for the provider. Mutually exclusive with `accountId`.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SlidesAPI.CreatePresentation(context.Background()).CreatePresentationRequest(createPresentationRequest).AccountId(accountId).Provider(provider).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SlidesAPI.CreatePresentation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreatePresentation`: Presentation
	fmt.Fprintf(os.Stdout, "Response from `SlidesAPI.CreatePresentation`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreatePresentationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createPresentationRequest** | [**CreatePresentationRequest**](CreatePresentationRequest.md) |  | 
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **provider** | **string** | Provider id (e.g. &#x60;native-notes&#x60;, &#x60;notion&#x60;). Selects every connected account for the provider. Mutually exclusive with &#x60;accountId&#x60;.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**Presentation**](Presentation.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateSlide

> Slide CreateSlide(ctx, id).CreateSlideRequest(createSlideRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Insert a slide.

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
	id := "id_example" // string | Presentation id.
	createSlideRequest := *openapiclient.NewCreateSlideRequest() // CreateSlideRequest | 
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SlidesAPI.CreateSlide(context.Background(), id).CreateSlideRequest(createSlideRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SlidesAPI.CreateSlide``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateSlide`: Slide
	fmt.Fprintf(os.Stdout, "Response from `SlidesAPI.CreateSlide`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Presentation id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateSlideRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createSlideRequest** | [**CreateSlideRequest**](CreateSlideRequest.md) |  | 
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**Slide**](Slide.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateSlideElement

> SlideElement CreateSlideElement(ctx, id, slideId).CreateSlideElementRequest(createSlideElementRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Add a canvas element (text/shape/image) to a slide.

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
	id := "id_example" // string | Presentation id.
	slideId := "slideId_example" // string | Slide id within the presentation.
	createSlideElementRequest := *openapiclient.NewCreateSlideElementRequest("ElementType_example") // CreateSlideElementRequest | 
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SlidesAPI.CreateSlideElement(context.Background(), id, slideId).CreateSlideElementRequest(createSlideElementRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SlidesAPI.CreateSlideElement``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateSlideElement`: SlideElement
	fmt.Fprintf(os.Stdout, "Response from `SlidesAPI.CreateSlideElement`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Presentation id. | 
**slideId** | **string** | Slide id within the presentation. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateSlideElementRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **createSlideElementRequest** | [**CreateSlideElementRequest**](CreateSlideElementRequest.md) |  | 
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**SlideElement**](SlideElement.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeletePresentation

> SuccessFlag DeletePresentation(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Delete a presentation.

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
	id := "id_example" // string | Presentation id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SlidesAPI.DeletePresentation(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SlidesAPI.DeletePresentation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeletePresentation`: SuccessFlag
	fmt.Fprintf(os.Stdout, "Response from `SlidesAPI.DeletePresentation`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Presentation id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeletePresentationRequest struct via the builder pattern


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


## DeleteSlide

> SuccessFlag DeleteSlide(ctx, id, slideId).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Delete a slide.

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
	id := "id_example" // string | Presentation id.
	slideId := "slideId_example" // string | Slide id within the presentation.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SlidesAPI.DeleteSlide(context.Background(), id, slideId).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SlidesAPI.DeleteSlide``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteSlide`: SuccessFlag
	fmt.Fprintf(os.Stdout, "Response from `SlidesAPI.DeleteSlide`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Presentation id. | 
**slideId** | **string** | Slide id within the presentation. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteSlideRequest struct via the builder pattern


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


## DeleteSlideElement

> SuccessFlag DeleteSlideElement(ctx, id, slideId, elementId).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Delete a slide element.

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
	id := "id_example" // string | Presentation id.
	slideId := "slideId_example" // string | Slide id within the presentation.
	elementId := "elementId_example" // string | Slide-element id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SlidesAPI.DeleteSlideElement(context.Background(), id, slideId, elementId).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SlidesAPI.DeleteSlideElement``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteSlideElement`: SuccessFlag
	fmt.Fprintf(os.Stdout, "Response from `SlidesAPI.DeleteSlideElement`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Presentation id. | 
**slideId** | **string** | Slide id within the presentation. | 
**elementId** | **string** | Slide-element id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteSlideElementRequest struct via the builder pattern


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


## DisablePresentationShare

> DisablePresentationShare(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

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
	id := "id_example" // string | Presentation id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.SlidesAPI.DisablePresentationShare(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SlidesAPI.DisablePresentationShare``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Presentation id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDisablePresentationShareRequest struct via the builder pattern


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


## EnablePresentationShare

> ShareSettings EnablePresentationShare(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).EnableShareRequest(enableShareRequest).Execute()

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
	id := "id_example" // string | Presentation id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)
	enableShareRequest := *openapiclient.NewEnableShareRequest() // EnableShareRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SlidesAPI.EnablePresentationShare(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).EnableShareRequest(enableShareRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SlidesAPI.EnablePresentationShare``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `EnablePresentationShare`: ShareSettings
	fmt.Fprintf(os.Stdout, "Response from `SlidesAPI.EnablePresentationShare`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Presentation id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiEnablePresentationShareRequest struct via the builder pattern


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


## ExportPresentationPdf

> *os.File ExportPresentationPdf(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Storage(storage).Filename(filename).ExportPDFRequest(exportPDFRequest).Execute()

Render the presentation as a PDF.



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
	id := "id_example" // string | Presentation id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)
	storage := "storage_example" // string |  (optional) (default to "stream")
	filename := "filename_example" // string | Sanitized base name for the downloaded PDF. (optional)
	exportPDFRequest := *openapiclient.NewExportPDFRequest() // ExportPDFRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SlidesAPI.ExportPresentationPdf(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Storage(storage).Filename(filename).ExportPDFRequest(exportPDFRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SlidesAPI.ExportPresentationPdf``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExportPresentationPdf`: *os.File
	fmt.Fprintf(os.Stdout, "Response from `SlidesAPI.ExportPresentationPdf`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Presentation id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiExportPresentationPdfRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 
 **storage** | **string** |  | [default to &quot;stream&quot;]
 **filename** | **string** | Sanitized base name for the downloaded PDF. | 
 **exportPDFRequest** | [**ExportPDFRequest**](ExportPDFRequest.md) |  | 

### Return type

[***os.File**](*os.File.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/pdf, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ExportPresentationPptx

> *os.File ExportPresentationPptx(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Storage(storage).Filename(filename).ExportPDFRequest(exportPDFRequest).Execute()

Render the presentation as a PowerPoint (.pptx) file.



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
	id := "id_example" // string | Presentation id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)
	storage := "storage_example" // string |  (optional) (default to "stream")
	filename := "filename_example" // string | Sanitized base name for the downloaded PPTX. (optional)
	exportPDFRequest := *openapiclient.NewExportPDFRequest() // ExportPDFRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SlidesAPI.ExportPresentationPptx(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Storage(storage).Filename(filename).ExportPDFRequest(exportPDFRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SlidesAPI.ExportPresentationPptx``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExportPresentationPptx`: *os.File
	fmt.Fprintf(os.Stdout, "Response from `SlidesAPI.ExportPresentationPptx`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Presentation id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiExportPresentationPptxRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 
 **storage** | **string** |  | [default to &quot;stream&quot;]
 **filename** | **string** | Sanitized base name for the downloaded PPTX. | 
 **exportPDFRequest** | [**ExportPDFRequest**](ExportPDFRequest.md) |  | 

### Return type

[***os.File**](*os.File.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/vnd.openxmlformats-officedocument.presentationml.presentation, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetPresentation

> Presentation GetPresentation(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Fetch one presentation.

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
	id := "id_example" // string | Presentation id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SlidesAPI.GetPresentation(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SlidesAPI.GetPresentation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetPresentation`: Presentation
	fmt.Fprintf(os.Stdout, "Response from `SlidesAPI.GetPresentation`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Presentation id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetPresentationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**Presentation**](Presentation.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetPresentationShareSettings

> ShareSettings GetPresentationShareSettings(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Fetch share settings for a presentation.



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
	id := "id_example" // string | Presentation id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SlidesAPI.GetPresentationShareSettings(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SlidesAPI.GetPresentationShareSettings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetPresentationShareSettings`: ShareSettings
	fmt.Fprintf(os.Stdout, "Response from `SlidesAPI.GetPresentationShareSettings`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Presentation id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetPresentationShareSettingsRequest struct via the builder pattern


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


## GetPublicPresentation

> map[string]interface{} GetPublicPresentation(ctx, token).Password(password).Execute()

Fetch a publicly shared presentation.



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
	resp, r, err := apiClient.SlidesAPI.GetPublicPresentation(context.Background(), token).Password(password).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SlidesAPI.GetPublicPresentation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetPublicPresentation`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `SlidesAPI.GetPublicPresentation`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**token** | **string** | Opaque public-share token. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetPublicPresentationRequest struct via the builder pattern


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


## GetSlide

> Slide GetSlide(ctx, id, slideId).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Fetch one slide.

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
	id := "id_example" // string | Presentation id.
	slideId := "slideId_example" // string | Slide id within the presentation.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SlidesAPI.GetSlide(context.Background(), id, slideId).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SlidesAPI.GetSlide``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetSlide`: Slide
	fmt.Fprintf(os.Stdout, "Response from `SlidesAPI.GetSlide`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Presentation id. | 
**slideId** | **string** | Slide id within the presentation. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetSlideRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**Slide**](Slide.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetSlideElement

> SlideElement GetSlideElement(ctx, id, slideId, elementId).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Fetch one slide element.

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
	id := "id_example" // string | Presentation id.
	slideId := "slideId_example" // string | Slide id within the presentation.
	elementId := "elementId_example" // string | Slide-element id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SlidesAPI.GetSlideElement(context.Background(), id, slideId, elementId).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SlidesAPI.GetSlideElement``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetSlideElement`: SlideElement
	fmt.Fprintf(os.Stdout, "Response from `SlidesAPI.GetSlideElement`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Presentation id. | 
**slideId** | **string** | Slide id within the presentation. | 
**elementId** | **string** | Slide-element id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetSlideElementRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**SlideElement**](SlideElement.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListPresentations

> PresentationListEnvelope ListPresentations(ctx).AccountId(accountId).Provider(provider).XWorkspaceID(xWorkspaceID).Limit(limit).Offset(offset).Execute()

List presentations across connected accounts.



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
	limit := int32(56) // int32 |  (optional) (default to 50)
	offset := int32(56) // int32 |  (optional) (default to 0)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SlidesAPI.ListPresentations(context.Background()).AccountId(accountId).Provider(provider).XWorkspaceID(xWorkspaceID).Limit(limit).Offset(offset).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SlidesAPI.ListPresentations``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListPresentations`: PresentationListEnvelope
	fmt.Fprintf(os.Stdout, "Response from `SlidesAPI.ListPresentations`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListPresentationsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **provider** | **string** | Provider id (e.g. &#x60;native-notes&#x60;, &#x60;notion&#x60;). Selects every connected account for the provider. Mutually exclusive with &#x60;accountId&#x60;.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 
 **limit** | **int32** |  | [default to 50]
 **offset** | **int32** |  | [default to 0]

### Return type

[**PresentationListEnvelope**](PresentationListEnvelope.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListSlideElements

> SlideElementList ListSlideElements(ctx, id, slideId).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

List the canvas elements on a slide.

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
	id := "id_example" // string | Presentation id.
	slideId := "slideId_example" // string | Slide id within the presentation.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SlidesAPI.ListSlideElements(context.Background(), id, slideId).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SlidesAPI.ListSlideElements``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListSlideElements`: SlideElementList
	fmt.Fprintf(os.Stdout, "Response from `SlidesAPI.ListSlideElements`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Presentation id. | 
**slideId** | **string** | Slide id within the presentation. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListSlideElementsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**SlideElementList**](SlideElementList.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListSlidesInPresentation

> SlideList ListSlidesInPresentation(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

List slides in a presentation.



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
	id := "id_example" // string | Presentation id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SlidesAPI.ListSlidesInPresentation(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SlidesAPI.ListSlidesInPresentation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListSlidesInPresentation`: SlideList
	fmt.Fprintf(os.Stdout, "Response from `SlidesAPI.ListSlidesInPresentation`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Presentation id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListSlidesInPresentationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**SlideList**](SlideList.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RotatePresentationShareToken

> ShareSettings RotatePresentationShareToken(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Rotate the share token, invalidating outstanding URLs.

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
	id := "id_example" // string | Presentation id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SlidesAPI.RotatePresentationShareToken(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SlidesAPI.RotatePresentationShareToken``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RotatePresentationShareToken`: ShareSettings
	fmt.Fprintf(os.Stdout, "Response from `SlidesAPI.RotatePresentationShareToken`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Presentation id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRotatePresentationShareTokenRequest struct via the builder pattern


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


## UpdatePresentation

> Presentation UpdatePresentation(ctx, id).UpdatePresentationRequest(updatePresentationRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Update presentation metadata (partial).

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
	id := "id_example" // string | Presentation id.
	updatePresentationRequest := *openapiclient.NewUpdatePresentationRequest() // UpdatePresentationRequest | 
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SlidesAPI.UpdatePresentation(context.Background(), id).UpdatePresentationRequest(updatePresentationRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SlidesAPI.UpdatePresentation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdatePresentation`: Presentation
	fmt.Fprintf(os.Stdout, "Response from `SlidesAPI.UpdatePresentation`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Presentation id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdatePresentationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updatePresentationRequest** | [**UpdatePresentationRequest**](UpdatePresentationRequest.md) |  | 
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**Presentation**](Presentation.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateSlide

> Slide UpdateSlide(ctx, id, slideId).UpdateSlideRequest(updateSlideRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Update a slide (partial).

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
	id := "id_example" // string | Presentation id.
	slideId := "slideId_example" // string | Slide id within the presentation.
	updateSlideRequest := *openapiclient.NewUpdateSlideRequest() // UpdateSlideRequest | 
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SlidesAPI.UpdateSlide(context.Background(), id, slideId).UpdateSlideRequest(updateSlideRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SlidesAPI.UpdateSlide``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateSlide`: Slide
	fmt.Fprintf(os.Stdout, "Response from `SlidesAPI.UpdateSlide`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Presentation id. | 
**slideId** | **string** | Slide id within the presentation. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateSlideRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **updateSlideRequest** | [**UpdateSlideRequest**](UpdateSlideRequest.md) |  | 
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**Slide**](Slide.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateSlideElement

> SlideElement UpdateSlideElement(ctx, id, slideId, elementId).UpdateSlideElementRequest(updateSlideElementRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Update a slide element (partial).

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
	id := "id_example" // string | Presentation id.
	slideId := "slideId_example" // string | Slide id within the presentation.
	elementId := "elementId_example" // string | Slide-element id.
	updateSlideElementRequest := *openapiclient.NewUpdateSlideElementRequest() // UpdateSlideElementRequest | 
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SlidesAPI.UpdateSlideElement(context.Background(), id, slideId, elementId).UpdateSlideElementRequest(updateSlideElementRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SlidesAPI.UpdateSlideElement``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateSlideElement`: SlideElement
	fmt.Fprintf(os.Stdout, "Response from `SlidesAPI.UpdateSlideElement`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Presentation id. | 
**slideId** | **string** | Slide id within the presentation. | 
**elementId** | **string** | Slide-element id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateSlideElementRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **updateSlideElementRequest** | [**UpdateSlideElementRequest**](UpdateSlideElementRequest.md) |  | 
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**SlideElement**](SlideElement.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

