# ClientRegistrationResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ClientId** | **string** |  | 
**ClientSecret** | Pointer to **string** | Only returned when token_endpoint_auth_method is client_secret_*. | [optional] 
**ClientName** | **string** |  | 
**RedirectUris** | **[]string** |  | 
**GrantTypes** | Pointer to **[]string** |  | [optional] 
**ResponseTypes** | Pointer to **[]string** |  | [optional] 
**Scope** | Pointer to **string** |  | [optional] 
**TokenEndpointAuthMethod** | Pointer to **string** |  | [optional] 
**RegistrationAccessToken** | **string** |  | 
**RegistrationClientUri** | Pointer to **string** |  | [optional] 
**ClientIdIssuedAt** | **int32** |  | 

## Methods

### NewClientRegistrationResponse

`func NewClientRegistrationResponse(clientId string, clientName string, redirectUris []string, registrationAccessToken string, clientIdIssuedAt int32, ) *ClientRegistrationResponse`

NewClientRegistrationResponse instantiates a new ClientRegistrationResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewClientRegistrationResponseWithDefaults

`func NewClientRegistrationResponseWithDefaults() *ClientRegistrationResponse`

NewClientRegistrationResponseWithDefaults instantiates a new ClientRegistrationResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetClientId

`func (o *ClientRegistrationResponse) GetClientId() string`

GetClientId returns the ClientId field if non-nil, zero value otherwise.

### GetClientIdOk

`func (o *ClientRegistrationResponse) GetClientIdOk() (*string, bool)`

GetClientIdOk returns a tuple with the ClientId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientId

`func (o *ClientRegistrationResponse) SetClientId(v string)`

SetClientId sets ClientId field to given value.


### GetClientSecret

`func (o *ClientRegistrationResponse) GetClientSecret() string`

GetClientSecret returns the ClientSecret field if non-nil, zero value otherwise.

### GetClientSecretOk

`func (o *ClientRegistrationResponse) GetClientSecretOk() (*string, bool)`

GetClientSecretOk returns a tuple with the ClientSecret field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientSecret

`func (o *ClientRegistrationResponse) SetClientSecret(v string)`

SetClientSecret sets ClientSecret field to given value.

### HasClientSecret

`func (o *ClientRegistrationResponse) HasClientSecret() bool`

HasClientSecret returns a boolean if a field has been set.

### GetClientName

`func (o *ClientRegistrationResponse) GetClientName() string`

GetClientName returns the ClientName field if non-nil, zero value otherwise.

### GetClientNameOk

`func (o *ClientRegistrationResponse) GetClientNameOk() (*string, bool)`

GetClientNameOk returns a tuple with the ClientName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientName

`func (o *ClientRegistrationResponse) SetClientName(v string)`

SetClientName sets ClientName field to given value.


### GetRedirectUris

`func (o *ClientRegistrationResponse) GetRedirectUris() []string`

GetRedirectUris returns the RedirectUris field if non-nil, zero value otherwise.

### GetRedirectUrisOk

`func (o *ClientRegistrationResponse) GetRedirectUrisOk() (*[]string, bool)`

GetRedirectUrisOk returns a tuple with the RedirectUris field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRedirectUris

`func (o *ClientRegistrationResponse) SetRedirectUris(v []string)`

SetRedirectUris sets RedirectUris field to given value.


### GetGrantTypes

`func (o *ClientRegistrationResponse) GetGrantTypes() []string`

GetGrantTypes returns the GrantTypes field if non-nil, zero value otherwise.

### GetGrantTypesOk

`func (o *ClientRegistrationResponse) GetGrantTypesOk() (*[]string, bool)`

GetGrantTypesOk returns a tuple with the GrantTypes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGrantTypes

`func (o *ClientRegistrationResponse) SetGrantTypes(v []string)`

SetGrantTypes sets GrantTypes field to given value.

### HasGrantTypes

`func (o *ClientRegistrationResponse) HasGrantTypes() bool`

HasGrantTypes returns a boolean if a field has been set.

### GetResponseTypes

`func (o *ClientRegistrationResponse) GetResponseTypes() []string`

GetResponseTypes returns the ResponseTypes field if non-nil, zero value otherwise.

### GetResponseTypesOk

`func (o *ClientRegistrationResponse) GetResponseTypesOk() (*[]string, bool)`

GetResponseTypesOk returns a tuple with the ResponseTypes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseTypes

`func (o *ClientRegistrationResponse) SetResponseTypes(v []string)`

SetResponseTypes sets ResponseTypes field to given value.

### HasResponseTypes

`func (o *ClientRegistrationResponse) HasResponseTypes() bool`

HasResponseTypes returns a boolean if a field has been set.

### GetScope

`func (o *ClientRegistrationResponse) GetScope() string`

GetScope returns the Scope field if non-nil, zero value otherwise.

### GetScopeOk

`func (o *ClientRegistrationResponse) GetScopeOk() (*string, bool)`

GetScopeOk returns a tuple with the Scope field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScope

`func (o *ClientRegistrationResponse) SetScope(v string)`

SetScope sets Scope field to given value.

### HasScope

`func (o *ClientRegistrationResponse) HasScope() bool`

HasScope returns a boolean if a field has been set.

### GetTokenEndpointAuthMethod

`func (o *ClientRegistrationResponse) GetTokenEndpointAuthMethod() string`

GetTokenEndpointAuthMethod returns the TokenEndpointAuthMethod field if non-nil, zero value otherwise.

### GetTokenEndpointAuthMethodOk

`func (o *ClientRegistrationResponse) GetTokenEndpointAuthMethodOk() (*string, bool)`

GetTokenEndpointAuthMethodOk returns a tuple with the TokenEndpointAuthMethod field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTokenEndpointAuthMethod

`func (o *ClientRegistrationResponse) SetTokenEndpointAuthMethod(v string)`

SetTokenEndpointAuthMethod sets TokenEndpointAuthMethod field to given value.

### HasTokenEndpointAuthMethod

`func (o *ClientRegistrationResponse) HasTokenEndpointAuthMethod() bool`

HasTokenEndpointAuthMethod returns a boolean if a field has been set.

### GetRegistrationAccessToken

`func (o *ClientRegistrationResponse) GetRegistrationAccessToken() string`

GetRegistrationAccessToken returns the RegistrationAccessToken field if non-nil, zero value otherwise.

### GetRegistrationAccessTokenOk

`func (o *ClientRegistrationResponse) GetRegistrationAccessTokenOk() (*string, bool)`

GetRegistrationAccessTokenOk returns a tuple with the RegistrationAccessToken field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegistrationAccessToken

`func (o *ClientRegistrationResponse) SetRegistrationAccessToken(v string)`

SetRegistrationAccessToken sets RegistrationAccessToken field to given value.


### GetRegistrationClientUri

`func (o *ClientRegistrationResponse) GetRegistrationClientUri() string`

GetRegistrationClientUri returns the RegistrationClientUri field if non-nil, zero value otherwise.

### GetRegistrationClientUriOk

`func (o *ClientRegistrationResponse) GetRegistrationClientUriOk() (*string, bool)`

GetRegistrationClientUriOk returns a tuple with the RegistrationClientUri field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegistrationClientUri

`func (o *ClientRegistrationResponse) SetRegistrationClientUri(v string)`

SetRegistrationClientUri sets RegistrationClientUri field to given value.

### HasRegistrationClientUri

`func (o *ClientRegistrationResponse) HasRegistrationClientUri() bool`

HasRegistrationClientUri returns a boolean if a field has been set.

### GetClientIdIssuedAt

`func (o *ClientRegistrationResponse) GetClientIdIssuedAt() int32`

GetClientIdIssuedAt returns the ClientIdIssuedAt field if non-nil, zero value otherwise.

### GetClientIdIssuedAtOk

`func (o *ClientRegistrationResponse) GetClientIdIssuedAtOk() (*int32, bool)`

GetClientIdIssuedAtOk returns a tuple with the ClientIdIssuedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientIdIssuedAt

`func (o *ClientRegistrationResponse) SetClientIdIssuedAt(v int32)`

SetClientIdIssuedAt sets ClientIdIssuedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


