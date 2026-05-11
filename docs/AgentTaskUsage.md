# AgentTaskUsage

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Allowed** | **bool** |  | 
**TaskCount** | Pointer to **NullableInt32** |  | [optional] 
**DailyLimit** | Pointer to **NullableInt32** |  | [optional] 
**TrialEndsAt** | Pointer to **NullableTime** |  | [optional] 
**Paid** | Pointer to **bool** |  | [optional] 

## Methods

### NewAgentTaskUsage

`func NewAgentTaskUsage(allowed bool, ) *AgentTaskUsage`

NewAgentTaskUsage instantiates a new AgentTaskUsage object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAgentTaskUsageWithDefaults

`func NewAgentTaskUsageWithDefaults() *AgentTaskUsage`

NewAgentTaskUsageWithDefaults instantiates a new AgentTaskUsage object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAllowed

`func (o *AgentTaskUsage) GetAllowed() bool`

GetAllowed returns the Allowed field if non-nil, zero value otherwise.

### GetAllowedOk

`func (o *AgentTaskUsage) GetAllowedOk() (*bool, bool)`

GetAllowedOk returns a tuple with the Allowed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAllowed

`func (o *AgentTaskUsage) SetAllowed(v bool)`

SetAllowed sets Allowed field to given value.


### GetTaskCount

`func (o *AgentTaskUsage) GetTaskCount() int32`

GetTaskCount returns the TaskCount field if non-nil, zero value otherwise.

### GetTaskCountOk

`func (o *AgentTaskUsage) GetTaskCountOk() (*int32, bool)`

GetTaskCountOk returns a tuple with the TaskCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaskCount

`func (o *AgentTaskUsage) SetTaskCount(v int32)`

SetTaskCount sets TaskCount field to given value.

### HasTaskCount

`func (o *AgentTaskUsage) HasTaskCount() bool`

HasTaskCount returns a boolean if a field has been set.

### SetTaskCountNil

`func (o *AgentTaskUsage) SetTaskCountNil(b bool)`

 SetTaskCountNil sets the value for TaskCount to be an explicit nil

### UnsetTaskCount
`func (o *AgentTaskUsage) UnsetTaskCount()`

UnsetTaskCount ensures that no value is present for TaskCount, not even an explicit nil
### GetDailyLimit

`func (o *AgentTaskUsage) GetDailyLimit() int32`

GetDailyLimit returns the DailyLimit field if non-nil, zero value otherwise.

### GetDailyLimitOk

`func (o *AgentTaskUsage) GetDailyLimitOk() (*int32, bool)`

GetDailyLimitOk returns a tuple with the DailyLimit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDailyLimit

`func (o *AgentTaskUsage) SetDailyLimit(v int32)`

SetDailyLimit sets DailyLimit field to given value.

### HasDailyLimit

`func (o *AgentTaskUsage) HasDailyLimit() bool`

HasDailyLimit returns a boolean if a field has been set.

### SetDailyLimitNil

`func (o *AgentTaskUsage) SetDailyLimitNil(b bool)`

 SetDailyLimitNil sets the value for DailyLimit to be an explicit nil

### UnsetDailyLimit
`func (o *AgentTaskUsage) UnsetDailyLimit()`

UnsetDailyLimit ensures that no value is present for DailyLimit, not even an explicit nil
### GetTrialEndsAt

`func (o *AgentTaskUsage) GetTrialEndsAt() time.Time`

GetTrialEndsAt returns the TrialEndsAt field if non-nil, zero value otherwise.

### GetTrialEndsAtOk

`func (o *AgentTaskUsage) GetTrialEndsAtOk() (*time.Time, bool)`

GetTrialEndsAtOk returns a tuple with the TrialEndsAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTrialEndsAt

`func (o *AgentTaskUsage) SetTrialEndsAt(v time.Time)`

SetTrialEndsAt sets TrialEndsAt field to given value.

### HasTrialEndsAt

`func (o *AgentTaskUsage) HasTrialEndsAt() bool`

HasTrialEndsAt returns a boolean if a field has been set.

### SetTrialEndsAtNil

`func (o *AgentTaskUsage) SetTrialEndsAtNil(b bool)`

 SetTrialEndsAtNil sets the value for TrialEndsAt to be an explicit nil

### UnsetTrialEndsAt
`func (o *AgentTaskUsage) UnsetTrialEndsAt()`

UnsetTrialEndsAt ensures that no value is present for TrialEndsAt, not even an explicit nil
### GetPaid

`func (o *AgentTaskUsage) GetPaid() bool`

GetPaid returns the Paid field if non-nil, zero value otherwise.

### GetPaidOk

`func (o *AgentTaskUsage) GetPaidOk() (*bool, bool)`

GetPaidOk returns a tuple with the Paid field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaid

`func (o *AgentTaskUsage) SetPaid(v bool)`

SetPaid sets Paid field to given value.

### HasPaid

`func (o *AgentTaskUsage) HasPaid() bool`

HasPaid returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


