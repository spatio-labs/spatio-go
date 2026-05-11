# AppListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Apps** | [**[]App**](App.md) |  | 
**Total** | Pointer to **int32** |  | [optional] 

## Methods

### NewAppListResponse

`func NewAppListResponse(apps []App, ) *AppListResponse`

NewAppListResponse instantiates a new AppListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAppListResponseWithDefaults

`func NewAppListResponseWithDefaults() *AppListResponse`

NewAppListResponseWithDefaults instantiates a new AppListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetApps

`func (o *AppListResponse) GetApps() []App`

GetApps returns the Apps field if non-nil, zero value otherwise.

### GetAppsOk

`func (o *AppListResponse) GetAppsOk() (*[]App, bool)`

GetAppsOk returns a tuple with the Apps field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApps

`func (o *AppListResponse) SetApps(v []App)`

SetApps sets Apps field to given value.


### SetAppsNil

`func (o *AppListResponse) SetAppsNil(b bool)`

 SetAppsNil sets the value for Apps to be an explicit nil

### UnsetApps
`func (o *AppListResponse) UnsetApps()`

UnsetApps ensures that no value is present for Apps, not even an explicit nil
### GetTotal

`func (o *AppListResponse) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *AppListResponse) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *AppListResponse) SetTotal(v int32)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *AppListResponse) HasTotal() bool`

HasTotal returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


