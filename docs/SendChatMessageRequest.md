# SendChatMessageRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AccountId** | Pointer to **string** |  | [optional] 
**Channel** | **string** | Channel or DM id (provider-scoped). | 
**Text** | **string** |  | 
**ThreadId** | Pointer to **string** |  | [optional] 
**Blocks** | Pointer to **[]map[string]interface{}** | Provider-specific rich-message blocks. | [optional] 

## Methods

### NewSendChatMessageRequest

`func NewSendChatMessageRequest(channel string, text string, ) *SendChatMessageRequest`

NewSendChatMessageRequest instantiates a new SendChatMessageRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSendChatMessageRequestWithDefaults

`func NewSendChatMessageRequestWithDefaults() *SendChatMessageRequest`

NewSendChatMessageRequestWithDefaults instantiates a new SendChatMessageRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAccountId

`func (o *SendChatMessageRequest) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *SendChatMessageRequest) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *SendChatMessageRequest) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *SendChatMessageRequest) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.

### GetChannel

`func (o *SendChatMessageRequest) GetChannel() string`

GetChannel returns the Channel field if non-nil, zero value otherwise.

### GetChannelOk

`func (o *SendChatMessageRequest) GetChannelOk() (*string, bool)`

GetChannelOk returns a tuple with the Channel field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChannel

`func (o *SendChatMessageRequest) SetChannel(v string)`

SetChannel sets Channel field to given value.


### GetText

`func (o *SendChatMessageRequest) GetText() string`

GetText returns the Text field if non-nil, zero value otherwise.

### GetTextOk

`func (o *SendChatMessageRequest) GetTextOk() (*string, bool)`

GetTextOk returns a tuple with the Text field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetText

`func (o *SendChatMessageRequest) SetText(v string)`

SetText sets Text field to given value.


### GetThreadId

`func (o *SendChatMessageRequest) GetThreadId() string`

GetThreadId returns the ThreadId field if non-nil, zero value otherwise.

### GetThreadIdOk

`func (o *SendChatMessageRequest) GetThreadIdOk() (*string, bool)`

GetThreadIdOk returns a tuple with the ThreadId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetThreadId

`func (o *SendChatMessageRequest) SetThreadId(v string)`

SetThreadId sets ThreadId field to given value.

### HasThreadId

`func (o *SendChatMessageRequest) HasThreadId() bool`

HasThreadId returns a boolean if a field has been set.

### GetBlocks

`func (o *SendChatMessageRequest) GetBlocks() []map[string]interface{}`

GetBlocks returns the Blocks field if non-nil, zero value otherwise.

### GetBlocksOk

`func (o *SendChatMessageRequest) GetBlocksOk() (*[]map[string]interface{}, bool)`

GetBlocksOk returns a tuple with the Blocks field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBlocks

`func (o *SendChatMessageRequest) SetBlocks(v []map[string]interface{})`

SetBlocks sets Blocks field to given value.

### HasBlocks

`func (o *SendChatMessageRequest) HasBlocks() bool`

HasBlocks returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


