# ReplyEmailRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AccountId** | Pointer to **string** |  | [optional] 
**To** | Pointer to **[]string** |  | [optional] 
**Cc** | Pointer to **[]string** |  | [optional] 
**Bcc** | Pointer to **[]string** |  | [optional] 
**Body** | **string** |  | 
**Html** | Pointer to **bool** |  | [optional] 
**Attachments** | Pointer to [**[]AttachmentInput**](AttachmentInput.md) |  | [optional] 

## Methods

### NewReplyEmailRequest

`func NewReplyEmailRequest(body string, ) *ReplyEmailRequest`

NewReplyEmailRequest instantiates a new ReplyEmailRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewReplyEmailRequestWithDefaults

`func NewReplyEmailRequestWithDefaults() *ReplyEmailRequest`

NewReplyEmailRequestWithDefaults instantiates a new ReplyEmailRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAccountId

`func (o *ReplyEmailRequest) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *ReplyEmailRequest) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *ReplyEmailRequest) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *ReplyEmailRequest) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.

### GetTo

`func (o *ReplyEmailRequest) GetTo() []string`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *ReplyEmailRequest) GetToOk() (*[]string, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *ReplyEmailRequest) SetTo(v []string)`

SetTo sets To field to given value.

### HasTo

`func (o *ReplyEmailRequest) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetCc

`func (o *ReplyEmailRequest) GetCc() []string`

GetCc returns the Cc field if non-nil, zero value otherwise.

### GetCcOk

`func (o *ReplyEmailRequest) GetCcOk() (*[]string, bool)`

GetCcOk returns a tuple with the Cc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCc

`func (o *ReplyEmailRequest) SetCc(v []string)`

SetCc sets Cc field to given value.

### HasCc

`func (o *ReplyEmailRequest) HasCc() bool`

HasCc returns a boolean if a field has been set.

### GetBcc

`func (o *ReplyEmailRequest) GetBcc() []string`

GetBcc returns the Bcc field if non-nil, zero value otherwise.

### GetBccOk

`func (o *ReplyEmailRequest) GetBccOk() (*[]string, bool)`

GetBccOk returns a tuple with the Bcc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBcc

`func (o *ReplyEmailRequest) SetBcc(v []string)`

SetBcc sets Bcc field to given value.

### HasBcc

`func (o *ReplyEmailRequest) HasBcc() bool`

HasBcc returns a boolean if a field has been set.

### GetBody

`func (o *ReplyEmailRequest) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *ReplyEmailRequest) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *ReplyEmailRequest) SetBody(v string)`

SetBody sets Body field to given value.


### GetHtml

`func (o *ReplyEmailRequest) GetHtml() bool`

GetHtml returns the Html field if non-nil, zero value otherwise.

### GetHtmlOk

`func (o *ReplyEmailRequest) GetHtmlOk() (*bool, bool)`

GetHtmlOk returns a tuple with the Html field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHtml

`func (o *ReplyEmailRequest) SetHtml(v bool)`

SetHtml sets Html field to given value.

### HasHtml

`func (o *ReplyEmailRequest) HasHtml() bool`

HasHtml returns a boolean if a field has been set.

### GetAttachments

`func (o *ReplyEmailRequest) GetAttachments() []AttachmentInput`

GetAttachments returns the Attachments field if non-nil, zero value otherwise.

### GetAttachmentsOk

`func (o *ReplyEmailRequest) GetAttachmentsOk() (*[]AttachmentInput, bool)`

GetAttachmentsOk returns a tuple with the Attachments field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttachments

`func (o *ReplyEmailRequest) SetAttachments(v []AttachmentInput)`

SetAttachments sets Attachments field to given value.

### HasAttachments

`func (o *ReplyEmailRequest) HasAttachments() bool`

HasAttachments returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


