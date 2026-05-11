# CallListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Calls** | [**[]SpatioCall**](SpatioCall.md) |  | 
**Total** | Pointer to **int32** |  | [optional] 

## Methods

### NewCallListResponse

`func NewCallListResponse(calls []SpatioCall, ) *CallListResponse`

NewCallListResponse instantiates a new CallListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCallListResponseWithDefaults

`func NewCallListResponseWithDefaults() *CallListResponse`

NewCallListResponseWithDefaults instantiates a new CallListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCalls

`func (o *CallListResponse) GetCalls() []SpatioCall`

GetCalls returns the Calls field if non-nil, zero value otherwise.

### GetCallsOk

`func (o *CallListResponse) GetCallsOk() (*[]SpatioCall, bool)`

GetCallsOk returns a tuple with the Calls field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCalls

`func (o *CallListResponse) SetCalls(v []SpatioCall)`

SetCalls sets Calls field to given value.


### SetCallsNil

`func (o *CallListResponse) SetCallsNil(b bool)`

 SetCallsNil sets the value for Calls to be an explicit nil

### UnsetCalls
`func (o *CallListResponse) UnsetCalls()`

UnsetCalls ensures that no value is present for Calls, not even an explicit nil
### GetTotal

`func (o *CallListResponse) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *CallListResponse) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *CallListResponse) SetTotal(v int32)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *CallListResponse) HasTotal() bool`

HasTotal returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


