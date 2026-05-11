# RoutineRunCompleteRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Status** | Pointer to **string** |  | [optional] 
**Metadata** | Pointer to **map[string]interface{}** |  | [optional] 

## Methods

### NewRoutineRunCompleteRequest

`func NewRoutineRunCompleteRequest() *RoutineRunCompleteRequest`

NewRoutineRunCompleteRequest instantiates a new RoutineRunCompleteRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRoutineRunCompleteRequestWithDefaults

`func NewRoutineRunCompleteRequestWithDefaults() *RoutineRunCompleteRequest`

NewRoutineRunCompleteRequestWithDefaults instantiates a new RoutineRunCompleteRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetStatus

`func (o *RoutineRunCompleteRequest) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *RoutineRunCompleteRequest) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *RoutineRunCompleteRequest) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *RoutineRunCompleteRequest) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetMetadata

`func (o *RoutineRunCompleteRequest) GetMetadata() map[string]interface{}`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *RoutineRunCompleteRequest) GetMetadataOk() (*map[string]interface{}, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *RoutineRunCompleteRequest) SetMetadata(v map[string]interface{})`

SetMetadata sets Metadata field to given value.

### HasMetadata

`func (o *RoutineRunCompleteRequest) HasMetadata() bool`

HasMetadata returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


