# \MailAPI

All URIs are relative to *https://api.spatio.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**BulkArchiveEmails**](MailAPI.md#BulkArchiveEmails) | **Post** /v1/mail/archive | Archive multiple messages (remove the INBOX label).
[**BulkDeleteEmails**](MailAPI.md#BulkDeleteEmails) | **Post** /v1/mail/delete | Delete multiple messages in one call.
[**BulkMarkEmailsRead**](MailAPI.md#BulkMarkEmailsRead) | **Post** /v1/mail/mark-read | Mark multiple messages read or unread in one call.
[**CreateDraft**](MailAPI.md#CreateDraft) | **Post** /v1/mail/drafts | Create a draft.
[**CreateEmailLabel**](MailAPI.md#CreateEmailLabel) | **Post** /v1/mail/labels | Create a label.
[**CreateMailTemplate**](MailAPI.md#CreateMailTemplate) | **Post** /v1/mail/templates | Create a mail template.
[**DeleteDraft**](MailAPI.md#DeleteDraft) | **Delete** /v1/mail/drafts/{id} | Delete a draft.
[**DeleteEmail**](MailAPI.md#DeleteEmail) | **Delete** /v1/mail/email/{id} | Delete an email.
[**DeleteEmailLabel**](MailAPI.md#DeleteEmailLabel) | **Delete** /v1/mail/labels/{id} | Delete a label.
[**DeleteMailTemplate**](MailAPI.md#DeleteMailTemplate) | **Delete** /v1/mail/templates/{id} | Delete a mail template.
[**GetEmail**](MailAPI.md#GetEmail) | **Get** /v1/mail/email/{id} | Fetch one email.
[**GetEmailAttachment**](MailAPI.md#GetEmailAttachment) | **Get** /v1/mail/attachment/{messageId}/{attachmentId} | Download an attachment.
[**GetEmailThread**](MailAPI.md#GetEmailThread) | **Get** /v1/mail/thread/{id} | Fetch a thread (the conversation a message belongs to).
[**GetMailTemplate**](MailAPI.md#GetMailTemplate) | **Get** /v1/mail/templates/{id} | Fetch a mail template.
[**GetMailThreadTracking**](MailAPI.md#GetMailThreadTracking) | **Get** /v1/mail/threads/{threadId}/tracking | Read mail-tracking events for a thread (open log, reply log, etc.).
[**InstantiateMailTemplate**](MailAPI.md#InstantiateMailTemplate) | **Post** /v1/mail/templates/{id}/instantiate | Render a template with variables and return the resulting draft.
[**ListDrafts**](MailAPI.md#ListDrafts) | **Get** /v1/mail/drafts | List drafts across connected mail accounts.
[**ListEmailLabels**](MailAPI.md#ListEmailLabels) | **Get** /v1/mail/labels | List labels on the resolved mail account.
[**ListEmails**](MailAPI.md#ListEmails) | **Get** /v1/mail/list | List emails across connected mail accounts.
[**ListMailTemplates**](MailAPI.md#ListMailTemplates) | **Get** /v1/mail/templates | List the caller&#39;s saved mail templates.
[**ReplyEmail**](MailAPI.md#ReplyEmail) | **Post** /v1/mail/reply | Reply to a specific email.
[**SaveMailTemplate**](MailAPI.md#SaveMailTemplate) | **Post** /v1/mail/templates/save | Save-or-create endpoint used by the renderer&#39;s \&quot;save as template\&quot; flow. Distinct from POST /v1/mail/templates which is the strict create. 
[**SearchEmails**](MailAPI.md#SearchEmails) | **Get** /v1/mail/search | Structured search across connected mail accounts.
[**SendDraft**](MailAPI.md#SendDraft) | **Post** /v1/mail/drafts/{id}/send | Send a draft.
[**SendEmail**](MailAPI.md#SendEmail) | **Post** /v1/mail/send | Send an email.
[**UpdateDraft**](MailAPI.md#UpdateDraft) | **Put** /v1/mail/drafts/{id} | Update a draft (full replacement of provided fields).
[**UpdateEmail**](MailAPI.md#UpdateEmail) | **Patch** /v1/mail/email/{id} | Update an email (mark read/star, add/remove labels).
[**UpdateMailTemplate**](MailAPI.md#UpdateMailTemplate) | **Patch** /v1/mail/templates/{id} | Update a mail template.
[**WorkspaceAddMailMessageLabels**](MailAPI.md#WorkspaceAddMailMessageLabels) | **Post** /v1/organizations/{org}/workspaces/{workspace}/mail/{messageId}/labels | 
[**WorkspaceCreateMailDraft**](MailAPI.md#WorkspaceCreateMailDraft) | **Post** /v1/organizations/{org}/workspaces/{workspace}/mail/drafts | 
[**WorkspaceCreateMailLabel**](MailAPI.md#WorkspaceCreateMailLabel) | **Post** /v1/organizations/{org}/workspaces/{workspace}/mail/labels | 
[**WorkspaceDeleteMail**](MailAPI.md#WorkspaceDeleteMail) | **Delete** /v1/organizations/{org}/workspaces/{workspace}/mail/email/{id} | 
[**WorkspaceDeleteMailDraft**](MailAPI.md#WorkspaceDeleteMailDraft) | **Delete** /v1/organizations/{org}/workspaces/{workspace}/mail/drafts/{id} | 
[**WorkspaceDeleteMailLabel**](MailAPI.md#WorkspaceDeleteMailLabel) | **Delete** /v1/organizations/{org}/workspaces/{workspace}/mail/labels/{id} | 
[**WorkspaceGetMail**](MailAPI.md#WorkspaceGetMail) | **Get** /v1/organizations/{org}/workspaces/{workspace}/mail/email/{id} | 
[**WorkspaceGetMailAttachment**](MailAPI.md#WorkspaceGetMailAttachment) | **Get** /v1/organizations/{org}/workspaces/{workspace}/mail/attachment/{messageId}/{attachmentId} | 
[**WorkspaceGetMailById**](MailAPI.md#WorkspaceGetMailById) | **Get** /v1/organizations/{org}/workspaces/{workspace}/mail/{id} | Workspace-scoped renderer-compat alias for mail/email/{id}.
[**WorkspaceGetMailDraft**](MailAPI.md#WorkspaceGetMailDraft) | **Get** /v1/organizations/{org}/workspaces/{workspace}/mail/drafts/{id} | 
[**WorkspaceGetMailThread**](MailAPI.md#WorkspaceGetMailThread) | **Get** /v1/organizations/{org}/workspaces/{workspace}/mail/thread/{id} | 
[**WorkspaceListMail**](MailAPI.md#WorkspaceListMail) | **Get** /v1/organizations/{org}/workspaces/{workspace}/mail/list | 
[**WorkspaceListMailDrafts**](MailAPI.md#WorkspaceListMailDrafts) | **Get** /v1/organizations/{org}/workspaces/{workspace}/mail/drafts | 
[**WorkspaceListMailLabels**](MailAPI.md#WorkspaceListMailLabels) | **Get** /v1/organizations/{org}/workspaces/{workspace}/mail/labels | 
[**WorkspacePatchMail**](MailAPI.md#WorkspacePatchMail) | **Patch** /v1/organizations/{org}/workspaces/{workspace}/mail/email/{id} | 
[**WorkspaceRemoveMailMessageLabel**](MailAPI.md#WorkspaceRemoveMailMessageLabel) | **Delete** /v1/organizations/{org}/workspaces/{workspace}/mail/{messageId}/labels/{labelId} | 
[**WorkspaceReplyMail**](MailAPI.md#WorkspaceReplyMail) | **Post** /v1/organizations/{org}/workspaces/{workspace}/mail/reply | 
[**WorkspaceSearchMail**](MailAPI.md#WorkspaceSearchMail) | **Get** /v1/organizations/{org}/workspaces/{workspace}/mail/search | 
[**WorkspaceSendMail**](MailAPI.md#WorkspaceSendMail) | **Post** /v1/organizations/{org}/workspaces/{workspace}/mail/send | 
[**WorkspaceSendMailDraft**](MailAPI.md#WorkspaceSendMailDraft) | **Post** /v1/organizations/{org}/workspaces/{workspace}/mail/drafts/{id}/send | 
[**WorkspaceSendMailEmailAlias**](MailAPI.md#WorkspaceSendMailEmailAlias) | **Post** /v1/organizations/{org}/workspaces/{workspace}/mail/email | Renderer-compat alias for /mail/send.
[**WorkspaceUpdateMail**](MailAPI.md#WorkspaceUpdateMail) | **Put** /v1/organizations/{org}/workspaces/{workspace}/mail/email/{id} | 
[**WorkspaceUpdateMailDraft**](MailAPI.md#WorkspaceUpdateMailDraft) | **Put** /v1/organizations/{org}/workspaces/{workspace}/mail/drafts/{id} | 
[**WorkspaceUpdateMailLabel**](MailAPI.md#WorkspaceUpdateMailLabel) | **Put** /v1/organizations/{org}/workspaces/{workspace}/mail/labels/{id} | 



## BulkArchiveEmails

> BulkArchiveResponse BulkArchiveEmails(ctx).BulkArchiveRequest(bulkArchiveRequest).Execute()

Archive multiple messages (remove the INBOX label).

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
	bulkArchiveRequest := *openapiclient.NewBulkArchiveRequest([]string{"MessageIds_example"}) // BulkArchiveRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.BulkArchiveEmails(context.Background()).BulkArchiveRequest(bulkArchiveRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.BulkArchiveEmails``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BulkArchiveEmails`: BulkArchiveResponse
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.BulkArchiveEmails`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBulkArchiveEmailsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **bulkArchiveRequest** | [**BulkArchiveRequest**](BulkArchiveRequest.md) |  | 

### Return type

[**BulkArchiveResponse**](BulkArchiveResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BulkDeleteEmails

> BulkDeleteEmailsResponse BulkDeleteEmails(ctx).BulkDeleteEmailsRequest(bulkDeleteEmailsRequest).Execute()

Delete multiple messages in one call.



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
	bulkDeleteEmailsRequest := *openapiclient.NewBulkDeleteEmailsRequest([]string{"MessageIds_example"}) // BulkDeleteEmailsRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.BulkDeleteEmails(context.Background()).BulkDeleteEmailsRequest(bulkDeleteEmailsRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.BulkDeleteEmails``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BulkDeleteEmails`: BulkDeleteEmailsResponse
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.BulkDeleteEmails`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBulkDeleteEmailsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **bulkDeleteEmailsRequest** | [**BulkDeleteEmailsRequest**](BulkDeleteEmailsRequest.md) |  | 

### Return type

[**BulkDeleteEmailsResponse**](BulkDeleteEmailsResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BulkMarkEmailsRead

> BulkMarkReadResponse BulkMarkEmailsRead(ctx).BulkMarkReadRequest(bulkMarkReadRequest).Execute()

Mark multiple messages read or unread in one call.

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
	bulkMarkReadRequest := *openapiclient.NewBulkMarkReadRequest([]string{"MessageIds_example"}) // BulkMarkReadRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.BulkMarkEmailsRead(context.Background()).BulkMarkReadRequest(bulkMarkReadRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.BulkMarkEmailsRead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BulkMarkEmailsRead`: BulkMarkReadResponse
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.BulkMarkEmailsRead`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBulkMarkEmailsReadRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **bulkMarkReadRequest** | [**BulkMarkReadRequest**](BulkMarkReadRequest.md) |  | 

### Return type

[**BulkMarkReadResponse**](BulkMarkReadResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateDraft

> DraftResponse CreateDraft(ctx).CreateDraftRequest(createDraftRequest).XWorkspaceID(xWorkspaceID).Execute()

Create a draft.

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
	createDraftRequest := *openapiclient.NewCreateDraftRequest() // CreateDraftRequest | 
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.CreateDraft(context.Background()).CreateDraftRequest(createDraftRequest).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.CreateDraft``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateDraft`: DraftResponse
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.CreateDraft`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateDraftRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createDraftRequest** | [**CreateDraftRequest**](CreateDraftRequest.md) |  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**DraftResponse**](DraftResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateEmailLabel

> CreateLabelResponse CreateEmailLabel(ctx).CreateLabelRequest(createLabelRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Create a label.

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
	createLabelRequest := *openapiclient.NewCreateLabelRequest("Name_example") // CreateLabelRequest | 
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.CreateEmailLabel(context.Background()).CreateLabelRequest(createLabelRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.CreateEmailLabel``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateEmailLabel`: CreateLabelResponse
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.CreateEmailLabel`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateEmailLabelRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createLabelRequest** | [**CreateLabelRequest**](CreateLabelRequest.md) |  | 
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**CreateLabelResponse**](CreateLabelResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateMailTemplate

> map[string]interface{} CreateMailTemplate(ctx).RequestBody(requestBody).Execute()

Create a mail template.

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
	resp, r, err := apiClient.MailAPI.CreateMailTemplate(context.Background()).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.CreateMailTemplate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateMailTemplate`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.CreateMailTemplate`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateMailTemplateRequest struct via the builder pattern


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


## DeleteDraft

> DeleteDraft(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Delete a draft.

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
	id := "id_example" // string | Draft id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MailAPI.DeleteDraft(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.DeleteDraft``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Draft id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteDraftRequest struct via the builder pattern


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


## DeleteEmail

> SuccessFlag DeleteEmail(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Delete an email.



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
	id := "id_example" // string | Email message id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.DeleteEmail(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.DeleteEmail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteEmail`: SuccessFlag
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.DeleteEmail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Email message id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteEmailRequest struct via the builder pattern


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


## DeleteEmailLabel

> DeleteEmailLabel(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Delete a label.

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
	id := "id_example" // string | Label id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MailAPI.DeleteEmailLabel(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.DeleteEmailLabel``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Label id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteEmailLabelRequest struct via the builder pattern


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


## DeleteMailTemplate

> DeleteMailTemplate(ctx, id).Execute()

Delete a mail template.

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
	r, err := apiClient.MailAPI.DeleteMailTemplate(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.DeleteMailTemplate``: %v\n", err)
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

Other parameters are passed through a pointer to a apiDeleteMailTemplateRequest struct via the builder pattern


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


## GetEmail

> GetEmailResponse GetEmail(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Fetch one email.

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
	id := "id_example" // string | Email message id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.GetEmail(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.GetEmail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetEmail`: GetEmailResponse
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.GetEmail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Email message id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetEmailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**GetEmailResponse**](GetEmailResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetEmailAttachment

> *os.File GetEmailAttachment(ctx, messageId, attachmentId).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Download an attachment.



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
	messageId := "messageId_example" // string | Message id the attachment belongs to.
	attachmentId := "attachmentId_example" // string | Attachment id within the message.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.GetEmailAttachment(context.Background(), messageId, attachmentId).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.GetEmailAttachment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetEmailAttachment`: *os.File
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.GetEmailAttachment`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**messageId** | **string** | Message id the attachment belongs to. | 
**attachmentId** | **string** | Attachment id within the message. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetEmailAttachmentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[***os.File**](*os.File.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/octet-stream, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetEmailThread

> GetThreadResponse GetEmailThread(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Fetch a thread (the conversation a message belongs to).

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
	id := "id_example" // string | Thread id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.GetEmailThread(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.GetEmailThread``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetEmailThread`: GetThreadResponse
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.GetEmailThread`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Thread id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetEmailThreadRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**GetThreadResponse**](GetThreadResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetMailTemplate

> map[string]interface{} GetMailTemplate(ctx, id).Execute()

Fetch a mail template.

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
	resp, r, err := apiClient.MailAPI.GetMailTemplate(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.GetMailTemplate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetMailTemplate`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.GetMailTemplate`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetMailTemplateRequest struct via the builder pattern


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


## GetMailThreadTracking

> map[string]interface{} GetMailThreadTracking(ctx, threadId).Execute()

Read mail-tracking events for a thread (open log, reply log, etc.).

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
	threadId := "threadId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.GetMailThreadTracking(context.Background(), threadId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.GetMailThreadTracking``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetMailThreadTracking`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.GetMailThreadTracking`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**threadId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetMailThreadTrackingRequest struct via the builder pattern


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


## InstantiateMailTemplate

> map[string]interface{} InstantiateMailTemplate(ctx, id).RequestBody(requestBody).Execute()

Render a template with variables and return the resulting draft.

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
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.InstantiateMailTemplate(context.Background(), id).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.InstantiateMailTemplate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `InstantiateMailTemplate`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.InstantiateMailTemplate`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiInstantiateMailTemplateRequest struct via the builder pattern


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


## ListDrafts

> ListDraftsResponse ListDrafts(ctx).XWorkspaceID(xWorkspaceID).AccountIds(accountIds).Providers(providers).Limit(limit).NextPageToken(nextPageToken).Execute()

List drafts across connected mail accounts.

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
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)
	accountIds := []string{"Inner_example"} // []string | Repeatable. Restrict to these connected-account row ids. Mutually orthogonal to `providers` — when both are set the intersection is used.  (optional)
	providers := []string{"Inner_example"} // []string | Repeatable. Restrict to these provider ids (`gmail`, `outlook`). (optional)
	limit := int32(56) // int32 |  (optional) (default to 50)
	nextPageToken := "nextPageToken_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.ListDrafts(context.Background()).XWorkspaceID(xWorkspaceID).AccountIds(accountIds).Providers(providers).Limit(limit).NextPageToken(nextPageToken).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.ListDrafts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListDrafts`: ListDraftsResponse
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.ListDrafts`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListDraftsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 
 **accountIds** | **[]string** | Repeatable. Restrict to these connected-account row ids. Mutually orthogonal to &#x60;providers&#x60; — when both are set the intersection is used.  | 
 **providers** | **[]string** | Repeatable. Restrict to these provider ids (&#x60;gmail&#x60;, &#x60;outlook&#x60;). | 
 **limit** | **int32** |  | [default to 50]
 **nextPageToken** | **string** |  | 

### Return type

[**ListDraftsResponse**](ListDraftsResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListEmailLabels

> ListLabelsResponse ListEmailLabels(ctx).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

List labels on the resolved mail account.



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
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.ListEmailLabels(context.Background()).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.ListEmailLabels``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListEmailLabels`: ListLabelsResponse
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.ListEmailLabels`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListEmailLabelsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**ListLabelsResponse**](ListLabelsResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListEmails

> ListEmailsResponse ListEmails(ctx).AccountIds(accountIds).Providers(providers).XWorkspaceID(xWorkspaceID).Query(query).Labels(labels).Folder(folder).Limit(limit).Offset(offset).Execute()

List emails across connected mail accounts.



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
	accountIds := []string{"Inner_example"} // []string | Repeatable. Restrict to these connected-account row ids. Mutually orthogonal to `providers` — when both are set the intersection is used.  (optional)
	providers := []string{"Inner_example"} // []string | Repeatable. Restrict to these provider ids (`gmail`, `outlook`). (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)
	query := "query_example" // string | Provider-specific full-text query (e.g. Gmail search syntax). (optional)
	labels := []string{"Inner_example"} // []string | Repeatable. Filter to messages carrying every label. (optional)
	folder := "folder_example" // string | Logical folder filter. Canonical values: `inbox`, `sent`, `starred`, `trash`, `archive`. Provider-specific folders accepted as opaque strings.  (optional)
	limit := int32(56) // int32 |  (optional) (default to 50)
	offset := int32(56) // int32 |  (optional) (default to 0)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.ListEmails(context.Background()).AccountIds(accountIds).Providers(providers).XWorkspaceID(xWorkspaceID).Query(query).Labels(labels).Folder(folder).Limit(limit).Offset(offset).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.ListEmails``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListEmails`: ListEmailsResponse
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.ListEmails`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListEmailsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accountIds** | **[]string** | Repeatable. Restrict to these connected-account row ids. Mutually orthogonal to &#x60;providers&#x60; — when both are set the intersection is used.  | 
 **providers** | **[]string** | Repeatable. Restrict to these provider ids (&#x60;gmail&#x60;, &#x60;outlook&#x60;). | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 
 **query** | **string** | Provider-specific full-text query (e.g. Gmail search syntax). | 
 **labels** | **[]string** | Repeatable. Filter to messages carrying every label. | 
 **folder** | **string** | Logical folder filter. Canonical values: &#x60;inbox&#x60;, &#x60;sent&#x60;, &#x60;starred&#x60;, &#x60;trash&#x60;, &#x60;archive&#x60;. Provider-specific folders accepted as opaque strings.  | 
 **limit** | **int32** |  | [default to 50]
 **offset** | **int32** |  | [default to 0]

### Return type

[**ListEmailsResponse**](ListEmailsResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListMailTemplates

> map[string]interface{} ListMailTemplates(ctx).Execute()

List the caller's saved mail templates.

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
	resp, r, err := apiClient.MailAPI.ListMailTemplates(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.ListMailTemplates``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListMailTemplates`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.ListMailTemplates`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListMailTemplatesRequest struct via the builder pattern


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


## ReplyEmail

> SendEmailResponse ReplyEmail(ctx).MessageId(messageId).ReplyEmailRequest(replyEmailRequest).XWorkspaceID(xWorkspaceID).Execute()

Reply to a specific email.



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
	messageId := "messageId_example" // string | Id of the message being replied to.
	replyEmailRequest := *openapiclient.NewReplyEmailRequest("Body_example") // ReplyEmailRequest | 
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.ReplyEmail(context.Background()).MessageId(messageId).ReplyEmailRequest(replyEmailRequest).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.ReplyEmail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ReplyEmail`: SendEmailResponse
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.ReplyEmail`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiReplyEmailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **messageId** | **string** | Id of the message being replied to. | 
 **replyEmailRequest** | [**ReplyEmailRequest**](ReplyEmailRequest.md) |  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**SendEmailResponse**](SendEmailResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SaveMailTemplate

> map[string]interface{} SaveMailTemplate(ctx).RequestBody(requestBody).Execute()

Save-or-create endpoint used by the renderer's \"save as template\" flow. Distinct from POST /v1/mail/templates which is the strict create. 

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
	resp, r, err := apiClient.MailAPI.SaveMailTemplate(context.Background()).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.SaveMailTemplate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SaveMailTemplate`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.SaveMailTemplate`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSaveMailTemplateRequest struct via the builder pattern


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


## SearchEmails

> SearchEmailsResponse SearchEmails(ctx).Q(q).AccountIds(accountIds).Providers(providers).XWorkspaceID(xWorkspaceID).From(from).To(to).Subject(subject).HasAttachment(hasAttachment).IsUnread(isUnread).IsStarred(isStarred).Labels(labels).After(after).Before(before).Limit(limit).NextPageToken(nextPageToken).Execute()

Structured search across connected mail accounts.



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/spatio-labs/spatio-go"
)

func main() {
	q := "q_example" // string | Provider-specific full-text query string.
	accountIds := []string{"Inner_example"} // []string | Repeatable. Restrict to these connected-account row ids. Mutually orthogonal to `providers` — when both are set the intersection is used.  (optional)
	providers := []string{"Inner_example"} // []string | Repeatable. Restrict to these provider ids (`gmail`, `outlook`). (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)
	from := "from_example" // string |  (optional)
	to := "to_example" // string |  (optional)
	subject := "subject_example" // string |  (optional)
	hasAttachment := true // bool |  (optional)
	isUnread := true // bool |  (optional)
	isStarred := true // bool |  (optional)
	labels := []string{"Inner_example"} // []string |  (optional)
	after := time.Now() // time.Time | Inclusive lower-bound date. (optional)
	before := time.Now() // time.Time | Inclusive upper-bound date. (optional)
	limit := int32(56) // int32 |  (optional) (default to 50)
	nextPageToken := "nextPageToken_example" // string | Cursor returned by the previous call. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.SearchEmails(context.Background()).Q(q).AccountIds(accountIds).Providers(providers).XWorkspaceID(xWorkspaceID).From(from).To(to).Subject(subject).HasAttachment(hasAttachment).IsUnread(isUnread).IsStarred(isStarred).Labels(labels).After(after).Before(before).Limit(limit).NextPageToken(nextPageToken).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.SearchEmails``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SearchEmails`: SearchEmailsResponse
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.SearchEmails`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSearchEmailsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Provider-specific full-text query string. | 
 **accountIds** | **[]string** | Repeatable. Restrict to these connected-account row ids. Mutually orthogonal to &#x60;providers&#x60; — when both are set the intersection is used.  | 
 **providers** | **[]string** | Repeatable. Restrict to these provider ids (&#x60;gmail&#x60;, &#x60;outlook&#x60;). | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 
 **from** | **string** |  | 
 **to** | **string** |  | 
 **subject** | **string** |  | 
 **hasAttachment** | **bool** |  | 
 **isUnread** | **bool** |  | 
 **isStarred** | **bool** |  | 
 **labels** | **[]string** |  | 
 **after** | **time.Time** | Inclusive lower-bound date. | 
 **before** | **time.Time** | Inclusive upper-bound date. | 
 **limit** | **int32** |  | [default to 50]
 **nextPageToken** | **string** | Cursor returned by the previous call. | 

### Return type

[**SearchEmailsResponse**](SearchEmailsResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SendDraft

> SendEmailResponse SendDraft(ctx, id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Send a draft.



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
	id := "id_example" // string | Draft id.
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.SendDraft(context.Background(), id).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.SendDraft``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SendDraft`: SendEmailResponse
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.SendDraft`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Draft id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiSendDraftRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**SendEmailResponse**](SendEmailResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SendEmail

> SendEmailResponse SendEmail(ctx).SendEmailRequest(sendEmailRequest).XWorkspaceID(xWorkspaceID).Execute()

Send an email.



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
	sendEmailRequest := *openapiclient.NewSendEmailRequest([]string{"To_example"}, "Subject_example", "Body_example") // SendEmailRequest | 
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.SendEmail(context.Background()).SendEmailRequest(sendEmailRequest).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.SendEmail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SendEmail`: SendEmailResponse
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.SendEmail`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSendEmailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sendEmailRequest** | [**SendEmailRequest**](SendEmailRequest.md) |  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**SendEmailResponse**](SendEmailResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateDraft

> DraftResponse UpdateDraft(ctx, id).UpdateDraftRequest(updateDraftRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Update a draft (full replacement of provided fields).



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
	id := "id_example" // string | Draft id.
	updateDraftRequest := *openapiclient.NewUpdateDraftRequest() // UpdateDraftRequest | 
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.UpdateDraft(context.Background(), id).UpdateDraftRequest(updateDraftRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.UpdateDraft``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateDraft`: DraftResponse
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.UpdateDraft`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Draft id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateDraftRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateDraftRequest** | [**UpdateDraftRequest**](UpdateDraftRequest.md) |  | 
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**DraftResponse**](DraftResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateEmail

> UpdateEmailResponse UpdateEmail(ctx, id).UpdateEmailRequest(updateEmailRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()

Update an email (mark read/star, add/remove labels).

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
	id := "id_example" // string | Email message id.
	updateEmailRequest := *openapiclient.NewUpdateEmailRequest() // UpdateEmailRequest | 
	accountId := "accountId_example" // string | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with `provider`. If omitted on a list endpoint the call fans out across every connected account.  (optional)
	xWorkspaceID := "xWorkspaceID_example" // string | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.UpdateEmail(context.Background(), id).UpdateEmailRequest(updateEmailRequest).AccountId(accountId).XWorkspaceID(xWorkspaceID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.UpdateEmail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateEmail`: UpdateEmailResponse
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.UpdateEmail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Email message id. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateEmailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateEmailRequest** | [**UpdateEmailRequest**](UpdateEmailRequest.md) |  | 
 **accountId** | **string** | Connected-account row id. Selects which provider account this request targets when more than one is connected. Mutually exclusive with &#x60;provider&#x60;. If omitted on a list endpoint the call fans out across every connected account.  | 
 **xWorkspaceID** | **string** | Workspace scope for unscoped tokens. Workspace-scoped PATs and OAuth tokens carry this implicitly; for session/JWT auth without a scoped PAT, pass it explicitly.  | 

### Return type

[**UpdateEmailResponse**](UpdateEmailResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateMailTemplate

> map[string]interface{} UpdateMailTemplate(ctx, id).RequestBody(requestBody).Execute()

Update a mail template.

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
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.UpdateMailTemplate(context.Background(), id).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.UpdateMailTemplate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateMailTemplate`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.UpdateMailTemplate`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateMailTemplateRequest struct via the builder pattern


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


## WorkspaceAddMailMessageLabels

> map[string]interface{} WorkspaceAddMailMessageLabels(ctx, org, workspace, messageId).RequestBody(requestBody).Execute()



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
	workspace := "workspace_example" // string | 
	messageId := "messageId_example" // string | 
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.WorkspaceAddMailMessageLabels(context.Background(), org, workspace, messageId).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.WorkspaceAddMailMessageLabels``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceAddMailMessageLabels`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.WorkspaceAddMailMessageLabels`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 
**messageId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceAddMailMessageLabelsRequest struct via the builder pattern


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


## WorkspaceCreateMailDraft

> map[string]interface{} WorkspaceCreateMailDraft(ctx, org, workspace).RequestBody(requestBody).Execute()



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
	workspace := "workspace_example" // string | 
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.WorkspaceCreateMailDraft(context.Background(), org, workspace).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.WorkspaceCreateMailDraft``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceCreateMailDraft`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.WorkspaceCreateMailDraft`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceCreateMailDraftRequest struct via the builder pattern


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


## WorkspaceCreateMailLabel

> map[string]interface{} WorkspaceCreateMailLabel(ctx, org, workspace).RequestBody(requestBody).Execute()



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
	workspace := "workspace_example" // string | 
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.WorkspaceCreateMailLabel(context.Background(), org, workspace).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.WorkspaceCreateMailLabel``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceCreateMailLabel`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.WorkspaceCreateMailLabel`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceCreateMailLabelRequest struct via the builder pattern


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


## WorkspaceDeleteMail

> WorkspaceDeleteMail(ctx, org, workspace, id).Execute()



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
	workspace := "workspace_example" // string | 
	id := "id_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MailAPI.WorkspaceDeleteMail(context.Background(), org, workspace, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.WorkspaceDeleteMail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceDeleteMailRequest struct via the builder pattern


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


## WorkspaceDeleteMailDraft

> WorkspaceDeleteMailDraft(ctx, org, workspace, id).Execute()



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
	workspace := "workspace_example" // string | 
	id := "id_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MailAPI.WorkspaceDeleteMailDraft(context.Background(), org, workspace, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.WorkspaceDeleteMailDraft``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceDeleteMailDraftRequest struct via the builder pattern


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


## WorkspaceDeleteMailLabel

> WorkspaceDeleteMailLabel(ctx, org, workspace, id).Execute()



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
	workspace := "workspace_example" // string | 
	id := "id_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MailAPI.WorkspaceDeleteMailLabel(context.Background(), org, workspace, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.WorkspaceDeleteMailLabel``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceDeleteMailLabelRequest struct via the builder pattern


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


## WorkspaceGetMail

> map[string]interface{} WorkspaceGetMail(ctx, org, workspace, id).Execute()



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
	workspace := "workspace_example" // string | 
	id := "id_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.WorkspaceGetMail(context.Background(), org, workspace, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.WorkspaceGetMail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceGetMail`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.WorkspaceGetMail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceGetMailRequest struct via the builder pattern


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


## WorkspaceGetMailAttachment

> map[string]interface{} WorkspaceGetMailAttachment(ctx, org, workspace, messageId, attachmentId).Execute()



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
	workspace := "workspace_example" // string | 
	messageId := "messageId_example" // string | 
	attachmentId := "attachmentId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.WorkspaceGetMailAttachment(context.Background(), org, workspace, messageId, attachmentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.WorkspaceGetMailAttachment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceGetMailAttachment`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.WorkspaceGetMailAttachment`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 
**messageId** | **string** |  | 
**attachmentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceGetMailAttachmentRequest struct via the builder pattern


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


## WorkspaceGetMailById

> map[string]interface{} WorkspaceGetMailById(ctx, org, workspace, id).Execute()

Workspace-scoped renderer-compat alias for mail/email/{id}.

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
	workspace := "workspace_example" // string | 
	id := "id_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.WorkspaceGetMailById(context.Background(), org, workspace, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.WorkspaceGetMailById``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceGetMailById`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.WorkspaceGetMailById`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceGetMailByIdRequest struct via the builder pattern


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


## WorkspaceGetMailDraft

> map[string]interface{} WorkspaceGetMailDraft(ctx, org, workspace, id).Execute()



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
	workspace := "workspace_example" // string | 
	id := "id_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.WorkspaceGetMailDraft(context.Background(), org, workspace, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.WorkspaceGetMailDraft``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceGetMailDraft`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.WorkspaceGetMailDraft`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceGetMailDraftRequest struct via the builder pattern


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


## WorkspaceGetMailThread

> map[string]interface{} WorkspaceGetMailThread(ctx, org, workspace, id).Execute()



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
	workspace := "workspace_example" // string | 
	id := "id_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.WorkspaceGetMailThread(context.Background(), org, workspace, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.WorkspaceGetMailThread``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceGetMailThread`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.WorkspaceGetMailThread`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceGetMailThreadRequest struct via the builder pattern


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


## WorkspaceListMail

> map[string]interface{} WorkspaceListMail(ctx, org, workspace).Execute()



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
	workspace := "workspace_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.WorkspaceListMail(context.Background(), org, workspace).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.WorkspaceListMail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceListMail`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.WorkspaceListMail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceListMailRequest struct via the builder pattern


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


## WorkspaceListMailDrafts

> map[string]interface{} WorkspaceListMailDrafts(ctx, org, workspace).Execute()



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
	workspace := "workspace_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.WorkspaceListMailDrafts(context.Background(), org, workspace).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.WorkspaceListMailDrafts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceListMailDrafts`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.WorkspaceListMailDrafts`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceListMailDraftsRequest struct via the builder pattern


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


## WorkspaceListMailLabels

> map[string]interface{} WorkspaceListMailLabels(ctx, org, workspace).Execute()



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
	workspace := "workspace_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.WorkspaceListMailLabels(context.Background(), org, workspace).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.WorkspaceListMailLabels``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceListMailLabels`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.WorkspaceListMailLabels`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceListMailLabelsRequest struct via the builder pattern


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


## WorkspacePatchMail

> map[string]interface{} WorkspacePatchMail(ctx, org, workspace, id).RequestBody(requestBody).Execute()



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
	workspace := "workspace_example" // string | 
	id := "id_example" // string | 
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.WorkspacePatchMail(context.Background(), org, workspace, id).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.WorkspacePatchMail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspacePatchMail`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.WorkspacePatchMail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspacePatchMailRequest struct via the builder pattern


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


## WorkspaceRemoveMailMessageLabel

> WorkspaceRemoveMailMessageLabel(ctx, org, workspace, messageId, labelId).Execute()



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
	workspace := "workspace_example" // string | 
	messageId := "messageId_example" // string | 
	labelId := "labelId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MailAPI.WorkspaceRemoveMailMessageLabel(context.Background(), org, workspace, messageId, labelId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.WorkspaceRemoveMailMessageLabel``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 
**messageId** | **string** |  | 
**labelId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceRemoveMailMessageLabelRequest struct via the builder pattern


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


## WorkspaceReplyMail

> map[string]interface{} WorkspaceReplyMail(ctx, org, workspace).RequestBody(requestBody).Execute()



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
	workspace := "workspace_example" // string | 
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.WorkspaceReplyMail(context.Background(), org, workspace).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.WorkspaceReplyMail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceReplyMail`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.WorkspaceReplyMail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceReplyMailRequest struct via the builder pattern


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


## WorkspaceSearchMail

> map[string]interface{} WorkspaceSearchMail(ctx, org, workspace).Q(q).Execute()



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
	workspace := "workspace_example" // string | 
	q := "q_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.WorkspaceSearchMail(context.Background(), org, workspace).Q(q).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.WorkspaceSearchMail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceSearchMail`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.WorkspaceSearchMail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceSearchMailRequest struct via the builder pattern


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


## WorkspaceSendMail

> map[string]interface{} WorkspaceSendMail(ctx, org, workspace).RequestBody(requestBody).Execute()



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
	workspace := "workspace_example" // string | 
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.WorkspaceSendMail(context.Background(), org, workspace).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.WorkspaceSendMail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceSendMail`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.WorkspaceSendMail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceSendMailRequest struct via the builder pattern


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


## WorkspaceSendMailDraft

> map[string]interface{} WorkspaceSendMailDraft(ctx, org, workspace, id).Execute()



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
	workspace := "workspace_example" // string | 
	id := "id_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.WorkspaceSendMailDraft(context.Background(), org, workspace, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.WorkspaceSendMailDraft``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceSendMailDraft`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.WorkspaceSendMailDraft`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceSendMailDraftRequest struct via the builder pattern


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


## WorkspaceSendMailEmailAlias

> map[string]interface{} WorkspaceSendMailEmailAlias(ctx, org, workspace).RequestBody(requestBody).Execute()

Renderer-compat alias for /mail/send.

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
	workspace := "workspace_example" // string | 
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.WorkspaceSendMailEmailAlias(context.Background(), org, workspace).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.WorkspaceSendMailEmailAlias``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceSendMailEmailAlias`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.WorkspaceSendMailEmailAlias`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceSendMailEmailAliasRequest struct via the builder pattern


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


## WorkspaceUpdateMail

> map[string]interface{} WorkspaceUpdateMail(ctx, org, workspace, id).RequestBody(requestBody).Execute()



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
	workspace := "workspace_example" // string | 
	id := "id_example" // string | 
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.WorkspaceUpdateMail(context.Background(), org, workspace, id).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.WorkspaceUpdateMail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceUpdateMail`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.WorkspaceUpdateMail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceUpdateMailRequest struct via the builder pattern


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


## WorkspaceUpdateMailDraft

> map[string]interface{} WorkspaceUpdateMailDraft(ctx, org, workspace, id).RequestBody(requestBody).Execute()



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
	workspace := "workspace_example" // string | 
	id := "id_example" // string | 
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.WorkspaceUpdateMailDraft(context.Background(), org, workspace, id).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.WorkspaceUpdateMailDraft``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceUpdateMailDraft`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.WorkspaceUpdateMailDraft`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceUpdateMailDraftRequest struct via the builder pattern


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


## WorkspaceUpdateMailLabel

> map[string]interface{} WorkspaceUpdateMailLabel(ctx, org, workspace, id).RequestBody(requestBody).Execute()



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
	workspace := "workspace_example" // string | 
	id := "id_example" // string | 
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MailAPI.WorkspaceUpdateMailLabel(context.Background(), org, workspace, id).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MailAPI.WorkspaceUpdateMailLabel``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkspaceUpdateMailLabel`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MailAPI.WorkspaceUpdateMailLabel`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**org** | **string** |  | 
**workspace** | **string** |  | 
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWorkspaceUpdateMailLabelRequest struct via the builder pattern


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

