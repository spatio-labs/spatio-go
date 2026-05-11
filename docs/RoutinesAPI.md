# \RoutinesAPI

All URIs are relative to *https://api.spatio.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ClaimRoutineRun**](RoutinesAPI.md#ClaimRoutineRun) | **Post** /v1/routines/runs/{id}/claim | Worker claims a queued run.
[**CompleteRoutineRun**](RoutinesAPI.md#CompleteRoutineRun) | **Post** /v1/routines/runs/{id}/complete | Worker marks a run complete.
[**CreateRoutine**](RoutinesAPI.md#CreateRoutine) | **Post** /v1/routines | Create a routine.
[**DeleteRoutine**](RoutinesAPI.md#DeleteRoutine) | **Delete** /v1/routines/{id} | Delete a routine.
[**GetRoutine**](RoutinesAPI.md#GetRoutine) | **Get** /v1/routines/{id} | Fetch a routine.
[**ListRoutineRuns**](RoutinesAPI.md#ListRoutineRuns) | **Get** /v1/routines/{id}/runs | List runs for a routine.
[**ListRoutines**](RoutinesAPI.md#ListRoutines) | **Get** /v1/routines | List routines for the caller&#39;s workspace.
[**RunRoutineNow**](RoutinesAPI.md#RunRoutineNow) | **Post** /v1/routines/{id}/run-now | Trigger an ad-hoc run.
[**UpdateRoutine**](RoutinesAPI.md#UpdateRoutine) | **Patch** /v1/routines/{id} | Update a routine.
[**UpdateRoutineRunProgress**](RoutinesAPI.md#UpdateRoutineRunProgress) | **Post** /v1/routines/runs/{id}/progress | Worker reports progress.



## ClaimRoutineRun

> RoutineRun ClaimRoutineRun(ctx, id).Execute()

Worker claims a queued run.

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
	resp, r, err := apiClient.RoutinesAPI.ClaimRoutineRun(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RoutinesAPI.ClaimRoutineRun``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ClaimRoutineRun`: RoutineRun
	fmt.Fprintf(os.Stdout, "Response from `RoutinesAPI.ClaimRoutineRun`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiClaimRoutineRunRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**RoutineRun**](RoutineRun.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CompleteRoutineRun

> RoutineRun CompleteRoutineRun(ctx, id).RoutineRunCompleteRequest(routineRunCompleteRequest).Execute()

Worker marks a run complete.

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
	routineRunCompleteRequest := *openapiclient.NewRoutineRunCompleteRequest() // RoutineRunCompleteRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RoutinesAPI.CompleteRoutineRun(context.Background(), id).RoutineRunCompleteRequest(routineRunCompleteRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RoutinesAPI.CompleteRoutineRun``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CompleteRoutineRun`: RoutineRun
	fmt.Fprintf(os.Stdout, "Response from `RoutinesAPI.CompleteRoutineRun`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCompleteRoutineRunRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **routineRunCompleteRequest** | [**RoutineRunCompleteRequest**](RoutineRunCompleteRequest.md) |  | 

### Return type

[**RoutineRun**](RoutineRun.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateRoutine

> Routine CreateRoutine(ctx).CreateRoutineRequest(createRoutineRequest).Execute()

Create a routine.

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
	createRoutineRequest := *openapiclient.NewCreateRoutineRequest("Name_example") // CreateRoutineRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RoutinesAPI.CreateRoutine(context.Background()).CreateRoutineRequest(createRoutineRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RoutinesAPI.CreateRoutine``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateRoutine`: Routine
	fmt.Fprintf(os.Stdout, "Response from `RoutinesAPI.CreateRoutine`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateRoutineRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createRoutineRequest** | [**CreateRoutineRequest**](CreateRoutineRequest.md) |  | 

### Return type

[**Routine**](Routine.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteRoutine

> DeleteRoutine(ctx, id).Execute()

Delete a routine.

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
	r, err := apiClient.RoutinesAPI.DeleteRoutine(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RoutinesAPI.DeleteRoutine``: %v\n", err)
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

Other parameters are passed through a pointer to a apiDeleteRoutineRequest struct via the builder pattern


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


## GetRoutine

> Routine GetRoutine(ctx, id).Execute()

Fetch a routine.

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
	resp, r, err := apiClient.RoutinesAPI.GetRoutine(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RoutinesAPI.GetRoutine``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetRoutine`: Routine
	fmt.Fprintf(os.Stdout, "Response from `RoutinesAPI.GetRoutine`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetRoutineRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**Routine**](Routine.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListRoutineRuns

> RoutineRunListResponse ListRoutineRuns(ctx, id).Execute()

List runs for a routine.

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
	resp, r, err := apiClient.RoutinesAPI.ListRoutineRuns(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RoutinesAPI.ListRoutineRuns``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListRoutineRuns`: RoutineRunListResponse
	fmt.Fprintf(os.Stdout, "Response from `RoutinesAPI.ListRoutineRuns`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListRoutineRunsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**RoutineRunListResponse**](RoutineRunListResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListRoutines

> RoutineListResponse ListRoutines(ctx).WorkspaceId(workspaceId).Status(status).Execute()

List routines for the caller's workspace.

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
	workspaceId := "workspaceId_example" // string |  (optional)
	status := "status_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RoutinesAPI.ListRoutines(context.Background()).WorkspaceId(workspaceId).Status(status).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RoutinesAPI.ListRoutines``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListRoutines`: RoutineListResponse
	fmt.Fprintf(os.Stdout, "Response from `RoutinesAPI.ListRoutines`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListRoutinesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspaceId** | **string** |  | 
 **status** | **string** |  | 

### Return type

[**RoutineListResponse**](RoutineListResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RunRoutineNow

> RoutineRun RunRoutineNow(ctx, id).Execute()

Trigger an ad-hoc run.

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
	resp, r, err := apiClient.RoutinesAPI.RunRoutineNow(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RoutinesAPI.RunRoutineNow``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RunRoutineNow`: RoutineRun
	fmt.Fprintf(os.Stdout, "Response from `RoutinesAPI.RunRoutineNow`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRunRoutineNowRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**RoutineRun**](RoutineRun.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateRoutine

> Routine UpdateRoutine(ctx, id).UpdateRoutineRequest(updateRoutineRequest).Execute()

Update a routine.

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
	updateRoutineRequest := *openapiclient.NewUpdateRoutineRequest() // UpdateRoutineRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RoutinesAPI.UpdateRoutine(context.Background(), id).UpdateRoutineRequest(updateRoutineRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RoutinesAPI.UpdateRoutine``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateRoutine`: Routine
	fmt.Fprintf(os.Stdout, "Response from `RoutinesAPI.UpdateRoutine`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateRoutineRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateRoutineRequest** | [**UpdateRoutineRequest**](UpdateRoutineRequest.md) |  | 

### Return type

[**Routine**](Routine.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateRoutineRunProgress

> RoutineRun UpdateRoutineRunProgress(ctx, id).RoutineRunProgressRequest(routineRunProgressRequest).Execute()

Worker reports progress.

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
	routineRunProgressRequest := *openapiclient.NewRoutineRunProgressRequest() // RoutineRunProgressRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RoutinesAPI.UpdateRoutineRunProgress(context.Background(), id).RoutineRunProgressRequest(routineRunProgressRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RoutinesAPI.UpdateRoutineRunProgress``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateRoutineRunProgress`: RoutineRun
	fmt.Fprintf(os.Stdout, "Response from `RoutinesAPI.UpdateRoutineRunProgress`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateRoutineRunProgressRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **routineRunProgressRequest** | [**RoutineRunProgressRequest**](RoutineRunProgressRequest.md) |  | 

### Return type

[**RoutineRun**](RoutineRun.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

