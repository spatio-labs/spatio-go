# CreateRowRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Index** | Pointer to **int32** | Optional zero-based insert position. Omit to append at the end.  | [optional] 
**Cells** | **map[string]interface{}** |  | 

## Methods

### NewCreateRowRequest

`func NewCreateRowRequest(cells map[string]interface{}, ) *CreateRowRequest`

NewCreateRowRequest instantiates a new CreateRowRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateRowRequestWithDefaults

`func NewCreateRowRequestWithDefaults() *CreateRowRequest`

NewCreateRowRequestWithDefaults instantiates a new CreateRowRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetIndex

`func (o *CreateRowRequest) GetIndex() int32`

GetIndex returns the Index field if non-nil, zero value otherwise.

### GetIndexOk

`func (o *CreateRowRequest) GetIndexOk() (*int32, bool)`

GetIndexOk returns a tuple with the Index field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIndex

`func (o *CreateRowRequest) SetIndex(v int32)`

SetIndex sets Index field to given value.

### HasIndex

`func (o *CreateRowRequest) HasIndex() bool`

HasIndex returns a boolean if a field has been set.

### GetCells

`func (o *CreateRowRequest) GetCells() map[string]interface{}`

GetCells returns the Cells field if non-nil, zero value otherwise.

### GetCellsOk

`func (o *CreateRowRequest) GetCellsOk() (*map[string]interface{}, bool)`

GetCellsOk returns a tuple with the Cells field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCells

`func (o *CreateRowRequest) SetCells(v map[string]interface{})`

SetCells sets Cells field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


