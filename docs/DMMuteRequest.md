# DMMuteRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**UntilSeconds** | Pointer to **int64** |  | [optional] 
**Forever** | Pointer to **bool** |  | [optional] 
**AccountId** | Pointer to **string** |  | [optional] 

## Methods

### NewDMMuteRequest

`func NewDMMuteRequest() *DMMuteRequest`

NewDMMuteRequest instantiates a new DMMuteRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDMMuteRequestWithDefaults

`func NewDMMuteRequestWithDefaults() *DMMuteRequest`

NewDMMuteRequestWithDefaults instantiates a new DMMuteRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUntilSeconds

`func (o *DMMuteRequest) GetUntilSeconds() int64`

GetUntilSeconds returns the UntilSeconds field if non-nil, zero value otherwise.

### GetUntilSecondsOk

`func (o *DMMuteRequest) GetUntilSecondsOk() (*int64, bool)`

GetUntilSecondsOk returns a tuple with the UntilSeconds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUntilSeconds

`func (o *DMMuteRequest) SetUntilSeconds(v int64)`

SetUntilSeconds sets UntilSeconds field to given value.

### HasUntilSeconds

`func (o *DMMuteRequest) HasUntilSeconds() bool`

HasUntilSeconds returns a boolean if a field has been set.

### GetForever

`func (o *DMMuteRequest) GetForever() bool`

GetForever returns the Forever field if non-nil, zero value otherwise.

### GetForeverOk

`func (o *DMMuteRequest) GetForeverOk() (*bool, bool)`

GetForeverOk returns a tuple with the Forever field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetForever

`func (o *DMMuteRequest) SetForever(v bool)`

SetForever sets Forever field to given value.

### HasForever

`func (o *DMMuteRequest) HasForever() bool`

HasForever returns a boolean if a field has been set.

### GetAccountId

`func (o *DMMuteRequest) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *DMMuteRequest) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *DMMuteRequest) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *DMMuteRequest) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


