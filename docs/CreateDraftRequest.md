# CreateDraftRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AccountId** | Pointer to **string** |  | [optional] 
**To** | Pointer to **[]string** |  | [optional] 
**Cc** | Pointer to **[]string** |  | [optional] 
**Bcc** | Pointer to **[]string** |  | [optional] 
**Subject** | Pointer to **string** |  | [optional] 
**Body** | Pointer to **string** |  | [optional] 
**Html** | Pointer to **bool** |  | [optional] 
**Attachments** | Pointer to [**[]AttachmentInput**](AttachmentInput.md) |  | [optional] 
**ThreadId** | Pointer to **string** | Provider thread id — set when this draft is a reply, so the sent message lands inside the parent thread.  | [optional] 
**InReplyTo** | Pointer to **string** |  | [optional] 
**References** | Pointer to **[]string** |  | [optional] 

## Methods

### NewCreateDraftRequest

`func NewCreateDraftRequest() *CreateDraftRequest`

NewCreateDraftRequest instantiates a new CreateDraftRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateDraftRequestWithDefaults

`func NewCreateDraftRequestWithDefaults() *CreateDraftRequest`

NewCreateDraftRequestWithDefaults instantiates a new CreateDraftRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAccountId

`func (o *CreateDraftRequest) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *CreateDraftRequest) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *CreateDraftRequest) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *CreateDraftRequest) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.

### GetTo

`func (o *CreateDraftRequest) GetTo() []string`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *CreateDraftRequest) GetToOk() (*[]string, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *CreateDraftRequest) SetTo(v []string)`

SetTo sets To field to given value.

### HasTo

`func (o *CreateDraftRequest) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetCc

`func (o *CreateDraftRequest) GetCc() []string`

GetCc returns the Cc field if non-nil, zero value otherwise.

### GetCcOk

`func (o *CreateDraftRequest) GetCcOk() (*[]string, bool)`

GetCcOk returns a tuple with the Cc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCc

`func (o *CreateDraftRequest) SetCc(v []string)`

SetCc sets Cc field to given value.

### HasCc

`func (o *CreateDraftRequest) HasCc() bool`

HasCc returns a boolean if a field has been set.

### GetBcc

`func (o *CreateDraftRequest) GetBcc() []string`

GetBcc returns the Bcc field if non-nil, zero value otherwise.

### GetBccOk

`func (o *CreateDraftRequest) GetBccOk() (*[]string, bool)`

GetBccOk returns a tuple with the Bcc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBcc

`func (o *CreateDraftRequest) SetBcc(v []string)`

SetBcc sets Bcc field to given value.

### HasBcc

`func (o *CreateDraftRequest) HasBcc() bool`

HasBcc returns a boolean if a field has been set.

### GetSubject

`func (o *CreateDraftRequest) GetSubject() string`

GetSubject returns the Subject field if non-nil, zero value otherwise.

### GetSubjectOk

`func (o *CreateDraftRequest) GetSubjectOk() (*string, bool)`

GetSubjectOk returns a tuple with the Subject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubject

`func (o *CreateDraftRequest) SetSubject(v string)`

SetSubject sets Subject field to given value.

### HasSubject

`func (o *CreateDraftRequest) HasSubject() bool`

HasSubject returns a boolean if a field has been set.

### GetBody

`func (o *CreateDraftRequest) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *CreateDraftRequest) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *CreateDraftRequest) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *CreateDraftRequest) HasBody() bool`

HasBody returns a boolean if a field has been set.

### GetHtml

`func (o *CreateDraftRequest) GetHtml() bool`

GetHtml returns the Html field if non-nil, zero value otherwise.

### GetHtmlOk

`func (o *CreateDraftRequest) GetHtmlOk() (*bool, bool)`

GetHtmlOk returns a tuple with the Html field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHtml

`func (o *CreateDraftRequest) SetHtml(v bool)`

SetHtml sets Html field to given value.

### HasHtml

`func (o *CreateDraftRequest) HasHtml() bool`

HasHtml returns a boolean if a field has been set.

### GetAttachments

`func (o *CreateDraftRequest) GetAttachments() []AttachmentInput`

GetAttachments returns the Attachments field if non-nil, zero value otherwise.

### GetAttachmentsOk

`func (o *CreateDraftRequest) GetAttachmentsOk() (*[]AttachmentInput, bool)`

GetAttachmentsOk returns a tuple with the Attachments field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttachments

`func (o *CreateDraftRequest) SetAttachments(v []AttachmentInput)`

SetAttachments sets Attachments field to given value.

### HasAttachments

`func (o *CreateDraftRequest) HasAttachments() bool`

HasAttachments returns a boolean if a field has been set.

### GetThreadId

`func (o *CreateDraftRequest) GetThreadId() string`

GetThreadId returns the ThreadId field if non-nil, zero value otherwise.

### GetThreadIdOk

`func (o *CreateDraftRequest) GetThreadIdOk() (*string, bool)`

GetThreadIdOk returns a tuple with the ThreadId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetThreadId

`func (o *CreateDraftRequest) SetThreadId(v string)`

SetThreadId sets ThreadId field to given value.

### HasThreadId

`func (o *CreateDraftRequest) HasThreadId() bool`

HasThreadId returns a boolean if a field has been set.

### GetInReplyTo

`func (o *CreateDraftRequest) GetInReplyTo() string`

GetInReplyTo returns the InReplyTo field if non-nil, zero value otherwise.

### GetInReplyToOk

`func (o *CreateDraftRequest) GetInReplyToOk() (*string, bool)`

GetInReplyToOk returns a tuple with the InReplyTo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInReplyTo

`func (o *CreateDraftRequest) SetInReplyTo(v string)`

SetInReplyTo sets InReplyTo field to given value.

### HasInReplyTo

`func (o *CreateDraftRequest) HasInReplyTo() bool`

HasInReplyTo returns a boolean if a field has been set.

### GetReferences

`func (o *CreateDraftRequest) GetReferences() []string`

GetReferences returns the References field if non-nil, zero value otherwise.

### GetReferencesOk

`func (o *CreateDraftRequest) GetReferencesOk() (*[]string, bool)`

GetReferencesOk returns a tuple with the References field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReferences

`func (o *CreateDraftRequest) SetReferences(v []string)`

SetReferences sets References field to given value.

### HasReferences

`func (o *CreateDraftRequest) HasReferences() bool`

HasReferences returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


