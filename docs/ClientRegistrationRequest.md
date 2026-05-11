# ClientRegistrationRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ClientName** | **string** |  | 
**RedirectUris** | **[]string** |  | 
**GrantTypes** | Pointer to **[]string** |  | [optional] [default to {"authorization_code", "refresh_token"}]
**ResponseTypes** | Pointer to **[]string** |  | [optional] [default to {"code"}]
**Scope** | Pointer to **string** | Space-separated scope list. Defaults to &#x60;read:*&#x60;. | [optional] 
**TokenEndpointAuthMethod** | Pointer to **string** |  | [optional] [default to "none"]
**ClientUri** | Pointer to **string** |  | [optional] 
**LogoUri** | Pointer to **string** |  | [optional] 
**PolicyUri** | Pointer to **string** |  | [optional] 
**TosUri** | Pointer to **string** |  | [optional] 

## Methods

### NewClientRegistrationRequest

`func NewClientRegistrationRequest(clientName string, redirectUris []string, ) *ClientRegistrationRequest`

NewClientRegistrationRequest instantiates a new ClientRegistrationRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewClientRegistrationRequestWithDefaults

`func NewClientRegistrationRequestWithDefaults() *ClientRegistrationRequest`

NewClientRegistrationRequestWithDefaults instantiates a new ClientRegistrationRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetClientName

`func (o *ClientRegistrationRequest) GetClientName() string`

GetClientName returns the ClientName field if non-nil, zero value otherwise.

### GetClientNameOk

`func (o *ClientRegistrationRequest) GetClientNameOk() (*string, bool)`

GetClientNameOk returns a tuple with the ClientName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientName

`func (o *ClientRegistrationRequest) SetClientName(v string)`

SetClientName sets ClientName field to given value.


### GetRedirectUris

`func (o *ClientRegistrationRequest) GetRedirectUris() []string`

GetRedirectUris returns the RedirectUris field if non-nil, zero value otherwise.

### GetRedirectUrisOk

`func (o *ClientRegistrationRequest) GetRedirectUrisOk() (*[]string, bool)`

GetRedirectUrisOk returns a tuple with the RedirectUris field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRedirectUris

`func (o *ClientRegistrationRequest) SetRedirectUris(v []string)`

SetRedirectUris sets RedirectUris field to given value.


### GetGrantTypes

`func (o *ClientRegistrationRequest) GetGrantTypes() []string`

GetGrantTypes returns the GrantTypes field if non-nil, zero value otherwise.

### GetGrantTypesOk

`func (o *ClientRegistrationRequest) GetGrantTypesOk() (*[]string, bool)`

GetGrantTypesOk returns a tuple with the GrantTypes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGrantTypes

`func (o *ClientRegistrationRequest) SetGrantTypes(v []string)`

SetGrantTypes sets GrantTypes field to given value.

### HasGrantTypes

`func (o *ClientRegistrationRequest) HasGrantTypes() bool`

HasGrantTypes returns a boolean if a field has been set.

### GetResponseTypes

`func (o *ClientRegistrationRequest) GetResponseTypes() []string`

GetResponseTypes returns the ResponseTypes field if non-nil, zero value otherwise.

### GetResponseTypesOk

`func (o *ClientRegistrationRequest) GetResponseTypesOk() (*[]string, bool)`

GetResponseTypesOk returns a tuple with the ResponseTypes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseTypes

`func (o *ClientRegistrationRequest) SetResponseTypes(v []string)`

SetResponseTypes sets ResponseTypes field to given value.

### HasResponseTypes

`func (o *ClientRegistrationRequest) HasResponseTypes() bool`

HasResponseTypes returns a boolean if a field has been set.

### GetScope

`func (o *ClientRegistrationRequest) GetScope() string`

GetScope returns the Scope field if non-nil, zero value otherwise.

### GetScopeOk

`func (o *ClientRegistrationRequest) GetScopeOk() (*string, bool)`

GetScopeOk returns a tuple with the Scope field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScope

`func (o *ClientRegistrationRequest) SetScope(v string)`

SetScope sets Scope field to given value.

### HasScope

`func (o *ClientRegistrationRequest) HasScope() bool`

HasScope returns a boolean if a field has been set.

### GetTokenEndpointAuthMethod

`func (o *ClientRegistrationRequest) GetTokenEndpointAuthMethod() string`

GetTokenEndpointAuthMethod returns the TokenEndpointAuthMethod field if non-nil, zero value otherwise.

### GetTokenEndpointAuthMethodOk

`func (o *ClientRegistrationRequest) GetTokenEndpointAuthMethodOk() (*string, bool)`

GetTokenEndpointAuthMethodOk returns a tuple with the TokenEndpointAuthMethod field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTokenEndpointAuthMethod

`func (o *ClientRegistrationRequest) SetTokenEndpointAuthMethod(v string)`

SetTokenEndpointAuthMethod sets TokenEndpointAuthMethod field to given value.

### HasTokenEndpointAuthMethod

`func (o *ClientRegistrationRequest) HasTokenEndpointAuthMethod() bool`

HasTokenEndpointAuthMethod returns a boolean if a field has been set.

### GetClientUri

`func (o *ClientRegistrationRequest) GetClientUri() string`

GetClientUri returns the ClientUri field if non-nil, zero value otherwise.

### GetClientUriOk

`func (o *ClientRegistrationRequest) GetClientUriOk() (*string, bool)`

GetClientUriOk returns a tuple with the ClientUri field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientUri

`func (o *ClientRegistrationRequest) SetClientUri(v string)`

SetClientUri sets ClientUri field to given value.

### HasClientUri

`func (o *ClientRegistrationRequest) HasClientUri() bool`

HasClientUri returns a boolean if a field has been set.

### GetLogoUri

`func (o *ClientRegistrationRequest) GetLogoUri() string`

GetLogoUri returns the LogoUri field if non-nil, zero value otherwise.

### GetLogoUriOk

`func (o *ClientRegistrationRequest) GetLogoUriOk() (*string, bool)`

GetLogoUriOk returns a tuple with the LogoUri field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogoUri

`func (o *ClientRegistrationRequest) SetLogoUri(v string)`

SetLogoUri sets LogoUri field to given value.

### HasLogoUri

`func (o *ClientRegistrationRequest) HasLogoUri() bool`

HasLogoUri returns a boolean if a field has been set.

### GetPolicyUri

`func (o *ClientRegistrationRequest) GetPolicyUri() string`

GetPolicyUri returns the PolicyUri field if non-nil, zero value otherwise.

### GetPolicyUriOk

`func (o *ClientRegistrationRequest) GetPolicyUriOk() (*string, bool)`

GetPolicyUriOk returns a tuple with the PolicyUri field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolicyUri

`func (o *ClientRegistrationRequest) SetPolicyUri(v string)`

SetPolicyUri sets PolicyUri field to given value.

### HasPolicyUri

`func (o *ClientRegistrationRequest) HasPolicyUri() bool`

HasPolicyUri returns a boolean if a field has been set.

### GetTosUri

`func (o *ClientRegistrationRequest) GetTosUri() string`

GetTosUri returns the TosUri field if non-nil, zero value otherwise.

### GetTosUriOk

`func (o *ClientRegistrationRequest) GetTosUriOk() (*string, bool)`

GetTosUriOk returns a tuple with the TosUri field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTosUri

`func (o *ClientRegistrationRequest) SetTosUri(v string)`

SetTosUri sets TosUri field to given value.

### HasTosUri

`func (o *ClientRegistrationRequest) HasTosUri() bool`

HasTosUri returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


