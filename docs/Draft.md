# Draft

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**MessageId** | **string** |  | 
**ThreadId** | Pointer to **string** |  | [optional] 
**To** | Pointer to **[]string** |  | [optional] 
**Cc** | Pointer to **[]string** |  | [optional] 
**Bcc** | Pointer to **[]string** |  | [optional] 
**Subject** | Pointer to **string** |  | [optional] 
**Body** | Pointer to **string** |  | [optional] 
**Html** | **bool** |  | 
**Attachments** | Pointer to [**[]AttachmentMeta**](AttachmentMeta.md) |  | [optional] 
**CreatedAt** | **time.Time** |  | 
**UpdatedAt** | **time.Time** |  | 

## Methods

### NewDraft

`func NewDraft(id string, messageId string, html bool, createdAt time.Time, updatedAt time.Time, ) *Draft`

NewDraft instantiates a new Draft object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDraftWithDefaults

`func NewDraftWithDefaults() *Draft`

NewDraftWithDefaults instantiates a new Draft object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Draft) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Draft) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Draft) SetId(v string)`

SetId sets Id field to given value.


### GetMessageId

`func (o *Draft) GetMessageId() string`

GetMessageId returns the MessageId field if non-nil, zero value otherwise.

### GetMessageIdOk

`func (o *Draft) GetMessageIdOk() (*string, bool)`

GetMessageIdOk returns a tuple with the MessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageId

`func (o *Draft) SetMessageId(v string)`

SetMessageId sets MessageId field to given value.


### GetThreadId

`func (o *Draft) GetThreadId() string`

GetThreadId returns the ThreadId field if non-nil, zero value otherwise.

### GetThreadIdOk

`func (o *Draft) GetThreadIdOk() (*string, bool)`

GetThreadIdOk returns a tuple with the ThreadId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetThreadId

`func (o *Draft) SetThreadId(v string)`

SetThreadId sets ThreadId field to given value.

### HasThreadId

`func (o *Draft) HasThreadId() bool`

HasThreadId returns a boolean if a field has been set.

### GetTo

`func (o *Draft) GetTo() []string`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *Draft) GetToOk() (*[]string, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *Draft) SetTo(v []string)`

SetTo sets To field to given value.

### HasTo

`func (o *Draft) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetCc

`func (o *Draft) GetCc() []string`

GetCc returns the Cc field if non-nil, zero value otherwise.

### GetCcOk

`func (o *Draft) GetCcOk() (*[]string, bool)`

GetCcOk returns a tuple with the Cc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCc

`func (o *Draft) SetCc(v []string)`

SetCc sets Cc field to given value.

### HasCc

`func (o *Draft) HasCc() bool`

HasCc returns a boolean if a field has been set.

### GetBcc

`func (o *Draft) GetBcc() []string`

GetBcc returns the Bcc field if non-nil, zero value otherwise.

### GetBccOk

`func (o *Draft) GetBccOk() (*[]string, bool)`

GetBccOk returns a tuple with the Bcc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBcc

`func (o *Draft) SetBcc(v []string)`

SetBcc sets Bcc field to given value.

### HasBcc

`func (o *Draft) HasBcc() bool`

HasBcc returns a boolean if a field has been set.

### GetSubject

`func (o *Draft) GetSubject() string`

GetSubject returns the Subject field if non-nil, zero value otherwise.

### GetSubjectOk

`func (o *Draft) GetSubjectOk() (*string, bool)`

GetSubjectOk returns a tuple with the Subject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubject

`func (o *Draft) SetSubject(v string)`

SetSubject sets Subject field to given value.

### HasSubject

`func (o *Draft) HasSubject() bool`

HasSubject returns a boolean if a field has been set.

### GetBody

`func (o *Draft) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *Draft) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *Draft) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *Draft) HasBody() bool`

HasBody returns a boolean if a field has been set.

### GetHtml

`func (o *Draft) GetHtml() bool`

GetHtml returns the Html field if non-nil, zero value otherwise.

### GetHtmlOk

`func (o *Draft) GetHtmlOk() (*bool, bool)`

GetHtmlOk returns a tuple with the Html field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHtml

`func (o *Draft) SetHtml(v bool)`

SetHtml sets Html field to given value.


### GetAttachments

`func (o *Draft) GetAttachments() []AttachmentMeta`

GetAttachments returns the Attachments field if non-nil, zero value otherwise.

### GetAttachmentsOk

`func (o *Draft) GetAttachmentsOk() (*[]AttachmentMeta, bool)`

GetAttachmentsOk returns a tuple with the Attachments field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttachments

`func (o *Draft) SetAttachments(v []AttachmentMeta)`

SetAttachments sets Attachments field to given value.

### HasAttachments

`func (o *Draft) HasAttachments() bool`

HasAttachments returns a boolean if a field has been set.

### GetCreatedAt

`func (o *Draft) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Draft) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Draft) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *Draft) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *Draft) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *Draft) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


