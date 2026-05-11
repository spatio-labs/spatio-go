# SpatioConnection

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Name** | Pointer to **string** |  | [optional] 
**Category** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **string** |  | [optional] 
**AuthType** | Pointer to **string** |  | [optional] 
**Connected** | Pointer to **bool** |  | [optional] 
**ConnectedAccounts** | Pointer to **[]map[string]interface{}** |  | [optional] 
**Capabilities** | Pointer to **map[string]interface{}** |  | [optional] 
**GradientFrom** | Pointer to **string** |  | [optional] 
**GradientTo** | Pointer to **string** |  | [optional] 
**Icon** | Pointer to **string** |  | [optional] 

## Methods

### NewSpatioConnection

`func NewSpatioConnection(id string, ) *SpatioConnection`

NewSpatioConnection instantiates a new SpatioConnection object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSpatioConnectionWithDefaults

`func NewSpatioConnectionWithDefaults() *SpatioConnection`

NewSpatioConnectionWithDefaults instantiates a new SpatioConnection object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *SpatioConnection) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *SpatioConnection) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *SpatioConnection) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *SpatioConnection) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *SpatioConnection) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *SpatioConnection) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *SpatioConnection) HasName() bool`

HasName returns a boolean if a field has been set.

### GetCategory

`func (o *SpatioConnection) GetCategory() string`

GetCategory returns the Category field if non-nil, zero value otherwise.

### GetCategoryOk

`func (o *SpatioConnection) GetCategoryOk() (*string, bool)`

GetCategoryOk returns a tuple with the Category field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCategory

`func (o *SpatioConnection) SetCategory(v string)`

SetCategory sets Category field to given value.

### HasCategory

`func (o *SpatioConnection) HasCategory() bool`

HasCategory returns a boolean if a field has been set.

### GetDescription

`func (o *SpatioConnection) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *SpatioConnection) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *SpatioConnection) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *SpatioConnection) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetAuthType

`func (o *SpatioConnection) GetAuthType() string`

GetAuthType returns the AuthType field if non-nil, zero value otherwise.

### GetAuthTypeOk

`func (o *SpatioConnection) GetAuthTypeOk() (*string, bool)`

GetAuthTypeOk returns a tuple with the AuthType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAuthType

`func (o *SpatioConnection) SetAuthType(v string)`

SetAuthType sets AuthType field to given value.

### HasAuthType

`func (o *SpatioConnection) HasAuthType() bool`

HasAuthType returns a boolean if a field has been set.

### GetConnected

`func (o *SpatioConnection) GetConnected() bool`

GetConnected returns the Connected field if non-nil, zero value otherwise.

### GetConnectedOk

`func (o *SpatioConnection) GetConnectedOk() (*bool, bool)`

GetConnectedOk returns a tuple with the Connected field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConnected

`func (o *SpatioConnection) SetConnected(v bool)`

SetConnected sets Connected field to given value.

### HasConnected

`func (o *SpatioConnection) HasConnected() bool`

HasConnected returns a boolean if a field has been set.

### GetConnectedAccounts

`func (o *SpatioConnection) GetConnectedAccounts() []map[string]interface{}`

GetConnectedAccounts returns the ConnectedAccounts field if non-nil, zero value otherwise.

### GetConnectedAccountsOk

`func (o *SpatioConnection) GetConnectedAccountsOk() (*[]map[string]interface{}, bool)`

GetConnectedAccountsOk returns a tuple with the ConnectedAccounts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConnectedAccounts

`func (o *SpatioConnection) SetConnectedAccounts(v []map[string]interface{})`

SetConnectedAccounts sets ConnectedAccounts field to given value.

### HasConnectedAccounts

`func (o *SpatioConnection) HasConnectedAccounts() bool`

HasConnectedAccounts returns a boolean if a field has been set.

### SetConnectedAccountsNil

`func (o *SpatioConnection) SetConnectedAccountsNil(b bool)`

 SetConnectedAccountsNil sets the value for ConnectedAccounts to be an explicit nil

### UnsetConnectedAccounts
`func (o *SpatioConnection) UnsetConnectedAccounts()`

UnsetConnectedAccounts ensures that no value is present for ConnectedAccounts, not even an explicit nil
### GetCapabilities

`func (o *SpatioConnection) GetCapabilities() map[string]interface{}`

GetCapabilities returns the Capabilities field if non-nil, zero value otherwise.

### GetCapabilitiesOk

`func (o *SpatioConnection) GetCapabilitiesOk() (*map[string]interface{}, bool)`

GetCapabilitiesOk returns a tuple with the Capabilities field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCapabilities

`func (o *SpatioConnection) SetCapabilities(v map[string]interface{})`

SetCapabilities sets Capabilities field to given value.

### HasCapabilities

`func (o *SpatioConnection) HasCapabilities() bool`

HasCapabilities returns a boolean if a field has been set.

### GetGradientFrom

`func (o *SpatioConnection) GetGradientFrom() string`

GetGradientFrom returns the GradientFrom field if non-nil, zero value otherwise.

### GetGradientFromOk

`func (o *SpatioConnection) GetGradientFromOk() (*string, bool)`

GetGradientFromOk returns a tuple with the GradientFrom field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGradientFrom

`func (o *SpatioConnection) SetGradientFrom(v string)`

SetGradientFrom sets GradientFrom field to given value.

### HasGradientFrom

`func (o *SpatioConnection) HasGradientFrom() bool`

HasGradientFrom returns a boolean if a field has been set.

### GetGradientTo

`func (o *SpatioConnection) GetGradientTo() string`

GetGradientTo returns the GradientTo field if non-nil, zero value otherwise.

### GetGradientToOk

`func (o *SpatioConnection) GetGradientToOk() (*string, bool)`

GetGradientToOk returns a tuple with the GradientTo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGradientTo

`func (o *SpatioConnection) SetGradientTo(v string)`

SetGradientTo sets GradientTo field to given value.

### HasGradientTo

`func (o *SpatioConnection) HasGradientTo() bool`

HasGradientTo returns a boolean if a field has been set.

### GetIcon

`func (o *SpatioConnection) GetIcon() string`

GetIcon returns the Icon field if non-nil, zero value otherwise.

### GetIconOk

`func (o *SpatioConnection) GetIconOk() (*string, bool)`

GetIconOk returns a tuple with the Icon field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIcon

`func (o *SpatioConnection) SetIcon(v string)`

SetIcon sets Icon field to given value.

### HasIcon

`func (o *SpatioConnection) HasIcon() bool`

HasIcon returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


