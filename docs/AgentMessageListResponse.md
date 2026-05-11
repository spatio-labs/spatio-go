# AgentMessageListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Messages** | [**[]AgentMessage**](AgentMessage.md) |  | 
**Total** | Pointer to **int32** |  | [optional] 

## Methods

### NewAgentMessageListResponse

`func NewAgentMessageListResponse(messages []AgentMessage, ) *AgentMessageListResponse`

NewAgentMessageListResponse instantiates a new AgentMessageListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAgentMessageListResponseWithDefaults

`func NewAgentMessageListResponseWithDefaults() *AgentMessageListResponse`

NewAgentMessageListResponseWithDefaults instantiates a new AgentMessageListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMessages

`func (o *AgentMessageListResponse) GetMessages() []AgentMessage`

GetMessages returns the Messages field if non-nil, zero value otherwise.

### GetMessagesOk

`func (o *AgentMessageListResponse) GetMessagesOk() (*[]AgentMessage, bool)`

GetMessagesOk returns a tuple with the Messages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessages

`func (o *AgentMessageListResponse) SetMessages(v []AgentMessage)`

SetMessages sets Messages field to given value.


### GetTotal

`func (o *AgentMessageListResponse) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *AgentMessageListResponse) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *AgentMessageListResponse) SetTotal(v int32)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *AgentMessageListResponse) HasTotal() bool`

HasTotal returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


