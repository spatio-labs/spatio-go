# \RealtimeAPI

All URIs are relative to *https://api.spatio.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**IssueCollaborationToken**](RealtimeAPI.md#IssueCollaborationToken) | **Post** /v1/realtime/collaboration-token | Exchange a bearer token for a short-lived Yjs collaboration JWT.



## IssueCollaborationToken

> IssueCollaborationToken200Response IssueCollaborationToken(ctx).IssueCollaborationTokenRequest(issueCollaborationTokenRequest).Execute()

Exchange a bearer token for a short-lived Yjs collaboration JWT.



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
	issueCollaborationTokenRequest := *openapiclient.NewIssueCollaborationTokenRequest() // IssueCollaborationTokenRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RealtimeAPI.IssueCollaborationToken(context.Background()).IssueCollaborationTokenRequest(issueCollaborationTokenRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RealtimeAPI.IssueCollaborationToken``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `IssueCollaborationToken`: IssueCollaborationToken200Response
	fmt.Fprintf(os.Stdout, "Response from `RealtimeAPI.IssueCollaborationToken`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiIssueCollaborationTokenRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **issueCollaborationTokenRequest** | [**IssueCollaborationTokenRequest**](IssueCollaborationTokenRequest.md) |  | 

### Return type

[**IssueCollaborationToken200Response**](IssueCollaborationToken200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

