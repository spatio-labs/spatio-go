# RoutineRunProgressRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Progress** | Pointer to **int32** |  | [optional] 
**Metadata** | Pointer to **map[string]interface{}** |  | [optional] 

## Methods

### NewRoutineRunProgressRequest

`func NewRoutineRunProgressRequest() *RoutineRunProgressRequest`

NewRoutineRunProgressRequest instantiates a new RoutineRunProgressRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRoutineRunProgressRequestWithDefaults

`func NewRoutineRunProgressRequestWithDefaults() *RoutineRunProgressRequest`

NewRoutineRunProgressRequestWithDefaults instantiates a new RoutineRunProgressRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetProgress

`func (o *RoutineRunProgressRequest) GetProgress() int32`

GetProgress returns the Progress field if non-nil, zero value otherwise.

### GetProgressOk

`func (o *RoutineRunProgressRequest) GetProgressOk() (*int32, bool)`

GetProgressOk returns a tuple with the Progress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProgress

`func (o *RoutineRunProgressRequest) SetProgress(v int32)`

SetProgress sets Progress field to given value.

### HasProgress

`func (o *RoutineRunProgressRequest) HasProgress() bool`

HasProgress returns a boolean if a field has been set.

### GetMetadata

`func (o *RoutineRunProgressRequest) GetMetadata() map[string]interface{}`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *RoutineRunProgressRequest) GetMetadataOk() (*map[string]interface{}, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *RoutineRunProgressRequest) SetMetadata(v map[string]interface{})`

SetMetadata sets Metadata field to given value.

### HasMetadata

`func (o *RoutineRunProgressRequest) HasMetadata() bool`

HasMetadata returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


