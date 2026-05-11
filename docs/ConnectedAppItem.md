# ConnectedAppItem

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ClientId** | **string** |  | 
**ClientName** | **string** |  | 
**LogoUri** | Pointer to **string** |  | [optional] 
**ClientUri** | Pointer to **string** |  | [optional] 
**PolicyUri** | Pointer to **string** |  | [optional] 
**TosUri** | Pointer to **string** |  | [optional] 
**Scopes** | **[]string** |  | 
**ScopeLabels** | **[]string** |  | 
**GrantedAt** | **time.Time** |  | 

## Methods

### NewConnectedAppItem

`func NewConnectedAppItem(clientId string, clientName string, scopes []string, scopeLabels []string, grantedAt time.Time, ) *ConnectedAppItem`

NewConnectedAppItem instantiates a new ConnectedAppItem object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewConnectedAppItemWithDefaults

`func NewConnectedAppItemWithDefaults() *ConnectedAppItem`

NewConnectedAppItemWithDefaults instantiates a new ConnectedAppItem object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetClientId

`func (o *ConnectedAppItem) GetClientId() string`

GetClientId returns the ClientId field if non-nil, zero value otherwise.

### GetClientIdOk

`func (o *ConnectedAppItem) GetClientIdOk() (*string, bool)`

GetClientIdOk returns a tuple with the ClientId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientId

`func (o *ConnectedAppItem) SetClientId(v string)`

SetClientId sets ClientId field to given value.


### GetClientName

`func (o *ConnectedAppItem) GetClientName() string`

GetClientName returns the ClientName field if non-nil, zero value otherwise.

### GetClientNameOk

`func (o *ConnectedAppItem) GetClientNameOk() (*string, bool)`

GetClientNameOk returns a tuple with the ClientName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientName

`func (o *ConnectedAppItem) SetClientName(v string)`

SetClientName sets ClientName field to given value.


### GetLogoUri

`func (o *ConnectedAppItem) GetLogoUri() string`

GetLogoUri returns the LogoUri field if non-nil, zero value otherwise.

### GetLogoUriOk

`func (o *ConnectedAppItem) GetLogoUriOk() (*string, bool)`

GetLogoUriOk returns a tuple with the LogoUri field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogoUri

`func (o *ConnectedAppItem) SetLogoUri(v string)`

SetLogoUri sets LogoUri field to given value.

### HasLogoUri

`func (o *ConnectedAppItem) HasLogoUri() bool`

HasLogoUri returns a boolean if a field has been set.

### GetClientUri

`func (o *ConnectedAppItem) GetClientUri() string`

GetClientUri returns the ClientUri field if non-nil, zero value otherwise.

### GetClientUriOk

`func (o *ConnectedAppItem) GetClientUriOk() (*string, bool)`

GetClientUriOk returns a tuple with the ClientUri field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientUri

`func (o *ConnectedAppItem) SetClientUri(v string)`

SetClientUri sets ClientUri field to given value.

### HasClientUri

`func (o *ConnectedAppItem) HasClientUri() bool`

HasClientUri returns a boolean if a field has been set.

### GetPolicyUri

`func (o *ConnectedAppItem) GetPolicyUri() string`

GetPolicyUri returns the PolicyUri field if non-nil, zero value otherwise.

### GetPolicyUriOk

`func (o *ConnectedAppItem) GetPolicyUriOk() (*string, bool)`

GetPolicyUriOk returns a tuple with the PolicyUri field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolicyUri

`func (o *ConnectedAppItem) SetPolicyUri(v string)`

SetPolicyUri sets PolicyUri field to given value.

### HasPolicyUri

`func (o *ConnectedAppItem) HasPolicyUri() bool`

HasPolicyUri returns a boolean if a field has been set.

### GetTosUri

`func (o *ConnectedAppItem) GetTosUri() string`

GetTosUri returns the TosUri field if non-nil, zero value otherwise.

### GetTosUriOk

`func (o *ConnectedAppItem) GetTosUriOk() (*string, bool)`

GetTosUriOk returns a tuple with the TosUri field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTosUri

`func (o *ConnectedAppItem) SetTosUri(v string)`

SetTosUri sets TosUri field to given value.

### HasTosUri

`func (o *ConnectedAppItem) HasTosUri() bool`

HasTosUri returns a boolean if a field has been set.

### GetScopes

`func (o *ConnectedAppItem) GetScopes() []string`

GetScopes returns the Scopes field if non-nil, zero value otherwise.

### GetScopesOk

`func (o *ConnectedAppItem) GetScopesOk() (*[]string, bool)`

GetScopesOk returns a tuple with the Scopes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScopes

`func (o *ConnectedAppItem) SetScopes(v []string)`

SetScopes sets Scopes field to given value.


### GetScopeLabels

`func (o *ConnectedAppItem) GetScopeLabels() []string`

GetScopeLabels returns the ScopeLabels field if non-nil, zero value otherwise.

### GetScopeLabelsOk

`func (o *ConnectedAppItem) GetScopeLabelsOk() (*[]string, bool)`

GetScopeLabelsOk returns a tuple with the ScopeLabels field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScopeLabels

`func (o *ConnectedAppItem) SetScopeLabels(v []string)`

SetScopeLabels sets ScopeLabels field to given value.


### GetGrantedAt

`func (o *ConnectedAppItem) GetGrantedAt() time.Time`

GetGrantedAt returns the GrantedAt field if non-nil, zero value otherwise.

### GetGrantedAtOk

`func (o *ConnectedAppItem) GetGrantedAtOk() (*time.Time, bool)`

GetGrantedAtOk returns a tuple with the GrantedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGrantedAt

`func (o *ConnectedAppItem) SetGrantedAt(v time.Time)`

SetGrantedAt sets GrantedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


