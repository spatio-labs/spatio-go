# UpdateRowRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Cells** | **map[string]interface{}** | Sparse update. Keys present in the map overwrite that column; keys absent are preserved.  | 

## Methods

### NewUpdateRowRequest

`func NewUpdateRowRequest(cells map[string]interface{}, ) *UpdateRowRequest`

NewUpdateRowRequest instantiates a new UpdateRowRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateRowRequestWithDefaults

`func NewUpdateRowRequestWithDefaults() *UpdateRowRequest`

NewUpdateRowRequestWithDefaults instantiates a new UpdateRowRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCells

`func (o *UpdateRowRequest) GetCells() map[string]interface{}`

GetCells returns the Cells field if non-nil, zero value otherwise.

### GetCellsOk

`func (o *UpdateRowRequest) GetCellsOk() (*map[string]interface{}, bool)`

GetCellsOk returns a tuple with the Cells field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCells

`func (o *UpdateRowRequest) SetCells(v map[string]interface{})`

SetCells sets Cells field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


