# \MiscAPI

All URIs are relative to *https://api.spatio.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**DeletePinnedPlatform**](MiscAPI.md#DeletePinnedPlatform) | **Delete** /v1/pinned-platforms/{platformId} | Unpin a platform.
[**GetBootstrap**](MiscAPI.md#GetBootstrap) | **Get** /v1/bootstrap | Single-shot identity + config bundle the renderer hits on first load. Replaces the legacy server-side hydration in app/layout.tsx. 
[**GetOnboardingInvitations**](MiscAPI.md#GetOnboardingInvitations) | **Get** /v1/onboarding/invitations | Pending invitations the caller can accept during onboarding.
[**GetPinnedPlatforms**](MiscAPI.md#GetPinnedPlatforms) | **Get** /v1/pinned-platforms | Read the caller&#39;s pinned-platform list (sidebar order).
[**GetPlatformPreferences**](MiscAPI.md#GetPlatformPreferences) | **Get** /v1/platform-preferences | Read the caller&#39;s per-platform sidebar/visibility preferences.
[**GetPlatformSettingsLegacy**](MiscAPI.md#GetPlatformSettingsLegacy) | **Get** /v1/settings/platform | Legacy admin-tier platform settings read endpoint.
[**GetThreadsStatus**](MiscAPI.md#GetThreadsStatus) | **Get** /v1/threads/status | Async-thread / job-runner status snapshot.
[**GetUserPermissions**](MiscAPI.md#GetUserPermissions) | **Get** /v1/user/permissions | Read the caller&#39;s effective per-resource permissions.
[**GetWorkspaceActivity**](MiscAPI.md#GetWorkspaceActivity) | **Get** /v1/workspace-activity | Recent activity feed for a workspace.
[**GetWorkspaceLayout**](MiscAPI.md#GetWorkspaceLayout) | **Get** /v1/layout/{workspaceId} | Read the renderer&#39;s saved pane layout for a workspace.
[**PutPinnedPlatform**](MiscAPI.md#PutPinnedPlatform) | **Put** /v1/pinned-platforms | Pin a platform.
[**PutPlatformPreferences**](MiscAPI.md#PutPlatformPreferences) | **Put** /v1/platform-preferences | Replace the caller&#39;s platform preferences.
[**PutWorkspaceLayout**](MiscAPI.md#PutWorkspaceLayout) | **Put** /v1/layout/{workspaceId} | Save the renderer&#39;s pane layout.
[**ReorderPinnedPlatforms**](MiscAPI.md#ReorderPinnedPlatforms) | **Post** /v1/pinned-platforms/reorder | Reorder the pinned-platform list.
[**ResetPlatformPreferences**](MiscAPI.md#ResetPlatformPreferences) | **Post** /v1/platform-preferences/reset | Reset platform preferences to defaults.
[**UpdateUserProfile**](MiscAPI.md#UpdateUserProfile) | **Patch** /v1/user/profile | Update the caller&#39;s user profile (name, avatar, etc.).
[**ValidateOrganizationSlug**](MiscAPI.md#ValidateOrganizationSlug) | **Get** /v1/validate-slug/organization | Check whether an org slug is available.
[**ValidateWorkspaceSlug**](MiscAPI.md#ValidateWorkspaceSlug) | **Get** /v1/validate-slug/workspace | Check whether a workspace slug is available.



## DeletePinnedPlatform

> DeletePinnedPlatform(ctx, platformId).Execute()

Unpin a platform.

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
	platformId := "platformId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MiscAPI.DeletePinnedPlatform(context.Background(), platformId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MiscAPI.DeletePinnedPlatform``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**platformId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeletePinnedPlatformRequest struct via the builder pattern


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


## GetBootstrap

> map[string]interface{} GetBootstrap(ctx).Execute()

Single-shot identity + config bundle the renderer hits on first load. Replaces the legacy server-side hydration in app/layout.tsx. 

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
	resp, r, err := apiClient.MiscAPI.GetBootstrap(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MiscAPI.GetBootstrap``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetBootstrap`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MiscAPI.GetBootstrap`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetBootstrapRequest struct via the builder pattern


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


## GetOnboardingInvitations

> map[string]interface{} GetOnboardingInvitations(ctx).Execute()

Pending invitations the caller can accept during onboarding.

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
	resp, r, err := apiClient.MiscAPI.GetOnboardingInvitations(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MiscAPI.GetOnboardingInvitations``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetOnboardingInvitations`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MiscAPI.GetOnboardingInvitations`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetOnboardingInvitationsRequest struct via the builder pattern


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


## GetPinnedPlatforms

> map[string]interface{} GetPinnedPlatforms(ctx).Execute()

Read the caller's pinned-platform list (sidebar order).

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
	resp, r, err := apiClient.MiscAPI.GetPinnedPlatforms(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MiscAPI.GetPinnedPlatforms``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetPinnedPlatforms`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MiscAPI.GetPinnedPlatforms`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetPinnedPlatformsRequest struct via the builder pattern


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


## GetPlatformPreferences

> map[string]interface{} GetPlatformPreferences(ctx).Execute()

Read the caller's per-platform sidebar/visibility preferences.

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
	resp, r, err := apiClient.MiscAPI.GetPlatformPreferences(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MiscAPI.GetPlatformPreferences``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetPlatformPreferences`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MiscAPI.GetPlatformPreferences`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetPlatformPreferencesRequest struct via the builder pattern


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


## GetPlatformSettingsLegacy

> map[string]interface{} GetPlatformSettingsLegacy(ctx).Execute()

Legacy admin-tier platform settings read endpoint.

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
	resp, r, err := apiClient.MiscAPI.GetPlatformSettingsLegacy(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MiscAPI.GetPlatformSettingsLegacy``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetPlatformSettingsLegacy`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MiscAPI.GetPlatformSettingsLegacy`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetPlatformSettingsLegacyRequest struct via the builder pattern


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


## GetThreadsStatus

> map[string]interface{} GetThreadsStatus(ctx).Execute()

Async-thread / job-runner status snapshot.

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
	resp, r, err := apiClient.MiscAPI.GetThreadsStatus(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MiscAPI.GetThreadsStatus``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetThreadsStatus`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MiscAPI.GetThreadsStatus`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetThreadsStatusRequest struct via the builder pattern


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


## GetUserPermissions

> map[string]interface{} GetUserPermissions(ctx).Execute()

Read the caller's effective per-resource permissions.

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
	resp, r, err := apiClient.MiscAPI.GetUserPermissions(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MiscAPI.GetUserPermissions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetUserPermissions`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MiscAPI.GetUserPermissions`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetUserPermissionsRequest struct via the builder pattern


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


## GetWorkspaceActivity

> map[string]interface{} GetWorkspaceActivity(ctx).WorkspaceId(workspaceId).Limit(limit).Execute()

Recent activity feed for a workspace.

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
	limit := int32(56) // int32 |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MiscAPI.GetWorkspaceActivity(context.Background()).WorkspaceId(workspaceId).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MiscAPI.GetWorkspaceActivity``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetWorkspaceActivity`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MiscAPI.GetWorkspaceActivity`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetWorkspaceActivityRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspaceId** | **string** |  | 
 **limit** | **int32** |  | 

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


## GetWorkspaceLayout

> map[string]interface{} GetWorkspaceLayout(ctx, workspaceId).Execute()

Read the renderer's saved pane layout for a workspace.

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
	workspaceId := "workspaceId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MiscAPI.GetWorkspaceLayout(context.Background(), workspaceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MiscAPI.GetWorkspaceLayout``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetWorkspaceLayout`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MiscAPI.GetWorkspaceLayout`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**workspaceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetWorkspaceLayoutRequest struct via the builder pattern


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


## PutPinnedPlatform

> PutPinnedPlatform(ctx).RequestBody(requestBody).Execute()

Pin a platform.

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
	r, err := apiClient.MiscAPI.PutPinnedPlatform(context.Background()).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MiscAPI.PutPinnedPlatform``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiPutPinnedPlatformRequest struct via the builder pattern


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


## PutPlatformPreferences

> PutPlatformPreferences(ctx).RequestBody(requestBody).Execute()

Replace the caller's platform preferences.

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
	r, err := apiClient.MiscAPI.PutPlatformPreferences(context.Background()).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MiscAPI.PutPlatformPreferences``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiPutPlatformPreferencesRequest struct via the builder pattern


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


## PutWorkspaceLayout

> PutWorkspaceLayout(ctx, workspaceId).RequestBody(requestBody).Execute()

Save the renderer's pane layout.

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
	workspaceId := "workspaceId_example" // string | 
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MiscAPI.PutWorkspaceLayout(context.Background(), workspaceId).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MiscAPI.PutWorkspaceLayout``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**workspaceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPutWorkspaceLayoutRequest struct via the builder pattern


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


## ReorderPinnedPlatforms

> ReorderPinnedPlatforms(ctx).RequestBody(requestBody).Execute()

Reorder the pinned-platform list.

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
	r, err := apiClient.MiscAPI.ReorderPinnedPlatforms(context.Background()).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MiscAPI.ReorderPinnedPlatforms``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiReorderPinnedPlatformsRequest struct via the builder pattern


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


## ResetPlatformPreferences

> ResetPlatformPreferences(ctx).Execute()

Reset platform preferences to defaults.

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
	r, err := apiClient.MiscAPI.ResetPlatformPreferences(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MiscAPI.ResetPlatformPreferences``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiResetPlatformPreferencesRequest struct via the builder pattern


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


## UpdateUserProfile

> map[string]interface{} UpdateUserProfile(ctx).RequestBody(requestBody).Execute()

Update the caller's user profile (name, avatar, etc.).

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
	resp, r, err := apiClient.MiscAPI.UpdateUserProfile(context.Background()).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MiscAPI.UpdateUserProfile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateUserProfile`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MiscAPI.UpdateUserProfile`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiUpdateUserProfileRequest struct via the builder pattern


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


## ValidateOrganizationSlug

> map[string]interface{} ValidateOrganizationSlug(ctx).Slug(slug).Execute()

Check whether an org slug is available.

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
	slug := "slug_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MiscAPI.ValidateOrganizationSlug(context.Background()).Slug(slug).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MiscAPI.ValidateOrganizationSlug``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ValidateOrganizationSlug`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MiscAPI.ValidateOrganizationSlug`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiValidateOrganizationSlugRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **slug** | **string** |  | 

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


## ValidateWorkspaceSlug

> map[string]interface{} ValidateWorkspaceSlug(ctx).Slug(slug).OrganizationId(organizationId).Execute()

Check whether a workspace slug is available.

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
	slug := "slug_example" // string |  (optional)
	organizationId := "organizationId_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MiscAPI.ValidateWorkspaceSlug(context.Background()).Slug(slug).OrganizationId(organizationId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MiscAPI.ValidateWorkspaceSlug``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ValidateWorkspaceSlug`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MiscAPI.ValidateWorkspaceSlug`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiValidateWorkspaceSlugRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **slug** | **string** |  | 
 **organizationId** | **string** |  | 

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

