# ExecuteActionResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Ok** | Pointer to **bool** |  | [optional] 
**Data** | Pointer to **map[string]interface{}** |  | [optional] 
**Error** | Pointer to **string** |  | [optional] 

## Methods

### NewExecuteActionResponse

`func NewExecuteActionResponse() *ExecuteActionResponse`

NewExecuteActionResponse instantiates a new ExecuteActionResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewExecuteActionResponseWithDefaults

`func NewExecuteActionResponseWithDefaults() *ExecuteActionResponse`

NewExecuteActionResponseWithDefaults instantiates a new ExecuteActionResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetOk

`func (o *ExecuteActionResponse) GetOk() bool`

GetOk returns the Ok field if non-nil, zero value otherwise.

### GetOkOk

`func (o *ExecuteActionResponse) GetOkOk() (*bool, bool)`

GetOkOk returns a tuple with the Ok field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOk

`func (o *ExecuteActionResponse) SetOk(v bool)`

SetOk sets Ok field to given value.

### HasOk

`func (o *ExecuteActionResponse) HasOk() bool`

HasOk returns a boolean if a field has been set.

### GetData

`func (o *ExecuteActionResponse) GetData() map[string]interface{}`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *ExecuteActionResponse) GetDataOk() (*map[string]interface{}, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *ExecuteActionResponse) SetData(v map[string]interface{})`

SetData sets Data field to given value.

### HasData

`func (o *ExecuteActionResponse) HasData() bool`

HasData returns a boolean if a field has been set.

### GetError

`func (o *ExecuteActionResponse) GetError() string`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *ExecuteActionResponse) GetErrorOk() (*string, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *ExecuteActionResponse) SetError(v string)`

SetError sets Error field to given value.

### HasError

`func (o *ExecuteActionResponse) HasError() bool`

HasError returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


