# CalendarCapabilitiesResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AccountId** | **string** |  | 
**ProviderId** | **string** |  | 
**Capabilities** | **map[string]interface{}** | Per-account feature gate. The renderer reads these to enable/ disable form fields (recurrence pickers, attendee inputs, etc.) based on what the underlying provider supports.  | 

## Methods

### NewCalendarCapabilitiesResponse

`func NewCalendarCapabilitiesResponse(accountId string, providerId string, capabilities map[string]interface{}, ) *CalendarCapabilitiesResponse`

NewCalendarCapabilitiesResponse instantiates a new CalendarCapabilitiesResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCalendarCapabilitiesResponseWithDefaults

`func NewCalendarCapabilitiesResponseWithDefaults() *CalendarCapabilitiesResponse`

NewCalendarCapabilitiesResponseWithDefaults instantiates a new CalendarCapabilitiesResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAccountId

`func (o *CalendarCapabilitiesResponse) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *CalendarCapabilitiesResponse) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *CalendarCapabilitiesResponse) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.


### GetProviderId

`func (o *CalendarCapabilitiesResponse) GetProviderId() string`

GetProviderId returns the ProviderId field if non-nil, zero value otherwise.

### GetProviderIdOk

`func (o *CalendarCapabilitiesResponse) GetProviderIdOk() (*string, bool)`

GetProviderIdOk returns a tuple with the ProviderId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProviderId

`func (o *CalendarCapabilitiesResponse) SetProviderId(v string)`

SetProviderId sets ProviderId field to given value.


### GetCapabilities

`func (o *CalendarCapabilitiesResponse) GetCapabilities() map[string]interface{}`

GetCapabilities returns the Capabilities field if non-nil, zero value otherwise.

### GetCapabilitiesOk

`func (o *CalendarCapabilitiesResponse) GetCapabilitiesOk() (*map[string]interface{}, bool)`

GetCapabilitiesOk returns a tuple with the Capabilities field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCapabilities

`func (o *CalendarCapabilitiesResponse) SetCapabilities(v map[string]interface{})`

SetCapabilities sets Capabilities field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


