# Email

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**ThreadId** | Pointer to **string** |  | [optional] 
**Provider** | Pointer to **string** |  | [optional] 
**AccountId** | Pointer to **string** |  | [optional] 
**Subject** | **string** |  | 
**From** | **string** |  | 
**To** | **[]string** |  | 
**Cc** | Pointer to **[]string** |  | [optional] 
**Bcc** | Pointer to **[]string** |  | [optional] 
**Body** | **string** |  | 
**Html** | **bool** | &#x60;true&#x60; when &#x60;body&#x60; contains HTML, &#x60;false&#x60; for plain text.  | 
**Date** | **time.Time** |  | 
**Labels** | Pointer to **[]string** |  | [optional] 
**IsRead** | **bool** |  | 
**IsStarred** | **bool** |  | 
**Attachments** | Pointer to [**[]AttachmentMeta**](AttachmentMeta.md) |  | [optional] 
**Snippet** | Pointer to **string** |  | [optional] 
**MessageId** | Pointer to **string** | RFC 5322 Message-ID header. | [optional] 
**InReplyTo** | Pointer to **string** | RFC 5322 In-Reply-To header — the parent message id this message is a reply to.  | [optional] 
**References** | Pointer to **[]string** | RFC 5322 References header (ancestor chain). | [optional] 

## Methods

### NewEmail

`func NewEmail(id string, subject string, from string, to []string, body string, html bool, date time.Time, isRead bool, isStarred bool, ) *Email`

NewEmail instantiates a new Email object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEmailWithDefaults

`func NewEmailWithDefaults() *Email`

NewEmailWithDefaults instantiates a new Email object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Email) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Email) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Email) SetId(v string)`

SetId sets Id field to given value.


### GetThreadId

`func (o *Email) GetThreadId() string`

GetThreadId returns the ThreadId field if non-nil, zero value otherwise.

### GetThreadIdOk

`func (o *Email) GetThreadIdOk() (*string, bool)`

GetThreadIdOk returns a tuple with the ThreadId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetThreadId

`func (o *Email) SetThreadId(v string)`

SetThreadId sets ThreadId field to given value.

### HasThreadId

`func (o *Email) HasThreadId() bool`

HasThreadId returns a boolean if a field has been set.

### GetProvider

`func (o *Email) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *Email) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *Email) SetProvider(v string)`

SetProvider sets Provider field to given value.

### HasProvider

`func (o *Email) HasProvider() bool`

HasProvider returns a boolean if a field has been set.

### GetAccountId

`func (o *Email) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *Email) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *Email) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *Email) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.

### GetSubject

`func (o *Email) GetSubject() string`

GetSubject returns the Subject field if non-nil, zero value otherwise.

### GetSubjectOk

`func (o *Email) GetSubjectOk() (*string, bool)`

GetSubjectOk returns a tuple with the Subject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubject

`func (o *Email) SetSubject(v string)`

SetSubject sets Subject field to given value.


### GetFrom

`func (o *Email) GetFrom() string`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *Email) GetFromOk() (*string, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *Email) SetFrom(v string)`

SetFrom sets From field to given value.


### GetTo

`func (o *Email) GetTo() []string`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *Email) GetToOk() (*[]string, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *Email) SetTo(v []string)`

SetTo sets To field to given value.


### GetCc

`func (o *Email) GetCc() []string`

GetCc returns the Cc field if non-nil, zero value otherwise.

### GetCcOk

`func (o *Email) GetCcOk() (*[]string, bool)`

GetCcOk returns a tuple with the Cc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCc

`func (o *Email) SetCc(v []string)`

SetCc sets Cc field to given value.

### HasCc

`func (o *Email) HasCc() bool`

HasCc returns a boolean if a field has been set.

### GetBcc

`func (o *Email) GetBcc() []string`

GetBcc returns the Bcc field if non-nil, zero value otherwise.

### GetBccOk

`func (o *Email) GetBccOk() (*[]string, bool)`

GetBccOk returns a tuple with the Bcc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBcc

`func (o *Email) SetBcc(v []string)`

SetBcc sets Bcc field to given value.

### HasBcc

`func (o *Email) HasBcc() bool`

HasBcc returns a boolean if a field has been set.

### GetBody

`func (o *Email) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *Email) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *Email) SetBody(v string)`

SetBody sets Body field to given value.


### GetHtml

`func (o *Email) GetHtml() bool`

GetHtml returns the Html field if non-nil, zero value otherwise.

### GetHtmlOk

`func (o *Email) GetHtmlOk() (*bool, bool)`

GetHtmlOk returns a tuple with the Html field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHtml

`func (o *Email) SetHtml(v bool)`

SetHtml sets Html field to given value.


### GetDate

`func (o *Email) GetDate() time.Time`

GetDate returns the Date field if non-nil, zero value otherwise.

### GetDateOk

`func (o *Email) GetDateOk() (*time.Time, bool)`

GetDateOk returns a tuple with the Date field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDate

`func (o *Email) SetDate(v time.Time)`

SetDate sets Date field to given value.


### GetLabels

`func (o *Email) GetLabels() []string`

GetLabels returns the Labels field if non-nil, zero value otherwise.

### GetLabelsOk

`func (o *Email) GetLabelsOk() (*[]string, bool)`

GetLabelsOk returns a tuple with the Labels field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabels

`func (o *Email) SetLabels(v []string)`

SetLabels sets Labels field to given value.

### HasLabels

`func (o *Email) HasLabels() bool`

HasLabels returns a boolean if a field has been set.

### GetIsRead

`func (o *Email) GetIsRead() bool`

GetIsRead returns the IsRead field if non-nil, zero value otherwise.

### GetIsReadOk

`func (o *Email) GetIsReadOk() (*bool, bool)`

GetIsReadOk returns a tuple with the IsRead field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsRead

`func (o *Email) SetIsRead(v bool)`

SetIsRead sets IsRead field to given value.


### GetIsStarred

`func (o *Email) GetIsStarred() bool`

GetIsStarred returns the IsStarred field if non-nil, zero value otherwise.

### GetIsStarredOk

`func (o *Email) GetIsStarredOk() (*bool, bool)`

GetIsStarredOk returns a tuple with the IsStarred field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsStarred

`func (o *Email) SetIsStarred(v bool)`

SetIsStarred sets IsStarred field to given value.


### GetAttachments

`func (o *Email) GetAttachments() []AttachmentMeta`

GetAttachments returns the Attachments field if non-nil, zero value otherwise.

### GetAttachmentsOk

`func (o *Email) GetAttachmentsOk() (*[]AttachmentMeta, bool)`

GetAttachmentsOk returns a tuple with the Attachments field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttachments

`func (o *Email) SetAttachments(v []AttachmentMeta)`

SetAttachments sets Attachments field to given value.

### HasAttachments

`func (o *Email) HasAttachments() bool`

HasAttachments returns a boolean if a field has been set.

### GetSnippet

`func (o *Email) GetSnippet() string`

GetSnippet returns the Snippet field if non-nil, zero value otherwise.

### GetSnippetOk

`func (o *Email) GetSnippetOk() (*string, bool)`

GetSnippetOk returns a tuple with the Snippet field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSnippet

`func (o *Email) SetSnippet(v string)`

SetSnippet sets Snippet field to given value.

### HasSnippet

`func (o *Email) HasSnippet() bool`

HasSnippet returns a boolean if a field has been set.

### GetMessageId

`func (o *Email) GetMessageId() string`

GetMessageId returns the MessageId field if non-nil, zero value otherwise.

### GetMessageIdOk

`func (o *Email) GetMessageIdOk() (*string, bool)`

GetMessageIdOk returns a tuple with the MessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageId

`func (o *Email) SetMessageId(v string)`

SetMessageId sets MessageId field to given value.

### HasMessageId

`func (o *Email) HasMessageId() bool`

HasMessageId returns a boolean if a field has been set.

### GetInReplyTo

`func (o *Email) GetInReplyTo() string`

GetInReplyTo returns the InReplyTo field if non-nil, zero value otherwise.

### GetInReplyToOk

`func (o *Email) GetInReplyToOk() (*string, bool)`

GetInReplyToOk returns a tuple with the InReplyTo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInReplyTo

`func (o *Email) SetInReplyTo(v string)`

SetInReplyTo sets InReplyTo field to given value.

### HasInReplyTo

`func (o *Email) HasInReplyTo() bool`

HasInReplyTo returns a boolean if a field has been set.

### GetReferences

`func (o *Email) GetReferences() []string`

GetReferences returns the References field if non-nil, zero value otherwise.

### GetReferencesOk

`func (o *Email) GetReferencesOk() (*[]string, bool)`

GetReferencesOk returns a tuple with the References field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReferences

`func (o *Email) SetReferences(v []string)`

SetReferences sets References field to given value.

### HasReferences

`func (o *Email) HasReferences() bool`

HasReferences returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


