# TaskProvidersInfo

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Providers** | **[]string** | Registered provider ids (e.g. &#x60;native-tasks&#x60;, &#x60;linear&#x60;). | 
**Platform** | [**TaskProvidersInfoPlatform**](TaskProvidersInfoPlatform.md) |  | 

## Methods

### NewTaskProvidersInfo

`func NewTaskProvidersInfo(providers []string, platform TaskProvidersInfoPlatform, ) *TaskProvidersInfo`

NewTaskProvidersInfo instantiates a new TaskProvidersInfo object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTaskProvidersInfoWithDefaults

`func NewTaskProvidersInfoWithDefaults() *TaskProvidersInfo`

NewTaskProvidersInfoWithDefaults instantiates a new TaskProvidersInfo object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetProviders

`func (o *TaskProvidersInfo) GetProviders() []string`

GetProviders returns the Providers field if non-nil, zero value otherwise.

### GetProvidersOk

`func (o *TaskProvidersInfo) GetProvidersOk() (*[]string, bool)`

GetProvidersOk returns a tuple with the Providers field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProviders

`func (o *TaskProvidersInfo) SetProviders(v []string)`

SetProviders sets Providers field to given value.


### GetPlatform

`func (o *TaskProvidersInfo) GetPlatform() TaskProvidersInfoPlatform`

GetPlatform returns the Platform field if non-nil, zero value otherwise.

### GetPlatformOk

`func (o *TaskProvidersInfo) GetPlatformOk() (*TaskProvidersInfoPlatform, bool)`

GetPlatformOk returns a tuple with the Platform field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPlatform

`func (o *TaskProvidersInfo) SetPlatform(v TaskProvidersInfoPlatform)`

SetPlatform sets Platform field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


