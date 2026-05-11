# SendChatMessageResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | **bool** |  | 
**MessageId** | **string** |  | 
**ChannelId** | Pointer to **string** |  | [optional] 
**ThreadId** | Pointer to **string** |  | [optional] 
**Provider** | **string** |  | 
**Error** | Pointer to **string** |  | [optional] 

## Methods

### NewSendChatMessageResponse

`func NewSendChatMessageResponse(success bool, messageId string, provider string, ) *SendChatMessageResponse`

NewSendChatMessageResponse instantiates a new SendChatMessageResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSendChatMessageResponseWithDefaults

`func NewSendChatMessageResponseWithDefaults() *SendChatMessageResponse`

NewSendChatMessageResponseWithDefaults instantiates a new SendChatMessageResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *SendChatMessageResponse) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *SendChatMessageResponse) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *SendChatMessageResponse) SetSuccess(v bool)`

SetSuccess sets Success field to given value.


### GetMessageId

`func (o *SendChatMessageResponse) GetMessageId() string`

GetMessageId returns the MessageId field if non-nil, zero value otherwise.

### GetMessageIdOk

`func (o *SendChatMessageResponse) GetMessageIdOk() (*string, bool)`

GetMessageIdOk returns a tuple with the MessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageId

`func (o *SendChatMessageResponse) SetMessageId(v string)`

SetMessageId sets MessageId field to given value.


### GetChannelId

`func (o *SendChatMessageResponse) GetChannelId() string`

GetChannelId returns the ChannelId field if non-nil, zero value otherwise.

### GetChannelIdOk

`func (o *SendChatMessageResponse) GetChannelIdOk() (*string, bool)`

GetChannelIdOk returns a tuple with the ChannelId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChannelId

`func (o *SendChatMessageResponse) SetChannelId(v string)`

SetChannelId sets ChannelId field to given value.

### HasChannelId

`func (o *SendChatMessageResponse) HasChannelId() bool`

HasChannelId returns a boolean if a field has been set.

### GetThreadId

`func (o *SendChatMessageResponse) GetThreadId() string`

GetThreadId returns the ThreadId field if non-nil, zero value otherwise.

### GetThreadIdOk

`func (o *SendChatMessageResponse) GetThreadIdOk() (*string, bool)`

GetThreadIdOk returns a tuple with the ThreadId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetThreadId

`func (o *SendChatMessageResponse) SetThreadId(v string)`

SetThreadId sets ThreadId field to given value.

### HasThreadId

`func (o *SendChatMessageResponse) HasThreadId() bool`

HasThreadId returns a boolean if a field has been set.

### GetProvider

`func (o *SendChatMessageResponse) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *SendChatMessageResponse) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *SendChatMessageResponse) SetProvider(v string)`

SetProvider sets Provider field to given value.


### GetError

`func (o *SendChatMessageResponse) GetError() string`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *SendChatMessageResponse) GetErrorOk() (*string, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *SendChatMessageResponse) SetError(v string)`

SetError sets Error field to given value.

### HasError

`func (o *SendChatMessageResponse) HasError() bool`

HasError returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


