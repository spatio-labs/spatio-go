# CalendarProviderInfo

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Stable provider id (e.g. &#x60;google-calendar&#x60;, &#x60;native-calendar&#x60;). | 
**Name** | **string** |  | 
**DisplayName** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **string** |  | [optional] 
**IsSystem** | Pointer to **bool** | &#x60;true&#x60; for built-in providers (the native calendar). | [optional] 

## Methods

### NewCalendarProviderInfo

`func NewCalendarProviderInfo(id string, name string, ) *CalendarProviderInfo`

NewCalendarProviderInfo instantiates a new CalendarProviderInfo object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCalendarProviderInfoWithDefaults

`func NewCalendarProviderInfoWithDefaults() *CalendarProviderInfo`

NewCalendarProviderInfoWithDefaults instantiates a new CalendarProviderInfo object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *CalendarProviderInfo) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *CalendarProviderInfo) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *CalendarProviderInfo) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *CalendarProviderInfo) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CalendarProviderInfo) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CalendarProviderInfo) SetName(v string)`

SetName sets Name field to given value.


### GetDisplayName

`func (o *CalendarProviderInfo) GetDisplayName() string`

GetDisplayName returns the DisplayName field if non-nil, zero value otherwise.

### GetDisplayNameOk

`func (o *CalendarProviderInfo) GetDisplayNameOk() (*string, bool)`

GetDisplayNameOk returns a tuple with the DisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayName

`func (o *CalendarProviderInfo) SetDisplayName(v string)`

SetDisplayName sets DisplayName field to given value.

### HasDisplayName

`func (o *CalendarProviderInfo) HasDisplayName() bool`

HasDisplayName returns a boolean if a field has been set.

### GetDescription

`func (o *CalendarProviderInfo) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *CalendarProviderInfo) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *CalendarProviderInfo) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *CalendarProviderInfo) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetIsSystem

`func (o *CalendarProviderInfo) GetIsSystem() bool`

GetIsSystem returns the IsSystem field if non-nil, zero value otherwise.

### GetIsSystemOk

`func (o *CalendarProviderInfo) GetIsSystemOk() (*bool, bool)`

GetIsSystemOk returns a tuple with the IsSystem field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsSystem

`func (o *CalendarProviderInfo) SetIsSystem(v bool)`

SetIsSystem sets IsSystem field to given value.

### HasIsSystem

`func (o *CalendarProviderInfo) HasIsSystem() bool`

HasIsSystem returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


