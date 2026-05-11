# SendEmailRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AccountId** | Pointer to **string** |  | [optional] 
**To** | **[]string** |  | 
**Cc** | Pointer to **[]string** |  | [optional] 
**Bcc** | Pointer to **[]string** |  | [optional] 
**Subject** | **string** |  | 
**Body** | **string** |  | 
**Html** | Pointer to **bool** |  | [optional] 
**Attachments** | Pointer to [**[]AttachmentInput**](AttachmentInput.md) |  | [optional] 
**InReplyTo** | Pointer to **string** |  | [optional] 
**References** | Pointer to **[]string** |  | [optional] 

## Methods

### NewSendEmailRequest

`func NewSendEmailRequest(to []string, subject string, body string, ) *SendEmailRequest`

NewSendEmailRequest instantiates a new SendEmailRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSendEmailRequestWithDefaults

`func NewSendEmailRequestWithDefaults() *SendEmailRequest`

NewSendEmailRequestWithDefaults instantiates a new SendEmailRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAccountId

`func (o *SendEmailRequest) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *SendEmailRequest) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *SendEmailRequest) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *SendEmailRequest) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.

### GetTo

`func (o *SendEmailRequest) GetTo() []string`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *SendEmailRequest) GetToOk() (*[]string, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *SendEmailRequest) SetTo(v []string)`

SetTo sets To field to given value.


### GetCc

`func (o *SendEmailRequest) GetCc() []string`

GetCc returns the Cc field if non-nil, zero value otherwise.

### GetCcOk

`func (o *SendEmailRequest) GetCcOk() (*[]string, bool)`

GetCcOk returns a tuple with the Cc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCc

`func (o *SendEmailRequest) SetCc(v []string)`

SetCc sets Cc field to given value.

### HasCc

`func (o *SendEmailRequest) HasCc() bool`

HasCc returns a boolean if a field has been set.

### GetBcc

`func (o *SendEmailRequest) GetBcc() []string`

GetBcc returns the Bcc field if non-nil, zero value otherwise.

### GetBccOk

`func (o *SendEmailRequest) GetBccOk() (*[]string, bool)`

GetBccOk returns a tuple with the Bcc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBcc

`func (o *SendEmailRequest) SetBcc(v []string)`

SetBcc sets Bcc field to given value.

### HasBcc

`func (o *SendEmailRequest) HasBcc() bool`

HasBcc returns a boolean if a field has been set.

### GetSubject

`func (o *SendEmailRequest) GetSubject() string`

GetSubject returns the Subject field if non-nil, zero value otherwise.

### GetSubjectOk

`func (o *SendEmailRequest) GetSubjectOk() (*string, bool)`

GetSubjectOk returns a tuple with the Subject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubject

`func (o *SendEmailRequest) SetSubject(v string)`

SetSubject sets Subject field to given value.


### GetBody

`func (o *SendEmailRequest) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *SendEmailRequest) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *SendEmailRequest) SetBody(v string)`

SetBody sets Body field to given value.


### GetHtml

`func (o *SendEmailRequest) GetHtml() bool`

GetHtml returns the Html field if non-nil, zero value otherwise.

### GetHtmlOk

`func (o *SendEmailRequest) GetHtmlOk() (*bool, bool)`

GetHtmlOk returns a tuple with the Html field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHtml

`func (o *SendEmailRequest) SetHtml(v bool)`

SetHtml sets Html field to given value.

### HasHtml

`func (o *SendEmailRequest) HasHtml() bool`

HasHtml returns a boolean if a field has been set.

### GetAttachments

`func (o *SendEmailRequest) GetAttachments() []AttachmentInput`

GetAttachments returns the Attachments field if non-nil, zero value otherwise.

### GetAttachmentsOk

`func (o *SendEmailRequest) GetAttachmentsOk() (*[]AttachmentInput, bool)`

GetAttachmentsOk returns a tuple with the Attachments field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttachments

`func (o *SendEmailRequest) SetAttachments(v []AttachmentInput)`

SetAttachments sets Attachments field to given value.

### HasAttachments

`func (o *SendEmailRequest) HasAttachments() bool`

HasAttachments returns a boolean if a field has been set.

### GetInReplyTo

`func (o *SendEmailRequest) GetInReplyTo() string`

GetInReplyTo returns the InReplyTo field if non-nil, zero value otherwise.

### GetInReplyToOk

`func (o *SendEmailRequest) GetInReplyToOk() (*string, bool)`

GetInReplyToOk returns a tuple with the InReplyTo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInReplyTo

`func (o *SendEmailRequest) SetInReplyTo(v string)`

SetInReplyTo sets InReplyTo field to given value.

### HasInReplyTo

`func (o *SendEmailRequest) HasInReplyTo() bool`

HasInReplyTo returns a boolean if a field has been set.

### GetReferences

`func (o *SendEmailRequest) GetReferences() []string`

GetReferences returns the References field if non-nil, zero value otherwise.

### GetReferencesOk

`func (o *SendEmailRequest) GetReferencesOk() (*[]string, bool)`

GetReferencesOk returns a tuple with the References field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReferences

`func (o *SendEmailRequest) SetReferences(v []string)`

SetReferences sets References field to given value.

### HasReferences

`func (o *SendEmailRequest) HasReferences() bool`

HasReferences returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


