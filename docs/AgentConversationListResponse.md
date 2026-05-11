# AgentConversationListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Conversations** | [**[]AgentConversation**](AgentConversation.md) |  | 
**Total** | Pointer to **int32** |  | [optional] 

## Methods

### NewAgentConversationListResponse

`func NewAgentConversationListResponse(conversations []AgentConversation, ) *AgentConversationListResponse`

NewAgentConversationListResponse instantiates a new AgentConversationListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAgentConversationListResponseWithDefaults

`func NewAgentConversationListResponseWithDefaults() *AgentConversationListResponse`

NewAgentConversationListResponseWithDefaults instantiates a new AgentConversationListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetConversations

`func (o *AgentConversationListResponse) GetConversations() []AgentConversation`

GetConversations returns the Conversations field if non-nil, zero value otherwise.

### GetConversationsOk

`func (o *AgentConversationListResponse) GetConversationsOk() (*[]AgentConversation, bool)`

GetConversationsOk returns a tuple with the Conversations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConversations

`func (o *AgentConversationListResponse) SetConversations(v []AgentConversation)`

SetConversations sets Conversations field to given value.


### GetTotal

`func (o *AgentConversationListResponse) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *AgentConversationListResponse) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *AgentConversationListResponse) SetTotal(v int32)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *AgentConversationListResponse) HasTotal() bool`

HasTotal returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


