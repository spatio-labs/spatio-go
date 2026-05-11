# UpdateDraftRequest

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

## Methods

### NewUpdateDraftRequest

`func NewUpdateDraftRequest() *UpdateDraftRequest`

NewUpdateDraftRequest instantiates a new UpdateDraftRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateDraftRequestWithDefaults

`func NewUpdateDraftRequestWithDefaults() *UpdateDraftRequest`

NewUpdateDraftRequestWithDefaults instantiates a new UpdateDraftRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAccountId

`func (o *UpdateDraftRequest) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *UpdateDraftRequest) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *UpdateDraftRequest) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *UpdateDraftRequest) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.

### GetTo

`func (o *UpdateDraftRequest) GetTo() []string`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *UpdateDraftRequest) GetToOk() (*[]string, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *UpdateDraftRequest) SetTo(v []string)`

SetTo sets To field to given value.

### HasTo

`func (o *UpdateDraftRequest) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetCc

`func (o *UpdateDraftRequest) GetCc() []string`

GetCc returns the Cc field if non-nil, zero value otherwise.

### GetCcOk

`func (o *UpdateDraftRequest) GetCcOk() (*[]string, bool)`

GetCcOk returns a tuple with the Cc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCc

`func (o *UpdateDraftRequest) SetCc(v []string)`

SetCc sets Cc field to given value.

### HasCc

`func (o *UpdateDraftRequest) HasCc() bool`

HasCc returns a boolean if a field has been set.

### GetBcc

`func (o *UpdateDraftRequest) GetBcc() []string`

GetBcc returns the Bcc field if non-nil, zero value otherwise.

### GetBccOk

`func (o *UpdateDraftRequest) GetBccOk() (*[]string, bool)`

GetBccOk returns a tuple with the Bcc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBcc

`func (o *UpdateDraftRequest) SetBcc(v []string)`

SetBcc sets Bcc field to given value.

### HasBcc

`func (o *UpdateDraftRequest) HasBcc() bool`

HasBcc returns a boolean if a field has been set.

### GetSubject

`func (o *UpdateDraftRequest) GetSubject() string`

GetSubject returns the Subject field if non-nil, zero value otherwise.

### GetSubjectOk

`func (o *UpdateDraftRequest) GetSubjectOk() (*string, bool)`

GetSubjectOk returns a tuple with the Subject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubject

`func (o *UpdateDraftRequest) SetSubject(v string)`

SetSubject sets Subject field to given value.

### HasSubject

`func (o *UpdateDraftRequest) HasSubject() bool`

HasSubject returns a boolean if a field has been set.

### GetBody

`func (o *UpdateDraftRequest) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *UpdateDraftRequest) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *UpdateDraftRequest) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *UpdateDraftRequest) HasBody() bool`

HasBody returns a boolean if a field has been set.

### GetHtml

`func (o *UpdateDraftRequest) GetHtml() bool`

GetHtml returns the Html field if non-nil, zero value otherwise.

### GetHtmlOk

`func (o *UpdateDraftRequest) GetHtmlOk() (*bool, bool)`

GetHtmlOk returns a tuple with the Html field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHtml

`func (o *UpdateDraftRequest) SetHtml(v bool)`

SetHtml sets Html field to given value.

### HasHtml

`func (o *UpdateDraftRequest) HasHtml() bool`

HasHtml returns a boolean if a field has been set.

### GetAttachments

`func (o *UpdateDraftRequest) GetAttachments() []AttachmentInput`

GetAttachments returns the Attachments field if non-nil, zero value otherwise.

### GetAttachmentsOk

`func (o *UpdateDraftRequest) GetAttachmentsOk() (*[]AttachmentInput, bool)`

GetAttachmentsOk returns a tuple with the Attachments field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttachments

`func (o *UpdateDraftRequest) SetAttachments(v []AttachmentInput)`

SetAttachments sets Attachments field to given value.

### HasAttachments

`func (o *UpdateDraftRequest) HasAttachments() bool`

HasAttachments returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


