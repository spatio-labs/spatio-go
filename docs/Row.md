# Row

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Index** | **int32** | Zero-based row position. | 
**Cells** | **map[string]interface{}** |  | 

## Methods

### NewRow

`func NewRow(index int32, cells map[string]interface{}, ) *Row`

NewRow instantiates a new Row object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRowWithDefaults

`func NewRowWithDefaults() *Row`

NewRowWithDefaults instantiates a new Row object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetIndex

`func (o *Row) GetIndex() int32`

GetIndex returns the Index field if non-nil, zero value otherwise.

### GetIndexOk

`func (o *Row) GetIndexOk() (*int32, bool)`

GetIndexOk returns a tuple with the Index field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIndex

`func (o *Row) SetIndex(v int32)`

SetIndex sets Index field to given value.


### GetCells

`func (o *Row) GetCells() map[string]interface{}`

GetCells returns the Cells field if non-nil, zero value otherwise.

### GetCellsOk

`func (o *Row) GetCellsOk() (*map[string]interface{}, bool)`

GetCellsOk returns a tuple with the Cells field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCells

`func (o *Row) SetCells(v map[string]interface{})`

SetCells sets Cells field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


