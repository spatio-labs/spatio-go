# AgentListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Agents** | [**[]Agent**](Agent.md) |  | 
**HasMore** | Pointer to **bool** |  | [optional] 
**Total** | Pointer to **int32** |  | [optional] 
**TotalCount** | Pointer to **int32** |  | [optional] 

## Methods

### NewAgentListResponse

`func NewAgentListResponse(agents []Agent, ) *AgentListResponse`

NewAgentListResponse instantiates a new AgentListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAgentListResponseWithDefaults

`func NewAgentListResponseWithDefaults() *AgentListResponse`

NewAgentListResponseWithDefaults instantiates a new AgentListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAgents

`func (o *AgentListResponse) GetAgents() []Agent`

GetAgents returns the Agents field if non-nil, zero value otherwise.

### GetAgentsOk

`func (o *AgentListResponse) GetAgentsOk() (*[]Agent, bool)`

GetAgentsOk returns a tuple with the Agents field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAgents

`func (o *AgentListResponse) SetAgents(v []Agent)`

SetAgents sets Agents field to given value.


### SetAgentsNil

`func (o *AgentListResponse) SetAgentsNil(b bool)`

 SetAgentsNil sets the value for Agents to be an explicit nil

### UnsetAgents
`func (o *AgentListResponse) UnsetAgents()`

UnsetAgents ensures that no value is present for Agents, not even an explicit nil
### GetHasMore

`func (o *AgentListResponse) GetHasMore() bool`

GetHasMore returns the HasMore field if non-nil, zero value otherwise.

### GetHasMoreOk

`func (o *AgentListResponse) GetHasMoreOk() (*bool, bool)`

GetHasMoreOk returns a tuple with the HasMore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasMore

`func (o *AgentListResponse) SetHasMore(v bool)`

SetHasMore sets HasMore field to given value.

### HasHasMore

`func (o *AgentListResponse) HasHasMore() bool`

HasHasMore returns a boolean if a field has been set.

### GetTotal

`func (o *AgentListResponse) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *AgentListResponse) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *AgentListResponse) SetTotal(v int32)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *AgentListResponse) HasTotal() bool`

HasTotal returns a boolean if a field has been set.

### GetTotalCount

`func (o *AgentListResponse) GetTotalCount() int32`

GetTotalCount returns the TotalCount field if non-nil, zero value otherwise.

### GetTotalCountOk

`func (o *AgentListResponse) GetTotalCountOk() (*int32, bool)`

GetTotalCountOk returns a tuple with the TotalCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalCount

`func (o *AgentListResponse) SetTotalCount(v int32)`

SetTotalCount sets TotalCount field to given value.

### HasTotalCount

`func (o *AgentListResponse) HasTotalCount() bool`

HasTotalCount returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


