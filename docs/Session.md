# Session

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**IpAddress** | Pointer to **string** |  | [optional] 
**UserAgent** | Pointer to **string** |  | [optional] 
**DeviceType** | Pointer to **string** |  | [optional] 
**Browser** | Pointer to **string** |  | [optional] 
**Os** | Pointer to **string** |  | [optional] 
**Country** | Pointer to **string** |  | [optional] 
**City** | Pointer to **string** |  | [optional] 
**CreatedAt** | Pointer to **time.Time** |  | [optional] 
**LastActiveAt** | Pointer to **time.Time** |  | [optional] 
**IsCurrent** | Pointer to **bool** |  | [optional] 

## Methods

### NewSession

`func NewSession(id string, ) *Session`

NewSession instantiates a new Session object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSessionWithDefaults

`func NewSessionWithDefaults() *Session`

NewSessionWithDefaults instantiates a new Session object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Session) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Session) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Session) SetId(v string)`

SetId sets Id field to given value.


### GetIpAddress

`func (o *Session) GetIpAddress() string`

GetIpAddress returns the IpAddress field if non-nil, zero value otherwise.

### GetIpAddressOk

`func (o *Session) GetIpAddressOk() (*string, bool)`

GetIpAddressOk returns a tuple with the IpAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIpAddress

`func (o *Session) SetIpAddress(v string)`

SetIpAddress sets IpAddress field to given value.

### HasIpAddress

`func (o *Session) HasIpAddress() bool`

HasIpAddress returns a boolean if a field has been set.

### GetUserAgent

`func (o *Session) GetUserAgent() string`

GetUserAgent returns the UserAgent field if non-nil, zero value otherwise.

### GetUserAgentOk

`func (o *Session) GetUserAgentOk() (*string, bool)`

GetUserAgentOk returns a tuple with the UserAgent field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserAgent

`func (o *Session) SetUserAgent(v string)`

SetUserAgent sets UserAgent field to given value.

### HasUserAgent

`func (o *Session) HasUserAgent() bool`

HasUserAgent returns a boolean if a field has been set.

### GetDeviceType

`func (o *Session) GetDeviceType() string`

GetDeviceType returns the DeviceType field if non-nil, zero value otherwise.

### GetDeviceTypeOk

`func (o *Session) GetDeviceTypeOk() (*string, bool)`

GetDeviceTypeOk returns a tuple with the DeviceType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeviceType

`func (o *Session) SetDeviceType(v string)`

SetDeviceType sets DeviceType field to given value.

### HasDeviceType

`func (o *Session) HasDeviceType() bool`

HasDeviceType returns a boolean if a field has been set.

### GetBrowser

`func (o *Session) GetBrowser() string`

GetBrowser returns the Browser field if non-nil, zero value otherwise.

### GetBrowserOk

`func (o *Session) GetBrowserOk() (*string, bool)`

GetBrowserOk returns a tuple with the Browser field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBrowser

`func (o *Session) SetBrowser(v string)`

SetBrowser sets Browser field to given value.

### HasBrowser

`func (o *Session) HasBrowser() bool`

HasBrowser returns a boolean if a field has been set.

### GetOs

`func (o *Session) GetOs() string`

GetOs returns the Os field if non-nil, zero value otherwise.

### GetOsOk

`func (o *Session) GetOsOk() (*string, bool)`

GetOsOk returns a tuple with the Os field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOs

`func (o *Session) SetOs(v string)`

SetOs sets Os field to given value.

### HasOs

`func (o *Session) HasOs() bool`

HasOs returns a boolean if a field has been set.

### GetCountry

`func (o *Session) GetCountry() string`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *Session) GetCountryOk() (*string, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *Session) SetCountry(v string)`

SetCountry sets Country field to given value.

### HasCountry

`func (o *Session) HasCountry() bool`

HasCountry returns a boolean if a field has been set.

### GetCity

`func (o *Session) GetCity() string`

GetCity returns the City field if non-nil, zero value otherwise.

### GetCityOk

`func (o *Session) GetCityOk() (*string, bool)`

GetCityOk returns a tuple with the City field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCity

`func (o *Session) SetCity(v string)`

SetCity sets City field to given value.

### HasCity

`func (o *Session) HasCity() bool`

HasCity returns a boolean if a field has been set.

### GetCreatedAt

`func (o *Session) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Session) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Session) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *Session) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetLastActiveAt

`func (o *Session) GetLastActiveAt() time.Time`

GetLastActiveAt returns the LastActiveAt field if non-nil, zero value otherwise.

### GetLastActiveAtOk

`func (o *Session) GetLastActiveAtOk() (*time.Time, bool)`

GetLastActiveAtOk returns a tuple with the LastActiveAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastActiveAt

`func (o *Session) SetLastActiveAt(v time.Time)`

SetLastActiveAt sets LastActiveAt field to given value.

### HasLastActiveAt

`func (o *Session) HasLastActiveAt() bool`

HasLastActiveAt returns a boolean if a field has been set.

### GetIsCurrent

`func (o *Session) GetIsCurrent() bool`

GetIsCurrent returns the IsCurrent field if non-nil, zero value otherwise.

### GetIsCurrentOk

`func (o *Session) GetIsCurrentOk() (*bool, bool)`

GetIsCurrentOk returns a tuple with the IsCurrent field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsCurrent

`func (o *Session) SetIsCurrent(v bool)`

SetIsCurrent sets IsCurrent field to given value.

### HasIsCurrent

`func (o *Session) HasIsCurrent() bool`

HasIsCurrent returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


