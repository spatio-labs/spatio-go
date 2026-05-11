# Conversation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**UserId** | **string** |  | 
**Title** | **string** |  | 
**Context** | Pointer to **NullableString** | Free-form context tag (e.g. &#x60;sidebar:sheets:entity:&lt;id&gt;&#x60;). | [optional] 
**Cwd** | Pointer to **NullableString** |  | [optional] 
**SessionId** | Pointer to **NullableString** |  | [optional] 
**Pinned** | Pointer to **bool** |  | [optional] 
**LastMessageAt** | Pointer to **NullableTime** |  | [optional] 
**MessageCount** | Pointer to **int32** |  | [optional] 
**IsActive** | Pointer to **bool** |  | [optional] 
**Metadata** | Pointer to **map[string]interface{}** |  | [optional] 
**CreatedAt** | Pointer to **time.Time** |  | [optional] 
**UpdatedAt** | Pointer to **time.Time** |  | [optional] 

## Methods

### NewConversation

`func NewConversation(id string, userId string, title string, ) *Conversation`

NewConversation instantiates a new Conversation object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewConversationWithDefaults

`func NewConversationWithDefaults() *Conversation`

NewConversationWithDefaults instantiates a new Conversation object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Conversation) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Conversation) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Conversation) SetId(v string)`

SetId sets Id field to given value.


### GetUserId

`func (o *Conversation) GetUserId() string`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *Conversation) GetUserIdOk() (*string, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *Conversation) SetUserId(v string)`

SetUserId sets UserId field to given value.


### GetTitle

`func (o *Conversation) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *Conversation) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *Conversation) SetTitle(v string)`

SetTitle sets Title field to given value.


### GetContext

`func (o *Conversation) GetContext() string`

GetContext returns the Context field if non-nil, zero value otherwise.

### GetContextOk

`func (o *Conversation) GetContextOk() (*string, bool)`

GetContextOk returns a tuple with the Context field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContext

`func (o *Conversation) SetContext(v string)`

SetContext sets Context field to given value.

### HasContext

`func (o *Conversation) HasContext() bool`

HasContext returns a boolean if a field has been set.

### SetContextNil

`func (o *Conversation) SetContextNil(b bool)`

 SetContextNil sets the value for Context to be an explicit nil

### UnsetContext
`func (o *Conversation) UnsetContext()`

UnsetContext ensures that no value is present for Context, not even an explicit nil
### GetCwd

`func (o *Conversation) GetCwd() string`

GetCwd returns the Cwd field if non-nil, zero value otherwise.

### GetCwdOk

`func (o *Conversation) GetCwdOk() (*string, bool)`

GetCwdOk returns a tuple with the Cwd field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCwd

`func (o *Conversation) SetCwd(v string)`

SetCwd sets Cwd field to given value.

### HasCwd

`func (o *Conversation) HasCwd() bool`

HasCwd returns a boolean if a field has been set.

### SetCwdNil

`func (o *Conversation) SetCwdNil(b bool)`

 SetCwdNil sets the value for Cwd to be an explicit nil

### UnsetCwd
`func (o *Conversation) UnsetCwd()`

UnsetCwd ensures that no value is present for Cwd, not even an explicit nil
### GetSessionId

`func (o *Conversation) GetSessionId() string`

GetSessionId returns the SessionId field if non-nil, zero value otherwise.

### GetSessionIdOk

`func (o *Conversation) GetSessionIdOk() (*string, bool)`

GetSessionIdOk returns a tuple with the SessionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSessionId

`func (o *Conversation) SetSessionId(v string)`

SetSessionId sets SessionId field to given value.

### HasSessionId

`func (o *Conversation) HasSessionId() bool`

HasSessionId returns a boolean if a field has been set.

### SetSessionIdNil

`func (o *Conversation) SetSessionIdNil(b bool)`

 SetSessionIdNil sets the value for SessionId to be an explicit nil

### UnsetSessionId
`func (o *Conversation) UnsetSessionId()`

UnsetSessionId ensures that no value is present for SessionId, not even an explicit nil
### GetPinned

`func (o *Conversation) GetPinned() bool`

GetPinned returns the Pinned field if non-nil, zero value otherwise.

### GetPinnedOk

`func (o *Conversation) GetPinnedOk() (*bool, bool)`

GetPinnedOk returns a tuple with the Pinned field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPinned

`func (o *Conversation) SetPinned(v bool)`

SetPinned sets Pinned field to given value.

### HasPinned

`func (o *Conversation) HasPinned() bool`

HasPinned returns a boolean if a field has been set.

### GetLastMessageAt

`func (o *Conversation) GetLastMessageAt() time.Time`

GetLastMessageAt returns the LastMessageAt field if non-nil, zero value otherwise.

### GetLastMessageAtOk

`func (o *Conversation) GetLastMessageAtOk() (*time.Time, bool)`

GetLastMessageAtOk returns a tuple with the LastMessageAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastMessageAt

`func (o *Conversation) SetLastMessageAt(v time.Time)`

SetLastMessageAt sets LastMessageAt field to given value.

### HasLastMessageAt

`func (o *Conversation) HasLastMessageAt() bool`

HasLastMessageAt returns a boolean if a field has been set.

### SetLastMessageAtNil

`func (o *Conversation) SetLastMessageAtNil(b bool)`

 SetLastMessageAtNil sets the value for LastMessageAt to be an explicit nil

### UnsetLastMessageAt
`func (o *Conversation) UnsetLastMessageAt()`

UnsetLastMessageAt ensures that no value is present for LastMessageAt, not even an explicit nil
### GetMessageCount

`func (o *Conversation) GetMessageCount() int32`

GetMessageCount returns the MessageCount field if non-nil, zero value otherwise.

### GetMessageCountOk

`func (o *Conversation) GetMessageCountOk() (*int32, bool)`

GetMessageCountOk returns a tuple with the MessageCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageCount

`func (o *Conversation) SetMessageCount(v int32)`

SetMessageCount sets MessageCount field to given value.

### HasMessageCount

`func (o *Conversation) HasMessageCount() bool`

HasMessageCount returns a boolean if a field has been set.

### GetIsActive

`func (o *Conversation) GetIsActive() bool`

GetIsActive returns the IsActive field if non-nil, zero value otherwise.

### GetIsActiveOk

`func (o *Conversation) GetIsActiveOk() (*bool, bool)`

GetIsActiveOk returns a tuple with the IsActive field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsActive

`func (o *Conversation) SetIsActive(v bool)`

SetIsActive sets IsActive field to given value.

### HasIsActive

`func (o *Conversation) HasIsActive() bool`

HasIsActive returns a boolean if a field has been set.

### GetMetadata

`func (o *Conversation) GetMetadata() map[string]interface{}`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *Conversation) GetMetadataOk() (*map[string]interface{}, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *Conversation) SetMetadata(v map[string]interface{})`

SetMetadata sets Metadata field to given value.

### HasMetadata

`func (o *Conversation) HasMetadata() bool`

HasMetadata returns a boolean if a field has been set.

### GetCreatedAt

`func (o *Conversation) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Conversation) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Conversation) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *Conversation) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetUpdatedAt

`func (o *Conversation) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *Conversation) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *Conversation) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *Conversation) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


