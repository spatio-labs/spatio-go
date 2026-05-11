# \OrganizationsAPI

All URIs are relative to *https://api.spatio.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AcceptOrganizationInvitation**](OrganizationsAPI.md#AcceptOrganizationInvitation) | **Post** /v1/organizations/{org}/accept-invitation | Accept an invitation to this organization.
[**AddOrganizationMember**](OrganizationsAPI.md#AddOrganizationMember) | **Post** /v1/organizations/{org}/members | Add a member directly (skips invitation flow).
[**CreateOrganization**](OrganizationsAPI.md#CreateOrganization) | **Post** /v1/organizations | Create an organization.
[**CreateOrganizationConcept**](OrganizationsAPI.md#CreateOrganizationConcept) | **Post** /v1/organizations/{org}/concepts | Create an org-brain concept (admin+ only).
[**CreateOrganizationCustomRole**](OrganizationsAPI.md#CreateOrganizationCustomRole) | **Post** /v1/organizations/{org}/roles | Create a custom role (admin+ only).
[**CreateOrganizationInvitation**](OrganizationsAPI.md#CreateOrganizationInvitation) | **Post** /v1/organizations/{org}/invitations | Invite a user to the organization.
[**CreateOrganizationWorkspace**](OrganizationsAPI.md#CreateOrganizationWorkspace) | **Post** /v1/organizations/{org}/workspaces | Create a workspace inside an organization.
[**DeleteOrganization**](OrganizationsAPI.md#DeleteOrganization) | **Delete** /v1/organizations/{org} | Delete an organization.
[**DeleteOrganizationConcept**](OrganizationsAPI.md#DeleteOrganizationConcept) | **Delete** /v1/organizations/{org}/concepts/{slug} | Delete a concept (admin+ only).
[**DeleteOrganizationCustomRole**](OrganizationsAPI.md#DeleteOrganizationCustomRole) | **Delete** /v1/organizations/{org}/roles/{roleId} | Delete a custom role (admin+ only).
[**DeleteOrganizationLogo**](OrganizationsAPI.md#DeleteOrganizationLogo) | **Delete** /v1/organizations/{org}/logo | Delete the organization logo.
[**GetOrganization**](OrganizationsAPI.md#GetOrganization) | **Get** /v1/organizations/{org} | Fetch a single organization.
[**GetOrganizationConcept**](OrganizationsAPI.md#GetOrganizationConcept) | **Get** /v1/organizations/{org}/concepts/{slug} | Fetch a concept.
[**ListMyOrganizations**](OrganizationsAPI.md#ListMyOrganizations) | **Get** /v1/organizations | List the caller&#39;s organizations.
[**ListOrganizationAuditLog**](OrganizationsAPI.md#ListOrganizationAuditLog) | **Get** /v1/organizations/{org}/audit-log | Read the organization audit log (admin / billing-admin only).
[**ListOrganizationConcepts**](OrganizationsAPI.md#ListOrganizationConcepts) | **Get** /v1/organizations/{org}/concepts | List org-brain concepts (curated knowledge surfaced to agents).
[**ListOrganizationCustomRoles**](OrganizationsAPI.md#ListOrganizationCustomRoles) | **Get** /v1/organizations/{org}/roles | List custom roles defined on the organization.
[**ListOrganizationInvitations**](OrganizationsAPI.md#ListOrganizationInvitations) | **Get** /v1/organizations/{org}/invitations | List pending invitations for an organization.
[**ListOrganizationMembers**](OrganizationsAPI.md#ListOrganizationMembers) | **Get** /v1/organizations/{org}/members | List members of an organization.
[**ListOrganizationWorkspaces**](OrganizationsAPI.md#ListOrganizationWorkspaces) | **Get** /v1/organizations/{org}/workspaces | List workspaces in an organization.
[**RemoveOrganizationMember**](OrganizationsAPI.md#RemoveOrganizationMember) | **Delete** /v1/organizations/{org}/members/{memberId} | Remove a member from the organization.
[**ResendOrganizationInvitation**](OrganizationsAPI.md#ResendOrganizationInvitation) | **Post** /v1/organizations/{org}/invitations/{invitationId}/resend | Revoke and reissue an invitation with a fresh token.
[**RevokeOrganizationInvitation**](OrganizationsAPI.md#RevokeOrganizationInvitation) | **Delete** /v1/organizations/{org}/invitations/{invitationId} | Revoke a pending invitation.
[**UpdateOrganization**](OrganizationsAPI.md#UpdateOrganization) | **Patch** /v1/organizations/{org} | Update organization metadata.
[**UpdateOrganizationConcept**](OrganizationsAPI.md#UpdateOrganizationConcept) | **Patch** /v1/organizations/{org}/concepts/{slug} | Update a concept (admin+ only).
[**UpdateOrganizationCustomRole**](OrganizationsAPI.md#UpdateOrganizationCustomRole) | **Patch** /v1/organizations/{org}/roles/{roleId} | Update a custom role (admin+ only).
[**UpdateOrganizationMember**](OrganizationsAPI.md#UpdateOrganizationMember) | **Patch** /v1/organizations/{org}/members/{memberId} | Update a member&#39;s role.
[**UploadOrganizationLogo**](OrganizationsAPI.md#UploadOrganizationLogo) | **Post** /v1/organizations/{org}/logo | Upload (or replace) the organization logo. Multipart.



## AcceptOrganizationInvitation

> map[string]interface{} AcceptOrganizationInvitation(ctx, org).AcceptOrganizationInvitationRequest(acceptOrganizationInvitationRequest).Execute()

Accept an invitation to this organization.

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
	acceptOrganizationInvitationRequest := *openapiclient.NewAcceptOrganizationInvitationRequest("Token_example") // AcceptOrganizationInvitationRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OrganizationsAPI.AcceptOrganizationInvitation(context.Background(), org).AcceptOrganizationInvitationRequest(acceptOrganizationInvitationRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.AcceptOrganizationInvitation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AcceptOrganizationInvitation`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `OrganizationsAPI.AcceptOrganizationInvitation`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiAcceptOrganizationInvitationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **acceptOrganizationInvitationRequest** | [**AcceptOrganizationInvitationRequest**](AcceptOrganizationInvitationRequest.md) |  | 

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


## AddOrganizationMember

> map[string]interface{} AddOrganizationMember(ctx, org).AddOrganizationMemberRequest(addOrganizationMemberRequest).Execute()

Add a member directly (skips invitation flow).

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
	addOrganizationMemberRequest := *openapiclient.NewAddOrganizationMemberRequest("Email_example") // AddOrganizationMemberRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OrganizationsAPI.AddOrganizationMember(context.Background(), org).AddOrganizationMemberRequest(addOrganizationMemberRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.AddOrganizationMember``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AddOrganizationMember`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `OrganizationsAPI.AddOrganizationMember`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiAddOrganizationMemberRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **addOrganizationMemberRequest** | [**AddOrganizationMemberRequest**](AddOrganizationMemberRequest.md) |  | 

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


## CreateOrganization

> map[string]interface{} CreateOrganization(ctx).CreateOrganizationRequest(createOrganizationRequest).Execute()

Create an organization.

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
	createOrganizationRequest := *openapiclient.NewCreateOrganizationRequest("Name_example") // CreateOrganizationRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OrganizationsAPI.CreateOrganization(context.Background()).CreateOrganizationRequest(createOrganizationRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.CreateOrganization``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateOrganization`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `OrganizationsAPI.CreateOrganization`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateOrganizationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createOrganizationRequest** | [**CreateOrganizationRequest**](CreateOrganizationRequest.md) |  | 

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


## CreateOrganizationConcept

> map[string]interface{} CreateOrganizationConcept(ctx, org).RequestBody(requestBody).Execute()

Create an org-brain concept (admin+ only).

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
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OrganizationsAPI.CreateOrganizationConcept(context.Background(), org).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.CreateOrganizationConcept``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateOrganizationConcept`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `OrganizationsAPI.CreateOrganizationConcept`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateOrganizationConceptRequest struct via the builder pattern


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


## CreateOrganizationCustomRole

> map[string]interface{} CreateOrganizationCustomRole(ctx, org).RequestBody(requestBody).Execute()

Create a custom role (admin+ only).

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
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OrganizationsAPI.CreateOrganizationCustomRole(context.Background(), org).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.CreateOrganizationCustomRole``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateOrganizationCustomRole`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `OrganizationsAPI.CreateOrganizationCustomRole`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateOrganizationCustomRoleRequest struct via the builder pattern


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


## CreateOrganizationInvitation

> OrganizationInvitation CreateOrganizationInvitation(ctx, org).CreateOrganizationInvitationRequest(createOrganizationInvitationRequest).Execute()

Invite a user to the organization.



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
	createOrganizationInvitationRequest := *openapiclient.NewCreateOrganizationInvitationRequest("Email_example", "Role_example") // CreateOrganizationInvitationRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OrganizationsAPI.CreateOrganizationInvitation(context.Background(), org).CreateOrganizationInvitationRequest(createOrganizationInvitationRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.CreateOrganizationInvitation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateOrganizationInvitation`: OrganizationInvitation
	fmt.Fprintf(os.Stdout, "Response from `OrganizationsAPI.CreateOrganizationInvitation`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateOrganizationInvitationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createOrganizationInvitationRequest** | [**CreateOrganizationInvitationRequest**](CreateOrganizationInvitationRequest.md) |  | 

### Return type

[**OrganizationInvitation**](OrganizationInvitation.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateOrganizationWorkspace

> WorkspaceEnvelope CreateOrganizationWorkspace(ctx, org).CreateWorkspaceRequest(createWorkspaceRequest).Execute()

Create a workspace inside an organization.



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
	createWorkspaceRequest := *openapiclient.NewCreateWorkspaceRequest("Name_example") // CreateWorkspaceRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OrganizationsAPI.CreateOrganizationWorkspace(context.Background(), org).CreateWorkspaceRequest(createWorkspaceRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.CreateOrganizationWorkspace``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateOrganizationWorkspace`: WorkspaceEnvelope
	fmt.Fprintf(os.Stdout, "Response from `OrganizationsAPI.CreateOrganizationWorkspace`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateOrganizationWorkspaceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createWorkspaceRequest** | [**CreateWorkspaceRequest**](CreateWorkspaceRequest.md) |  | 

### Return type

[**WorkspaceEnvelope**](WorkspaceEnvelope.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteOrganization

> DeleteOrganization(ctx, org).Execute()

Delete an organization.

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
	org := "org_example" // string | Organization id or slug.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.OrganizationsAPI.DeleteOrganization(context.Background(), org).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.DeleteOrganization``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** | Organization id or slug. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteOrganizationRequest struct via the builder pattern


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


## DeleteOrganizationConcept

> DeleteOrganizationConcept(ctx, org, slug).Execute()

Delete a concept (admin+ only).

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
	slug := "slug_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.OrganizationsAPI.DeleteOrganizationConcept(context.Background(), org, slug).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.DeleteOrganizationConcept``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**slug** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteOrganizationConceptRequest struct via the builder pattern


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


## DeleteOrganizationCustomRole

> DeleteOrganizationCustomRole(ctx, org, roleId).Execute()

Delete a custom role (admin+ only).

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
	roleId := "roleId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.OrganizationsAPI.DeleteOrganizationCustomRole(context.Background(), org, roleId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.DeleteOrganizationCustomRole``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**roleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteOrganizationCustomRoleRequest struct via the builder pattern


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


## DeleteOrganizationLogo

> DeleteOrganizationLogo(ctx, org).Execute()

Delete the organization logo.

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.OrganizationsAPI.DeleteOrganizationLogo(context.Background(), org).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.DeleteOrganizationLogo``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteOrganizationLogoRequest struct via the builder pattern


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


## GetOrganization

> OrganizationDetailLegacy GetOrganization(ctx, org).Execute()

Fetch a single organization.



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
	org := "org_example" // string | Organization id or slug.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OrganizationsAPI.GetOrganization(context.Background(), org).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.GetOrganization``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetOrganization`: OrganizationDetailLegacy
	fmt.Fprintf(os.Stdout, "Response from `OrganizationsAPI.GetOrganization`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** | Organization id or slug. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetOrganizationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**OrganizationDetailLegacy**](OrganizationDetailLegacy.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetOrganizationConcept

> map[string]interface{} GetOrganizationConcept(ctx, org, slug).Execute()

Fetch a concept.

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
	slug := "slug_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OrganizationsAPI.GetOrganizationConcept(context.Background(), org, slug).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.GetOrganizationConcept``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetOrganizationConcept`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `OrganizationsAPI.GetOrganizationConcept`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**slug** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetOrganizationConceptRequest struct via the builder pattern


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


## ListMyOrganizations

> OrganizationListResponse ListMyOrganizations(ctx).Execute()

List the caller's organizations.

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
	resp, r, err := apiClient.OrganizationsAPI.ListMyOrganizations(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.ListMyOrganizations``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListMyOrganizations`: OrganizationListResponse
	fmt.Fprintf(os.Stdout, "Response from `OrganizationsAPI.ListMyOrganizations`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListMyOrganizationsRequest struct via the builder pattern


### Return type

[**OrganizationListResponse**](OrganizationListResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListOrganizationAuditLog

> map[string]interface{} ListOrganizationAuditLog(ctx, org).Limit(limit).Cursor(cursor).Execute()

Read the organization audit log (admin / billing-admin only).

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
	limit := int32(56) // int32 |  (optional)
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OrganizationsAPI.ListOrganizationAuditLog(context.Background(), org).Limit(limit).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.ListOrganizationAuditLog``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListOrganizationAuditLog`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `OrganizationsAPI.ListOrganizationAuditLog`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListOrganizationAuditLogRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **limit** | **int32** |  | 
 **cursor** | **string** |  | 

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


## ListOrganizationConcepts

> map[string]interface{} ListOrganizationConcepts(ctx, org).Execute()

List org-brain concepts (curated knowledge surfaced to agents).

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OrganizationsAPI.ListOrganizationConcepts(context.Background(), org).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.ListOrganizationConcepts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListOrganizationConcepts`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `OrganizationsAPI.ListOrganizationConcepts`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListOrganizationConceptsRequest struct via the builder pattern


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


## ListOrganizationCustomRoles

> map[string]interface{} ListOrganizationCustomRoles(ctx, org).Execute()

List custom roles defined on the organization.

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OrganizationsAPI.ListOrganizationCustomRoles(context.Background(), org).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.ListOrganizationCustomRoles``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListOrganizationCustomRoles`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `OrganizationsAPI.ListOrganizationCustomRoles`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListOrganizationCustomRolesRequest struct via the builder pattern


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


## ListOrganizationInvitations

> OrganizationInvitationListResponse ListOrganizationInvitations(ctx, org).Execute()

List pending invitations for an organization.

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OrganizationsAPI.ListOrganizationInvitations(context.Background(), org).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.ListOrganizationInvitations``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListOrganizationInvitations`: OrganizationInvitationListResponse
	fmt.Fprintf(os.Stdout, "Response from `OrganizationsAPI.ListOrganizationInvitations`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListOrganizationInvitationsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**OrganizationInvitationListResponse**](OrganizationInvitationListResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListOrganizationMembers

> OrganizationMemberListResponse ListOrganizationMembers(ctx, org).Execute()

List members of an organization.

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OrganizationsAPI.ListOrganizationMembers(context.Background(), org).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.ListOrganizationMembers``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListOrganizationMembers`: OrganizationMemberListResponse
	fmt.Fprintf(os.Stdout, "Response from `OrganizationsAPI.ListOrganizationMembers`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListOrganizationMembersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**OrganizationMemberListResponse**](OrganizationMemberListResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListOrganizationWorkspaces

> WorkspaceListResponse ListOrganizationWorkspaces(ctx, org).Execute()

List workspaces in an organization.

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OrganizationsAPI.ListOrganizationWorkspaces(context.Background(), org).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.ListOrganizationWorkspaces``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListOrganizationWorkspaces`: WorkspaceListResponse
	fmt.Fprintf(os.Stdout, "Response from `OrganizationsAPI.ListOrganizationWorkspaces`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListOrganizationWorkspacesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**WorkspaceListResponse**](WorkspaceListResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RemoveOrganizationMember

> RemoveOrganizationMember(ctx, org, memberId).Execute()

Remove a member from the organization.

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
	memberId := "memberId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.OrganizationsAPI.RemoveOrganizationMember(context.Background(), org, memberId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.RemoveOrganizationMember``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**memberId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRemoveOrganizationMemberRequest struct via the builder pattern


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


## ResendOrganizationInvitation

> OrganizationInvitation ResendOrganizationInvitation(ctx, org, invitationId).Execute()

Revoke and reissue an invitation with a fresh token.

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
	invitationId := "invitationId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OrganizationsAPI.ResendOrganizationInvitation(context.Background(), org, invitationId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.ResendOrganizationInvitation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ResendOrganizationInvitation`: OrganizationInvitation
	fmt.Fprintf(os.Stdout, "Response from `OrganizationsAPI.ResendOrganizationInvitation`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**invitationId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiResendOrganizationInvitationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**OrganizationInvitation**](OrganizationInvitation.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RevokeOrganizationInvitation

> RevokeOrganizationInvitation(ctx, org, invitationId).Execute()

Revoke a pending invitation.

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
	invitationId := "invitationId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.OrganizationsAPI.RevokeOrganizationInvitation(context.Background(), org, invitationId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.RevokeOrganizationInvitation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**invitationId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRevokeOrganizationInvitationRequest struct via the builder pattern


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


## UpdateOrganization

> map[string]interface{} UpdateOrganization(ctx, org).UpdateOrganizationRequest(updateOrganizationRequest).Execute()

Update organization metadata.

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
	org := "org_example" // string | Organization id or slug.
	updateOrganizationRequest := *openapiclient.NewUpdateOrganizationRequest() // UpdateOrganizationRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OrganizationsAPI.UpdateOrganization(context.Background(), org).UpdateOrganizationRequest(updateOrganizationRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.UpdateOrganization``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateOrganization`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `OrganizationsAPI.UpdateOrganization`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** | Organization id or slug. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateOrganizationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateOrganizationRequest** | [**UpdateOrganizationRequest**](UpdateOrganizationRequest.md) |  | 

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


## UpdateOrganizationConcept

> map[string]interface{} UpdateOrganizationConcept(ctx, org, slug).RequestBody(requestBody).Execute()

Update a concept (admin+ only).

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
	slug := "slug_example" // string | 
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OrganizationsAPI.UpdateOrganizationConcept(context.Background(), org, slug).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.UpdateOrganizationConcept``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateOrganizationConcept`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `OrganizationsAPI.UpdateOrganizationConcept`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**slug** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateOrganizationConceptRequest struct via the builder pattern


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


## UpdateOrganizationCustomRole

> map[string]interface{} UpdateOrganizationCustomRole(ctx, org, roleId).RequestBody(requestBody).Execute()

Update a custom role (admin+ only).

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
	roleId := "roleId_example" // string | 
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OrganizationsAPI.UpdateOrganizationCustomRole(context.Background(), org, roleId).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.UpdateOrganizationCustomRole``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateOrganizationCustomRole`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `OrganizationsAPI.UpdateOrganizationCustomRole`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**roleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateOrganizationCustomRoleRequest struct via the builder pattern


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


## UpdateOrganizationMember

> map[string]interface{} UpdateOrganizationMember(ctx, org, memberId).UpdateOrganizationMemberRequest(updateOrganizationMemberRequest).Execute()

Update a member's role.

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
	memberId := "memberId_example" // string | 
	updateOrganizationMemberRequest := *openapiclient.NewUpdateOrganizationMemberRequest("Role_example") // UpdateOrganizationMemberRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OrganizationsAPI.UpdateOrganizationMember(context.Background(), org, memberId).UpdateOrganizationMemberRequest(updateOrganizationMemberRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.UpdateOrganizationMember``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateOrganizationMember`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `OrganizationsAPI.UpdateOrganizationMember`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**memberId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateOrganizationMemberRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **updateOrganizationMemberRequest** | [**UpdateOrganizationMemberRequest**](UpdateOrganizationMemberRequest.md) |  | 

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


## UploadOrganizationLogo

> map[string]interface{} UploadOrganizationLogo(ctx, org).File(file).Execute()

Upload (or replace) the organization logo. Multipart.

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
	file := os.NewFile(1234, "some_file") // *os.File |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OrganizationsAPI.UploadOrganizationLogo(context.Background(), org).File(file).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OrganizationsAPI.UploadOrganizationLogo``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UploadOrganizationLogo`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `OrganizationsAPI.UploadOrganizationLogo`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUploadOrganizationLogoRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **file** | ***os.File** |  | 

### Return type

**map[string]interface{}**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

