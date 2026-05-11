# CalendarSyncResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enqueued** | **int32** |  | 
**Jobs** | **[]string** |  | 
**Waited** | Pointer to **bool** |  | [optional] 
**TimedOut** | Pointer to **bool** |  | [optional] 
**Errors** | Pointer to **[]map[string]interface{}** |  | [optional] 

## Methods

### NewCalendarSyncResponse

`func NewCalendarSyncResponse(enqueued int32, jobs []string, ) *CalendarSyncResponse`

NewCalendarSyncResponse instantiates a new CalendarSyncResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCalendarSyncResponseWithDefaults

`func NewCalendarSyncResponseWithDefaults() *CalendarSyncResponse`

NewCalendarSyncResponseWithDefaults instantiates a new CalendarSyncResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEnqueued

`func (o *CalendarSyncResponse) GetEnqueued() int32`

GetEnqueued returns the Enqueued field if non-nil, zero value otherwise.

### GetEnqueuedOk

`func (o *CalendarSyncResponse) GetEnqueuedOk() (*int32, bool)`

GetEnqueuedOk returns a tuple with the Enqueued field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnqueued

`func (o *CalendarSyncResponse) SetEnqueued(v int32)`

SetEnqueued sets Enqueued field to given value.


### GetJobs

`func (o *CalendarSyncResponse) GetJobs() []string`

GetJobs returns the Jobs field if non-nil, zero value otherwise.

### GetJobsOk

`func (o *CalendarSyncResponse) GetJobsOk() (*[]string, bool)`

GetJobsOk returns a tuple with the Jobs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJobs

`func (o *CalendarSyncResponse) SetJobs(v []string)`

SetJobs sets Jobs field to given value.


### GetWaited

`func (o *CalendarSyncResponse) GetWaited() bool`

GetWaited returns the Waited field if non-nil, zero value otherwise.

### GetWaitedOk

`func (o *CalendarSyncResponse) GetWaitedOk() (*bool, bool)`

GetWaitedOk returns a tuple with the Waited field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWaited

`func (o *CalendarSyncResponse) SetWaited(v bool)`

SetWaited sets Waited field to given value.

### HasWaited

`func (o *CalendarSyncResponse) HasWaited() bool`

HasWaited returns a boolean if a field has been set.

### GetTimedOut

`func (o *CalendarSyncResponse) GetTimedOut() bool`

GetTimedOut returns the TimedOut field if non-nil, zero value otherwise.

### GetTimedOutOk

`func (o *CalendarSyncResponse) GetTimedOutOk() (*bool, bool)`

GetTimedOutOk returns a tuple with the TimedOut field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimedOut

`func (o *CalendarSyncResponse) SetTimedOut(v bool)`

SetTimedOut sets TimedOut field to given value.

### HasTimedOut

`func (o *CalendarSyncResponse) HasTimedOut() bool`

HasTimedOut returns a boolean if a field has been set.

### GetErrors

`func (o *CalendarSyncResponse) GetErrors() []map[string]interface{}`

GetErrors returns the Errors field if non-nil, zero value otherwise.

### GetErrorsOk

`func (o *CalendarSyncResponse) GetErrorsOk() (*[]map[string]interface{}, bool)`

GetErrorsOk returns a tuple with the Errors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrors

`func (o *CalendarSyncResponse) SetErrors(v []map[string]interface{})`

SetErrors sets Errors field to given value.

### HasErrors

`func (o *CalendarSyncResponse) HasErrors() bool`

HasErrors returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


