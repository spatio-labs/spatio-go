# Cell

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Row** | **int32** |  | 
**Column** | **string** |  | 
**Value** | **interface{}** | Any JSON value (string, number, boolean, null, object). | 

## Methods

### NewCell

`func NewCell(row int32, column string, value interface{}, ) *Cell`

NewCell instantiates a new Cell object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCellWithDefaults

`func NewCellWithDefaults() *Cell`

NewCellWithDefaults instantiates a new Cell object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRow

`func (o *Cell) GetRow() int32`

GetRow returns the Row field if non-nil, zero value otherwise.

### GetRowOk

`func (o *Cell) GetRowOk() (*int32, bool)`

GetRowOk returns a tuple with the Row field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRow

`func (o *Cell) SetRow(v int32)`

SetRow sets Row field to given value.


### GetColumn

`func (o *Cell) GetColumn() string`

GetColumn returns the Column field if non-nil, zero value otherwise.

### GetColumnOk

`func (o *Cell) GetColumnOk() (*string, bool)`

GetColumnOk returns a tuple with the Column field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetColumn

`func (o *Cell) SetColumn(v string)`

SetColumn sets Column field to given value.


### GetValue

`func (o *Cell) GetValue() interface{}`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *Cell) GetValueOk() (*interface{}, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *Cell) SetValue(v interface{})`

SetValue sets Value field to given value.


### SetValueNil

`func (o *Cell) SetValueNil(b bool)`

 SetValueNil sets the value for Value to be an explicit nil

### UnsetValue
`func (o *Cell) UnsetValue()`

UnsetValue ensures that no value is present for Value, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


