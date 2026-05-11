# InboxItem

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Category** | **string** |  | 
**Title** | Pointer to **string** |  | [optional] 
**Snippet** | Pointer to **string** |  | [optional] 
**Source** | Pointer to **string** |  | [optional] 
**SourceId** | Pointer to **string** |  | [optional] 
**AccountId** | Pointer to **NullableString** |  | [optional] 
**IsRead** | Pointer to **bool** |  | [optional] 
**IsMention** | Pointer to **bool** |  | [optional] 
**Timestamp** | Pointer to **time.Time** |  | [optional] 
**Metadata** | Pointer to **map[string]interface{}** |  | [optional] 

## Methods

### NewInboxItem

`func NewInboxItem(id string, category string, ) *InboxItem`

NewInboxItem instantiates a new InboxItem object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInboxItemWithDefaults

`func NewInboxItemWithDefaults() *InboxItem`

NewInboxItemWithDefaults instantiates a new InboxItem object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *InboxItem) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *InboxItem) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *InboxItem) SetId(v string)`

SetId sets Id field to given value.


### GetCategory

`func (o *InboxItem) GetCategory() string`

GetCategory returns the Category field if non-nil, zero value otherwise.

### GetCategoryOk

`func (o *InboxItem) GetCategoryOk() (*string, bool)`

GetCategoryOk returns a tuple with the Category field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCategory

`func (o *InboxItem) SetCategory(v string)`

SetCategory sets Category field to given value.


### GetTitle

`func (o *InboxItem) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *InboxItem) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *InboxItem) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *InboxItem) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### GetSnippet

`func (o *InboxItem) GetSnippet() string`

GetSnippet returns the Snippet field if non-nil, zero value otherwise.

### GetSnippetOk

`func (o *InboxItem) GetSnippetOk() (*string, bool)`

GetSnippetOk returns a tuple with the Snippet field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSnippet

`func (o *InboxItem) SetSnippet(v string)`

SetSnippet sets Snippet field to given value.

### HasSnippet

`func (o *InboxItem) HasSnippet() bool`

HasSnippet returns a boolean if a field has been set.

### GetSource

`func (o *InboxItem) GetSource() string`

GetSource returns the Source field if non-nil, zero value otherwise.

### GetSourceOk

`func (o *InboxItem) GetSourceOk() (*string, bool)`

GetSourceOk returns a tuple with the Source field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSource

`func (o *InboxItem) SetSource(v string)`

SetSource sets Source field to given value.

### HasSource

`func (o *InboxItem) HasSource() bool`

HasSource returns a boolean if a field has been set.

### GetSourceId

`func (o *InboxItem) GetSourceId() string`

GetSourceId returns the SourceId field if non-nil, zero value otherwise.

### GetSourceIdOk

`func (o *InboxItem) GetSourceIdOk() (*string, bool)`

GetSourceIdOk returns a tuple with the SourceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceId

`func (o *InboxItem) SetSourceId(v string)`

SetSourceId sets SourceId field to given value.

### HasSourceId

`func (o *InboxItem) HasSourceId() bool`

HasSourceId returns a boolean if a field has been set.

### GetAccountId

`func (o *InboxItem) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *InboxItem) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *InboxItem) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *InboxItem) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.

### SetAccountIdNil

`func (o *InboxItem) SetAccountIdNil(b bool)`

 SetAccountIdNil sets the value for AccountId to be an explicit nil

### UnsetAccountId
`func (o *InboxItem) UnsetAccountId()`

UnsetAccountId ensures that no value is present for AccountId, not even an explicit nil
### GetIsRead

`func (o *InboxItem) GetIsRead() bool`

GetIsRead returns the IsRead field if non-nil, zero value otherwise.

### GetIsReadOk

`func (o *InboxItem) GetIsReadOk() (*bool, bool)`

GetIsReadOk returns a tuple with the IsRead field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsRead

`func (o *InboxItem) SetIsRead(v bool)`

SetIsRead sets IsRead field to given value.

### HasIsRead

`func (o *InboxItem) HasIsRead() bool`

HasIsRead returns a boolean if a field has been set.

### GetIsMention

`func (o *InboxItem) GetIsMention() bool`

GetIsMention returns the IsMention field if non-nil, zero value otherwise.

### GetIsMentionOk

`func (o *InboxItem) GetIsMentionOk() (*bool, bool)`

GetIsMentionOk returns a tuple with the IsMention field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsMention

`func (o *InboxItem) SetIsMention(v bool)`

SetIsMention sets IsMention field to given value.

### HasIsMention

`func (o *InboxItem) HasIsMention() bool`

HasIsMention returns a boolean if a field has been set.

### GetTimestamp

`func (o *InboxItem) GetTimestamp() time.Time`

GetTimestamp returns the Timestamp field if non-nil, zero value otherwise.

### GetTimestampOk

`func (o *InboxItem) GetTimestampOk() (*time.Time, bool)`

GetTimestampOk returns a tuple with the Timestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimestamp

`func (o *InboxItem) SetTimestamp(v time.Time)`

SetTimestamp sets Timestamp field to given value.

### HasTimestamp

`func (o *InboxItem) HasTimestamp() bool`

HasTimestamp returns a boolean if a field has been set.

### GetMetadata

`func (o *InboxItem) GetMetadata() map[string]interface{}`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *InboxItem) GetMetadataOk() (*map[string]interface{}, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *InboxItem) SetMetadata(v map[string]interface{})`

SetMetadata sets Metadata field to given value.

### HasMetadata

`func (o *InboxItem) HasMetadata() bool`

HasMetadata returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


