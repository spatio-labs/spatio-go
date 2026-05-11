# \SearchAPI

All URIs are relative to *https://api.spatio.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**FederatedSearch**](SearchAPI.md#FederatedSearch) | **Post** /v1/search | Cross-platform federated search.



## FederatedSearch

> FederatedSearch200Response FederatedSearch(ctx).FederatedSearchRequest(federatedSearchRequest).Execute()

Cross-platform federated search.



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
	federatedSearchRequest := *openapiclient.NewFederatedSearchRequest("Query_example") // FederatedSearchRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SearchAPI.FederatedSearch(context.Background()).FederatedSearchRequest(federatedSearchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SearchAPI.FederatedSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FederatedSearch`: FederatedSearch200Response
	fmt.Fprintf(os.Stdout, "Response from `SearchAPI.FederatedSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiFederatedSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **federatedSearchRequest** | [**FederatedSearchRequest**](FederatedSearchRequest.md) |  | 

### Return type

[**FederatedSearch200Response**](FederatedSearch200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

