# \RecordsAPI

All URIs are relative to *https://api.spatio.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateRecord**](RecordsAPI.md#CreateRecord) | **Post** /v1/records | Create a record.
[**CreateRecordType**](RecordsAPI.md#CreateRecordType) | **Post** /v1/records/types | Create a record type (org-scoped).
[**DeleteRecord**](RecordsAPI.md#DeleteRecord) | **Delete** /v1/records/{id} | Delete a record.
[**GetRecord**](RecordsAPI.md#GetRecord) | **Get** /v1/records/{id} | Fetch a record.
[**ListRecordTypes**](RecordsAPI.md#ListRecordTypes) | **Get** /v1/records/types | List record types for an organization.
[**ListRecords**](RecordsAPI.md#ListRecords) | **Get** /v1/records | List records for an organization. &#x60;organization_id&#x60; query param is required (handler returns 400 otherwise). 
[**UpdateRecord**](RecordsAPI.md#UpdateRecord) | **Patch** /v1/records/{id} | Update a record.
[**UpdateRecordType**](RecordsAPI.md#UpdateRecordType) | **Patch** /v1/records/types/{id} | Update a record type.



## CreateRecord

> Record CreateRecord(ctx).CreateRecordRequest(createRecordRequest).Execute()

Create a record.

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
	createRecordRequest := *openapiclient.NewCreateRecordRequest("RecordTypeId_example") // CreateRecordRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RecordsAPI.CreateRecord(context.Background()).CreateRecordRequest(createRecordRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RecordsAPI.CreateRecord``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateRecord`: Record
	fmt.Fprintf(os.Stdout, "Response from `RecordsAPI.CreateRecord`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateRecordRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createRecordRequest** | [**CreateRecordRequest**](CreateRecordRequest.md) |  | 

### Return type

[**Record**](Record.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateRecordType

> RecordType CreateRecordType(ctx).CreateRecordTypeRequest(createRecordTypeRequest).Execute()

Create a record type (org-scoped).

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
	createRecordTypeRequest := *openapiclient.NewCreateRecordTypeRequest("Name_example") // CreateRecordTypeRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RecordsAPI.CreateRecordType(context.Background()).CreateRecordTypeRequest(createRecordTypeRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RecordsAPI.CreateRecordType``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateRecordType`: RecordType
	fmt.Fprintf(os.Stdout, "Response from `RecordsAPI.CreateRecordType`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateRecordTypeRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createRecordTypeRequest** | [**CreateRecordTypeRequest**](CreateRecordTypeRequest.md) |  | 

### Return type

[**RecordType**](RecordType.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteRecord

> DeleteRecord(ctx, id).Execute()

Delete a record.

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
	r, err := apiClient.RecordsAPI.DeleteRecord(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RecordsAPI.DeleteRecord``: %v\n", err)
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

Other parameters are passed through a pointer to a apiDeleteRecordRequest struct via the builder pattern


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


## GetRecord

> Record GetRecord(ctx, id).Execute()

Fetch a record.

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
	resp, r, err := apiClient.RecordsAPI.GetRecord(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RecordsAPI.GetRecord``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetRecord`: Record
	fmt.Fprintf(os.Stdout, "Response from `RecordsAPI.GetRecord`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetRecordRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**Record**](Record.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListRecordTypes

> RecordTypeListResponse ListRecordTypes(ctx).OrganizationId(organizationId).Execute()

List record types for an organization.

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
	organizationId := "organizationId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RecordsAPI.ListRecordTypes(context.Background()).OrganizationId(organizationId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RecordsAPI.ListRecordTypes``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListRecordTypes`: RecordTypeListResponse
	fmt.Fprintf(os.Stdout, "Response from `RecordsAPI.ListRecordTypes`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListRecordTypesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **organizationId** | **string** |  | 

### Return type

[**RecordTypeListResponse**](RecordTypeListResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListRecords

> RecordListResponse ListRecords(ctx).OrganizationId(organizationId).RecordTypeId(recordTypeId).Limit(limit).Execute()

List records for an organization. `organization_id` query param is required (handler returns 400 otherwise). 

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
	organizationId := "organizationId_example" // string | 
	recordTypeId := "recordTypeId_example" // string |  (optional)
	limit := int32(56) // int32 |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RecordsAPI.ListRecords(context.Background()).OrganizationId(organizationId).RecordTypeId(recordTypeId).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RecordsAPI.ListRecords``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListRecords`: RecordListResponse
	fmt.Fprintf(os.Stdout, "Response from `RecordsAPI.ListRecords`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListRecordsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **organizationId** | **string** |  | 
 **recordTypeId** | **string** |  | 
 **limit** | **int32** |  | 

### Return type

[**RecordListResponse**](RecordListResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateRecord

> Record UpdateRecord(ctx, id).UpdateRecordRequest(updateRecordRequest).Execute()

Update a record.

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
	updateRecordRequest := *openapiclient.NewUpdateRecordRequest() // UpdateRecordRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RecordsAPI.UpdateRecord(context.Background(), id).UpdateRecordRequest(updateRecordRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RecordsAPI.UpdateRecord``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateRecord`: Record
	fmt.Fprintf(os.Stdout, "Response from `RecordsAPI.UpdateRecord`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateRecordRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateRecordRequest** | [**UpdateRecordRequest**](UpdateRecordRequest.md) |  | 

### Return type

[**Record**](Record.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateRecordType

> RecordType UpdateRecordType(ctx, id).UpdateRecordTypeRequest(updateRecordTypeRequest).Execute()

Update a record type.

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
	updateRecordTypeRequest := *openapiclient.NewUpdateRecordTypeRequest() // UpdateRecordTypeRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RecordsAPI.UpdateRecordType(context.Background(), id).UpdateRecordTypeRequest(updateRecordTypeRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RecordsAPI.UpdateRecordType``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateRecordType`: RecordType
	fmt.Fprintf(os.Stdout, "Response from `RecordsAPI.UpdateRecordType`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateRecordTypeRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateRecordTypeRequest** | [**UpdateRecordTypeRequest**](UpdateRecordTypeRequest.md) |  | 

### Return type

[**RecordType**](RecordType.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

