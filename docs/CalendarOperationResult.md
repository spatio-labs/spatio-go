# CalendarOperationResult

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | **bool** |  | 
**Data** | Pointer to **interface{}** | Operation-specific payload. See the operation&#39;s response description for the concrete shape.  | [optional] 
**Errors** | Pointer to [**[]CalendarAccountError**](CalendarAccountError.md) |  | [optional] 
**Metadata** | Pointer to **map[string]interface{}** |  | [optional] 

## Methods

### NewCalendarOperationResult

`func NewCalendarOperationResult(success bool, ) *CalendarOperationResult`

NewCalendarOperationResult instantiates a new CalendarOperationResult object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCalendarOperationResultWithDefaults

`func NewCalendarOperationResultWithDefaults() *CalendarOperationResult`

NewCalendarOperationResultWithDefaults instantiates a new CalendarOperationResult object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *CalendarOperationResult) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *CalendarOperationResult) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *CalendarOperationResult) SetSuccess(v bool)`

SetSuccess sets Success field to given value.


### GetData

`func (o *CalendarOperationResult) GetData() interface{}`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *CalendarOperationResult) GetDataOk() (*interface{}, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *CalendarOperationResult) SetData(v interface{})`

SetData sets Data field to given value.

### HasData

`func (o *CalendarOperationResult) HasData() bool`

HasData returns a boolean if a field has been set.

### SetDataNil

`func (o *CalendarOperationResult) SetDataNil(b bool)`

 SetDataNil sets the value for Data to be an explicit nil

### UnsetData
`func (o *CalendarOperationResult) UnsetData()`

UnsetData ensures that no value is present for Data, not even an explicit nil
### GetErrors

`func (o *CalendarOperationResult) GetErrors() []CalendarAccountError`

GetErrors returns the Errors field if non-nil, zero value otherwise.

### GetErrorsOk

`func (o *CalendarOperationResult) GetErrorsOk() (*[]CalendarAccountError, bool)`

GetErrorsOk returns a tuple with the Errors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrors

`func (o *CalendarOperationResult) SetErrors(v []CalendarAccountError)`

SetErrors sets Errors field to given value.

### HasErrors

`func (o *CalendarOperationResult) HasErrors() bool`

HasErrors returns a boolean if a field has been set.

### GetMetadata

`func (o *CalendarOperationResult) GetMetadata() map[string]interface{}`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *CalendarOperationResult) GetMetadataOk() (*map[string]interface{}, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *CalendarOperationResult) SetMetadata(v map[string]interface{})`

SetMetadata sets Metadata field to given value.

### HasMetadata

`func (o *CalendarOperationResult) HasMetadata() bool`

HasMetadata returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


