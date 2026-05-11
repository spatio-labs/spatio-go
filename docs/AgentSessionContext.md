# AgentSessionContext

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**User** | Pointer to **map[string]interface{}** |  | [optional] 
**CurrentOrganization** | Pointer to **map[string]interface{}** |  | [optional] 
**CurrentWorkspace** | Pointer to **map[string]interface{}** |  | [optional] 
**ConnectedAccounts** | Pointer to **[]map[string]interface{}** |  | [optional] 

## Methods

### NewAgentSessionContext

`func NewAgentSessionContext() *AgentSessionContext`

NewAgentSessionContext instantiates a new AgentSessionContext object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAgentSessionContextWithDefaults

`func NewAgentSessionContextWithDefaults() *AgentSessionContext`

NewAgentSessionContextWithDefaults instantiates a new AgentSessionContext object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUser

`func (o *AgentSessionContext) GetUser() map[string]interface{}`

GetUser returns the User field if non-nil, zero value otherwise.

### GetUserOk

`func (o *AgentSessionContext) GetUserOk() (*map[string]interface{}, bool)`

GetUserOk returns a tuple with the User field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUser

`func (o *AgentSessionContext) SetUser(v map[string]interface{})`

SetUser sets User field to given value.

### HasUser

`func (o *AgentSessionContext) HasUser() bool`

HasUser returns a boolean if a field has been set.

### GetCurrentOrganization

`func (o *AgentSessionContext) GetCurrentOrganization() map[string]interface{}`

GetCurrentOrganization returns the CurrentOrganization field if non-nil, zero value otherwise.

### GetCurrentOrganizationOk

`func (o *AgentSessionContext) GetCurrentOrganizationOk() (*map[string]interface{}, bool)`

GetCurrentOrganizationOk returns a tuple with the CurrentOrganization field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrentOrganization

`func (o *AgentSessionContext) SetCurrentOrganization(v map[string]interface{})`

SetCurrentOrganization sets CurrentOrganization field to given value.

### HasCurrentOrganization

`func (o *AgentSessionContext) HasCurrentOrganization() bool`

HasCurrentOrganization returns a boolean if a field has been set.

### SetCurrentOrganizationNil

`func (o *AgentSessionContext) SetCurrentOrganizationNil(b bool)`

 SetCurrentOrganizationNil sets the value for CurrentOrganization to be an explicit nil

### UnsetCurrentOrganization
`func (o *AgentSessionContext) UnsetCurrentOrganization()`

UnsetCurrentOrganization ensures that no value is present for CurrentOrganization, not even an explicit nil
### GetCurrentWorkspace

`func (o *AgentSessionContext) GetCurrentWorkspace() map[string]interface{}`

GetCurrentWorkspace returns the CurrentWorkspace field if non-nil, zero value otherwise.

### GetCurrentWorkspaceOk

`func (o *AgentSessionContext) GetCurrentWorkspaceOk() (*map[string]interface{}, bool)`

GetCurrentWorkspaceOk returns a tuple with the CurrentWorkspace field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrentWorkspace

`func (o *AgentSessionContext) SetCurrentWorkspace(v map[string]interface{})`

SetCurrentWorkspace sets CurrentWorkspace field to given value.

### HasCurrentWorkspace

`func (o *AgentSessionContext) HasCurrentWorkspace() bool`

HasCurrentWorkspace returns a boolean if a field has been set.

### SetCurrentWorkspaceNil

`func (o *AgentSessionContext) SetCurrentWorkspaceNil(b bool)`

 SetCurrentWorkspaceNil sets the value for CurrentWorkspace to be an explicit nil

### UnsetCurrentWorkspace
`func (o *AgentSessionContext) UnsetCurrentWorkspace()`

UnsetCurrentWorkspace ensures that no value is present for CurrentWorkspace, not even an explicit nil
### GetConnectedAccounts

`func (o *AgentSessionContext) GetConnectedAccounts() []map[string]interface{}`

GetConnectedAccounts returns the ConnectedAccounts field if non-nil, zero value otherwise.

### GetConnectedAccountsOk

`func (o *AgentSessionContext) GetConnectedAccountsOk() (*[]map[string]interface{}, bool)`

GetConnectedAccountsOk returns a tuple with the ConnectedAccounts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConnectedAccounts

`func (o *AgentSessionContext) SetConnectedAccounts(v []map[string]interface{})`

SetConnectedAccounts sets ConnectedAccounts field to given value.

### HasConnectedAccounts

`func (o *AgentSessionContext) HasConnectedAccounts() bool`

HasConnectedAccounts returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


