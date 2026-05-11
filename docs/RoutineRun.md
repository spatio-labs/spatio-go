# RoutineRun

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**RoutineId** | Pointer to **string** |  | [optional] 
**Status** | Pointer to **string** |  | [optional] 
**Progress** | Pointer to **int32** |  | [optional] 
**Metadata** | Pointer to **map[string]interface{}** |  | [optional] 
**StartedAt** | Pointer to **time.Time** |  | [optional] 
**CompletedAt** | Pointer to **NullableTime** |  | [optional] 

## Methods

### NewRoutineRun

`func NewRoutineRun(id string, ) *RoutineRun`

NewRoutineRun instantiates a new RoutineRun object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRoutineRunWithDefaults

`func NewRoutineRunWithDefaults() *RoutineRun`

NewRoutineRunWithDefaults instantiates a new RoutineRun object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *RoutineRun) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *RoutineRun) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *RoutineRun) SetId(v string)`

SetId sets Id field to given value.


### GetRoutineId

`func (o *RoutineRun) GetRoutineId() string`

GetRoutineId returns the RoutineId field if non-nil, zero value otherwise.

### GetRoutineIdOk

`func (o *RoutineRun) GetRoutineIdOk() (*string, bool)`

GetRoutineIdOk returns a tuple with the RoutineId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRoutineId

`func (o *RoutineRun) SetRoutineId(v string)`

SetRoutineId sets RoutineId field to given value.

### HasRoutineId

`func (o *RoutineRun) HasRoutineId() bool`

HasRoutineId returns a boolean if a field has been set.

### GetStatus

`func (o *RoutineRun) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *RoutineRun) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *RoutineRun) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *RoutineRun) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetProgress

`func (o *RoutineRun) GetProgress() int32`

GetProgress returns the Progress field if non-nil, zero value otherwise.

### GetProgressOk

`func (o *RoutineRun) GetProgressOk() (*int32, bool)`

GetProgressOk returns a tuple with the Progress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProgress

`func (o *RoutineRun) SetProgress(v int32)`

SetProgress sets Progress field to given value.

### HasProgress

`func (o *RoutineRun) HasProgress() bool`

HasProgress returns a boolean if a field has been set.

### GetMetadata

`func (o *RoutineRun) GetMetadata() map[string]interface{}`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *RoutineRun) GetMetadataOk() (*map[string]interface{}, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *RoutineRun) SetMetadata(v map[string]interface{})`

SetMetadata sets Metadata field to given value.

### HasMetadata

`func (o *RoutineRun) HasMetadata() bool`

HasMetadata returns a boolean if a field has been set.

### GetStartedAt

`func (o *RoutineRun) GetStartedAt() time.Time`

GetStartedAt returns the StartedAt field if non-nil, zero value otherwise.

### GetStartedAtOk

`func (o *RoutineRun) GetStartedAtOk() (*time.Time, bool)`

GetStartedAtOk returns a tuple with the StartedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStartedAt

`func (o *RoutineRun) SetStartedAt(v time.Time)`

SetStartedAt sets StartedAt field to given value.

### HasStartedAt

`func (o *RoutineRun) HasStartedAt() bool`

HasStartedAt returns a boolean if a field has been set.

### GetCompletedAt

`func (o *RoutineRun) GetCompletedAt() time.Time`

GetCompletedAt returns the CompletedAt field if non-nil, zero value otherwise.

### GetCompletedAtOk

`func (o *RoutineRun) GetCompletedAtOk() (*time.Time, bool)`

GetCompletedAtOk returns a tuple with the CompletedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCompletedAt

`func (o *RoutineRun) SetCompletedAt(v time.Time)`

SetCompletedAt sets CompletedAt field to given value.

### HasCompletedAt

`func (o *RoutineRun) HasCompletedAt() bool`

HasCompletedAt returns a boolean if a field has been set.

### SetCompletedAtNil

`func (o *RoutineRun) SetCompletedAtNil(b bool)`

 SetCompletedAtNil sets the value for CompletedAt to be an explicit nil

### UnsetCompletedAt
`func (o *RoutineRun) UnsetCompletedAt()`

UnsetCompletedAt ensures that no value is present for CompletedAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


