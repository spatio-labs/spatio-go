# ConsumeAgentTaskResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Allowed** | **bool** |  | 
**TaskCount** | Pointer to **NullableInt32** |  | [optional] 
**DailyLimit** | Pointer to **NullableInt32** |  | [optional] 
**TrialEndsAt** | Pointer to **NullableTime** |  | [optional] 
**Paid** | Pointer to **bool** |  | [optional] 

## Methods

### NewConsumeAgentTaskResponse

`func NewConsumeAgentTaskResponse(allowed bool, ) *ConsumeAgentTaskResponse`

NewConsumeAgentTaskResponse instantiates a new ConsumeAgentTaskResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewConsumeAgentTaskResponseWithDefaults

`func NewConsumeAgentTaskResponseWithDefaults() *ConsumeAgentTaskResponse`

NewConsumeAgentTaskResponseWithDefaults instantiates a new ConsumeAgentTaskResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAllowed

`func (o *ConsumeAgentTaskResponse) GetAllowed() bool`

GetAllowed returns the Allowed field if non-nil, zero value otherwise.

### GetAllowedOk

`func (o *ConsumeAgentTaskResponse) GetAllowedOk() (*bool, bool)`

GetAllowedOk returns a tuple with the Allowed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAllowed

`func (o *ConsumeAgentTaskResponse) SetAllowed(v bool)`

SetAllowed sets Allowed field to given value.


### GetTaskCount

`func (o *ConsumeAgentTaskResponse) GetTaskCount() int32`

GetTaskCount returns the TaskCount field if non-nil, zero value otherwise.

### GetTaskCountOk

`func (o *ConsumeAgentTaskResponse) GetTaskCountOk() (*int32, bool)`

GetTaskCountOk returns a tuple with the TaskCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaskCount

`func (o *ConsumeAgentTaskResponse) SetTaskCount(v int32)`

SetTaskCount sets TaskCount field to given value.

### HasTaskCount

`func (o *ConsumeAgentTaskResponse) HasTaskCount() bool`

HasTaskCount returns a boolean if a field has been set.

### SetTaskCountNil

`func (o *ConsumeAgentTaskResponse) SetTaskCountNil(b bool)`

 SetTaskCountNil sets the value for TaskCount to be an explicit nil

### UnsetTaskCount
`func (o *ConsumeAgentTaskResponse) UnsetTaskCount()`

UnsetTaskCount ensures that no value is present for TaskCount, not even an explicit nil
### GetDailyLimit

`func (o *ConsumeAgentTaskResponse) GetDailyLimit() int32`

GetDailyLimit returns the DailyLimit field if non-nil, zero value otherwise.

### GetDailyLimitOk

`func (o *ConsumeAgentTaskResponse) GetDailyLimitOk() (*int32, bool)`

GetDailyLimitOk returns a tuple with the DailyLimit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDailyLimit

`func (o *ConsumeAgentTaskResponse) SetDailyLimit(v int32)`

SetDailyLimit sets DailyLimit field to given value.

### HasDailyLimit

`func (o *ConsumeAgentTaskResponse) HasDailyLimit() bool`

HasDailyLimit returns a boolean if a field has been set.

### SetDailyLimitNil

`func (o *ConsumeAgentTaskResponse) SetDailyLimitNil(b bool)`

 SetDailyLimitNil sets the value for DailyLimit to be an explicit nil

### UnsetDailyLimit
`func (o *ConsumeAgentTaskResponse) UnsetDailyLimit()`

UnsetDailyLimit ensures that no value is present for DailyLimit, not even an explicit nil
### GetTrialEndsAt

`func (o *ConsumeAgentTaskResponse) GetTrialEndsAt() time.Time`

GetTrialEndsAt returns the TrialEndsAt field if non-nil, zero value otherwise.

### GetTrialEndsAtOk

`func (o *ConsumeAgentTaskResponse) GetTrialEndsAtOk() (*time.Time, bool)`

GetTrialEndsAtOk returns a tuple with the TrialEndsAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTrialEndsAt

`func (o *ConsumeAgentTaskResponse) SetTrialEndsAt(v time.Time)`

SetTrialEndsAt sets TrialEndsAt field to given value.

### HasTrialEndsAt

`func (o *ConsumeAgentTaskResponse) HasTrialEndsAt() bool`

HasTrialEndsAt returns a boolean if a field has been set.

### SetTrialEndsAtNil

`func (o *ConsumeAgentTaskResponse) SetTrialEndsAtNil(b bool)`

 SetTrialEndsAtNil sets the value for TrialEndsAt to be an explicit nil

### UnsetTrialEndsAt
`func (o *ConsumeAgentTaskResponse) UnsetTrialEndsAt()`

UnsetTrialEndsAt ensures that no value is present for TrialEndsAt, not even an explicit nil
### GetPaid

`func (o *ConsumeAgentTaskResponse) GetPaid() bool`

GetPaid returns the Paid field if non-nil, zero value otherwise.

### GetPaidOk

`func (o *ConsumeAgentTaskResponse) GetPaidOk() (*bool, bool)`

GetPaidOk returns a tuple with the Paid field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaid

`func (o *ConsumeAgentTaskResponse) SetPaid(v bool)`

SetPaid sets Paid field to given value.

### HasPaid

`func (o *ConsumeAgentTaskResponse) HasPaid() bool`

HasPaid returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


