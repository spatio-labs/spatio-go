# CoreActionListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Actions** | [**[]CoreAction**](CoreAction.md) |  | 
**Total** | Pointer to **int32** |  | [optional] 

## Methods

### NewCoreActionListResponse

`func NewCoreActionListResponse(actions []CoreAction, ) *CoreActionListResponse`

NewCoreActionListResponse instantiates a new CoreActionListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCoreActionListResponseWithDefaults

`func NewCoreActionListResponseWithDefaults() *CoreActionListResponse`

NewCoreActionListResponseWithDefaults instantiates a new CoreActionListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetActions

`func (o *CoreActionListResponse) GetActions() []CoreAction`

GetActions returns the Actions field if non-nil, zero value otherwise.

### GetActionsOk

`func (o *CoreActionListResponse) GetActionsOk() (*[]CoreAction, bool)`

GetActionsOk returns a tuple with the Actions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActions

`func (o *CoreActionListResponse) SetActions(v []CoreAction)`

SetActions sets Actions field to given value.


### SetActionsNil

`func (o *CoreActionListResponse) SetActionsNil(b bool)`

 SetActionsNil sets the value for Actions to be an explicit nil

### UnsetActions
`func (o *CoreActionListResponse) UnsetActions()`

UnsetActions ensures that no value is present for Actions, not even an explicit nil
### GetTotal

`func (o *CoreActionListResponse) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *CoreActionListResponse) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *CoreActionListResponse) SetTotal(v int32)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *CoreActionListResponse) HasTotal() bool`

HasTotal returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


