# FederatedSearch200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Items** | [**[]FederatedSearch200ResponseItemsInner**](FederatedSearch200ResponseItemsInner.md) |  | 
**NextPageTokens** | Pointer to **map[string]string** |  | [optional] 
**PerPlatform** | [**map[string]FederatedSearch200ResponsePerPlatformValue**](FederatedSearch200ResponsePerPlatformValue.md) |  | 
**Errors** | Pointer to **map[string]string** | Per-platform errors. Other platforms still return results. | [optional] 
**TotalReturned** | **int32** |  | 
**Took** | **string** | Aggregate wall-clock time for the fan-out, e.g. \&quot;120ms\&quot;. | 

## Methods

### NewFederatedSearch200Response

`func NewFederatedSearch200Response(items []FederatedSearch200ResponseItemsInner, perPlatform map[string]FederatedSearch200ResponsePerPlatformValue, totalReturned int32, took string, ) *FederatedSearch200Response`

NewFederatedSearch200Response instantiates a new FederatedSearch200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewFederatedSearch200ResponseWithDefaults

`func NewFederatedSearch200ResponseWithDefaults() *FederatedSearch200Response`

NewFederatedSearch200ResponseWithDefaults instantiates a new FederatedSearch200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetItems

`func (o *FederatedSearch200Response) GetItems() []FederatedSearch200ResponseItemsInner`

GetItems returns the Items field if non-nil, zero value otherwise.

### GetItemsOk

`func (o *FederatedSearch200Response) GetItemsOk() (*[]FederatedSearch200ResponseItemsInner, bool)`

GetItemsOk returns a tuple with the Items field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItems

`func (o *FederatedSearch200Response) SetItems(v []FederatedSearch200ResponseItemsInner)`

SetItems sets Items field to given value.


### GetNextPageTokens

`func (o *FederatedSearch200Response) GetNextPageTokens() map[string]string`

GetNextPageTokens returns the NextPageTokens field if non-nil, zero value otherwise.

### GetNextPageTokensOk

`func (o *FederatedSearch200Response) GetNextPageTokensOk() (*map[string]string, bool)`

GetNextPageTokensOk returns a tuple with the NextPageTokens field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextPageTokens

`func (o *FederatedSearch200Response) SetNextPageTokens(v map[string]string)`

SetNextPageTokens sets NextPageTokens field to given value.

### HasNextPageTokens

`func (o *FederatedSearch200Response) HasNextPageTokens() bool`

HasNextPageTokens returns a boolean if a field has been set.

### GetPerPlatform

`func (o *FederatedSearch200Response) GetPerPlatform() map[string]FederatedSearch200ResponsePerPlatformValue`

GetPerPlatform returns the PerPlatform field if non-nil, zero value otherwise.

### GetPerPlatformOk

`func (o *FederatedSearch200Response) GetPerPlatformOk() (*map[string]FederatedSearch200ResponsePerPlatformValue, bool)`

GetPerPlatformOk returns a tuple with the PerPlatform field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPerPlatform

`func (o *FederatedSearch200Response) SetPerPlatform(v map[string]FederatedSearch200ResponsePerPlatformValue)`

SetPerPlatform sets PerPlatform field to given value.


### GetErrors

`func (o *FederatedSearch200Response) GetErrors() map[string]string`

GetErrors returns the Errors field if non-nil, zero value otherwise.

### GetErrorsOk

`func (o *FederatedSearch200Response) GetErrorsOk() (*map[string]string, bool)`

GetErrorsOk returns a tuple with the Errors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrors

`func (o *FederatedSearch200Response) SetErrors(v map[string]string)`

SetErrors sets Errors field to given value.

### HasErrors

`func (o *FederatedSearch200Response) HasErrors() bool`

HasErrors returns a boolean if a field has been set.

### GetTotalReturned

`func (o *FederatedSearch200Response) GetTotalReturned() int32`

GetTotalReturned returns the TotalReturned field if non-nil, zero value otherwise.

### GetTotalReturnedOk

`func (o *FederatedSearch200Response) GetTotalReturnedOk() (*int32, bool)`

GetTotalReturnedOk returns a tuple with the TotalReturned field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalReturned

`func (o *FederatedSearch200Response) SetTotalReturned(v int32)`

SetTotalReturned sets TotalReturned field to given value.


### GetTook

`func (o *FederatedSearch200Response) GetTook() string`

GetTook returns the Took field if non-nil, zero value otherwise.

### GetTookOk

`func (o *FederatedSearch200Response) GetTookOk() (*string, bool)`

GetTookOk returns a tuple with the Took field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTook

`func (o *FederatedSearch200Response) SetTook(v string)`

SetTook sets Took field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


