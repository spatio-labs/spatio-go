# \SheetsAPI

All URIs are relative to *https://api.spatio.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateSheet**](SheetsAPI.md#CreateSheet) | **Post** /v1/sheets | Create a sheet.
[**CreateSheetRow**](SheetsAPI.md#CreateSheetRow) | **Post** /v1/sheets/{id}/rows | Insert a row.
[**DeleteSheet**](SheetsAPI.md#DeleteSheet) | **Delete** /v1/sheets/{id} | Delete a sheet.
[**DeleteSheetRow**](SheetsAPI.md#DeleteSheetRow) | **Delete** /v1/sheets/{id}/rows/{rowIndex} | Delete a row.
[**GetSheet**](SheetsAPI.md#GetSheet) | **Get** /v1/sheets/{id} | Fetch one sheet.
[**ListSheetRows**](SheetsAPI.md#ListSheetRows) | **Get** /v1/sheets/{id}/rows | List rows in a sheet.
[**ListSheets**](SheetsAPI.md#ListSheets) | **Get** /v1/sheets | List sheets across connected accounts.
[**UpdateSheet**](SheetsAPI.md#UpdateSheet) | **Patch** /v1/sheets/{id} | Update a sheet (partial).
[**UpdateSheetCell**](SheetsAPI.md#UpdateSheetCell) | **Patch** /v1/sheets/{id}/rows/{rowIndex}/cells/{column} | Update a single cell.
[**UpdateSheetRow**](SheetsAPI.md#UpdateSheetRow) | **Patch** /v1/sheets/{id}/rows/{rowIndex} | Update a row (sparse).



## CreateSheet

> Sheet CreateSheet(ctx).CreateSheetRequest(createSheetRequest).AccountId(accountId).Provider(provider).XWorkspaceID(xWorkspaceID).Execute()

Create a sheet.



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
	createSheetRequest := *openapiclient.NewCreateSheetRequest("Name_example") // CreateSheetRequest | 
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	provider := "provider_example" // string | Provider id (e.g. `native-notes`, `notion`). Selects every connected account for the provider. Mutually exclusive with `accountId`.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SheetsAPI.CreateSheet(context.Background()).CreateSheetRequest(createSheetRequest).AccountId(accountId).Provider(provider).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SheetsAPI.CreateSheet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateSheet`: Sheet
	fmt.Fprintf(os.Stdout, "Response from `SheetsAPI.CreateSheet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateSheetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createSheetRequest** | [**CreateSheetRequest**](CreateSheetRequest.md) |  | 
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **provider** | **string** | Provider id (e.g. &#x60;native-notes&#x60;, &#x60;notion&#x60;). Selects every connected account for the provider. Mutually exclusive with &#x60;accountId&#x60;.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**Sheet**](Sheet.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateSheetRow

> Row CreateSheetRow(ctx, id).CreateRowRequest(createRowRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Insert a row.



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
	id := "id_example" // string | Sheet id.
	createRowRequest := *openapiclient.NewCreateRowRequest(map[string]interface{}{"key": interface{}(123)}) // CreateRowRequest | 
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SheetsAPI.CreateSheetRow(context.Background(), id).CreateRowRequest(createRowRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SheetsAPI.CreateSheetRow``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateSheetRow`: Row
	fmt.Fprintf(os.Stdout, "Response from `SheetsAPI.CreateSheetRow`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Sheet id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateSheetRowRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createRowRequest** | [**CreateRowRequest**](CreateRowRequest.md) |  | 
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**Row**](Row.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteSheet

> SuccessFlag DeleteSheet(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Delete a sheet.

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
	id := "id_example" // string | Sheet id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SheetsAPI.DeleteSheet(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SheetsAPI.DeleteSheet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteSheet`: SuccessFlag
	fmt.Fprintf(os.Stdout, "Response from `SheetsAPI.DeleteSheet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Sheet id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteSheetRequest struct via the builder pattern


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


## DeleteSheetRow

> SuccessFlag DeleteSheetRow(ctx, id, rowIndex).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Delete a row.

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
	id := "id_example" // string | Sheet id.
	rowIndex := int32(56) // int32 | Zero-based row index.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SheetsAPI.DeleteSheetRow(context.Background(), id, rowIndex).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SheetsAPI.DeleteSheetRow``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteSheetRow`: SuccessFlag
	fmt.Fprintf(os.Stdout, "Response from `SheetsAPI.DeleteSheetRow`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Sheet id. | 
**rowIndex** | **int32** | Zero-based row index. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteSheetRowRequest struct via the builder pattern


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


## GetSheet

> Sheet GetSheet(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Fetch one sheet.

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
	id := "id_example" // string | Sheet id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SheetsAPI.GetSheet(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SheetsAPI.GetSheet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetSheet`: Sheet
	fmt.Fprintf(os.Stdout, "Response from `SheetsAPI.GetSheet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Sheet id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetSheetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**Sheet**](Sheet.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListSheetRows

> RowList ListSheetRows(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Limit(limit).Offset(offset).Execute()

List rows in a sheet.



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
	id := "id_example" // string | Sheet id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)
	limit := int32(56) // int32 |  (optional) (default to 100)
	offset := int32(56) // int32 |  (optional) (default to 0)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SheetsAPI.ListSheetRows(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Limit(limit).Offset(offset).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SheetsAPI.ListSheetRows``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListSheetRows`: RowList
	fmt.Fprintf(os.Stdout, "Response from `SheetsAPI.ListSheetRows`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Sheet id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListSheetRowsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 
 **limit** | **int32** |  | [default to 100]
 **offset** | **int32** |  | [default to 0]

### Return type

[**RowList**](RowList.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListSheets

> SheetListEnvelope ListSheets(ctx).AccountId(accountId).Provider(provider).XWorkspaceID(xWorkspaceID).Limit(limit).Offset(offset).Execute()

List sheets across connected accounts.



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
	resp, r, err := apiClient.SheetsAPI.ListSheets(context.Background()).AccountId(accountId).Provider(provider).XWorkspaceID(xWorkspaceID).Limit(limit).Offset(offset).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SheetsAPI.ListSheets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListSheets`: SheetListEnvelope
	fmt.Fprintf(os.Stdout, "Response from `SheetsAPI.ListSheets`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListSheetsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **provider** | **string** | Provider id (e.g. &#x60;native-notes&#x60;, &#x60;notion&#x60;). Selects every connected account for the provider. Mutually exclusive with &#x60;accountId&#x60;.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 
 **limit** | **int32** |  | [default to 50]
 **offset** | **int32** |  | [default to 0]

### Return type

[**SheetListEnvelope**](SheetListEnvelope.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateSheet

> Sheet UpdateSheet(ctx, id).UpdateSheetRequest(updateSheetRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Update a sheet (partial).



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
	id := "id_example" // string | Sheet id.
	updateSheetRequest := *openapiclient.NewUpdateSheetRequest() // UpdateSheetRequest | 
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SheetsAPI.UpdateSheet(context.Background(), id).UpdateSheetRequest(updateSheetRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SheetsAPI.UpdateSheet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateSheet`: Sheet
	fmt.Fprintf(os.Stdout, "Response from `SheetsAPI.UpdateSheet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Sheet id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateSheetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateSheetRequest** | [**UpdateSheetRequest**](UpdateSheetRequest.md) |  | 
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**Sheet**](Sheet.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateSheetCell

> Cell UpdateSheetCell(ctx, id, rowIndex, column).UpdateCellRequest(updateCellRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Update a single cell.

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
	id := "id_example" // string | Sheet id.
	rowIndex := int32(56) // int32 | Zero-based row index.
	column := "column_example" // string | Column identifier. Provider-specific — usually a letter (`A`, `AB`) for spreadsheet providers or a column key string for structured providers. 
	updateCellRequest := *openapiclient.NewUpdateCellRequest(interface{}(123)) // UpdateCellRequest | 
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SheetsAPI.UpdateSheetCell(context.Background(), id, rowIndex, column).UpdateCellRequest(updateCellRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SheetsAPI.UpdateSheetCell``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateSheetCell`: Cell
	fmt.Fprintf(os.Stdout, "Response from `SheetsAPI.UpdateSheetCell`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Sheet id. | 
**rowIndex** | **int32** | Zero-based row index. | 
**column** | **string** | Column identifier. Provider-specific — usually a letter (&#x60;A&#x60;, &#x60;AB&#x60;) for spreadsheet providers or a column key string for structured providers.  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateSheetCellRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **updateCellRequest** | [**UpdateCellRequest**](UpdateCellRequest.md) |  | 
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**Cell**](Cell.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateSheetRow

> Row UpdateSheetRow(ctx, id, rowIndex).UpdateRowRequest(updateRowRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Update a row (sparse).



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
	id := "id_example" // string | Sheet id.
	rowIndex := int32(56) // int32 | Zero-based row index.
	updateRowRequest := *openapiclient.NewUpdateRowRequest(map[string]interface{}{"key": interface{}(123)}) // UpdateRowRequest | 
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SheetsAPI.UpdateSheetRow(context.Background(), id, rowIndex).UpdateRowRequest(updateRowRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SheetsAPI.UpdateSheetRow``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateSheetRow`: Row
	fmt.Fprintf(os.Stdout, "Response from `SheetsAPI.UpdateSheetRow`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Sheet id. | 
**rowIndex** | **int32** | Zero-based row index. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateSheetRowRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **updateRowRequest** | [**UpdateRowRequest**](UpdateRowRequest.md) |  | 
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**Row**](Row.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

