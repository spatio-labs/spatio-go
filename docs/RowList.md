# RowList

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Rows** | [**[]Row**](Row.md) |  | 
**Total** | **int32** |  | 

## Methods

### NewRowList

`func NewRowList(rows []Row, total int32, ) *RowList`

NewRowList instantiates a new RowList object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRowListWithDefaults

`func NewRowListWithDefaults() *RowList`

NewRowListWithDefaults instantiates a new RowList object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRows

`func (o *RowList) GetRows() []Row`

GetRows returns the Rows field if non-nil, zero value otherwise.

### GetRowsOk

`func (o *RowList) GetRowsOk() (*[]Row, bool)`

GetRowsOk returns a tuple with the Rows field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRows

`func (o *RowList) SetRows(v []Row)`

SetRows sets Rows field to given value.


### GetTotal

`func (o *RowList) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *RowList) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *RowList) SetTotal(v int32)`

SetTotal sets Total field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


