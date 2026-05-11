# GetThreadResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Thread** | [**SpatioThread**](SpatioThread.md) |  | 
**Provider** | **string** |  | 

## Methods

### NewGetThreadResponse

`func NewGetThreadResponse(thread SpatioThread, provider string, ) *GetThreadResponse`

NewGetThreadResponse instantiates a new GetThreadResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGetThreadResponseWithDefaults

`func NewGetThreadResponseWithDefaults() *GetThreadResponse`

NewGetThreadResponseWithDefaults instantiates a new GetThreadResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetThread

`func (o *GetThreadResponse) GetThread() SpatioThread`

GetThread returns the Thread field if non-nil, zero value otherwise.

### GetThreadOk

`func (o *GetThreadResponse) GetThreadOk() (*SpatioThread, bool)`

GetThreadOk returns a tuple with the Thread field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetThread

`func (o *GetThreadResponse) SetThread(v SpatioThread)`

SetThread sets Thread field to given value.


### GetProvider

`func (o *GetThreadResponse) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *GetThreadResponse) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *GetThreadResponse) SetProvider(v string)`

SetProvider sets Provider field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


