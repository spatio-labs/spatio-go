# DiscoveryDocument

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Issuer** | **string** |  | 
**AuthorizationEndpoint** | **string** |  | 
**TokenEndpoint** | **string** |  | 
**RegistrationEndpoint** | Pointer to **string** |  | [optional] 
**IntrospectionEndpoint** | Pointer to **string** |  | [optional] 
**RevocationEndpoint** | Pointer to **string** |  | [optional] 
**UserinfoEndpoint** | Pointer to **string** |  | [optional] 
**JwksUri** | **string** |  | 
**ResponseTypesSupported** | Pointer to **[]string** |  | [optional] 
**GrantTypesSupported** | Pointer to **[]string** |  | [optional] 
**TokenEndpointAuthMethodsSupported** | Pointer to **[]string** |  | [optional] 
**CodeChallengeMethodsSupported** | Pointer to **[]string** |  | [optional] 
**ScopesSupported** | **[]string** |  | 
**SubjectTypesSupported** | Pointer to **[]string** |  | [optional] 
**IdTokenSigningAlgValuesSupported** | Pointer to **[]string** |  | [optional] 
**PromptValuesSupported** | Pointer to **[]string** |  | [optional] 
**ClaimsSupported** | Pointer to **[]string** |  | [optional] 
**ServiceDocumentation** | Pointer to **string** |  | [optional] 

## Methods

### NewDiscoveryDocument

`func NewDiscoveryDocument(issuer string, authorizationEndpoint string, tokenEndpoint string, jwksUri string, scopesSupported []string, ) *DiscoveryDocument`

NewDiscoveryDocument instantiates a new DiscoveryDocument object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDiscoveryDocumentWithDefaults

`func NewDiscoveryDocumentWithDefaults() *DiscoveryDocument`

NewDiscoveryDocumentWithDefaults instantiates a new DiscoveryDocument object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetIssuer

`func (o *DiscoveryDocument) GetIssuer() string`

GetIssuer returns the Issuer field if non-nil, zero value otherwise.

### GetIssuerOk

`func (o *DiscoveryDocument) GetIssuerOk() (*string, bool)`

GetIssuerOk returns a tuple with the Issuer field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIssuer

`func (o *DiscoveryDocument) SetIssuer(v string)`

SetIssuer sets Issuer field to given value.


### GetAuthorizationEndpoint

`func (o *DiscoveryDocument) GetAuthorizationEndpoint() string`

GetAuthorizationEndpoint returns the AuthorizationEndpoint field if non-nil, zero value otherwise.

### GetAuthorizationEndpointOk

`func (o *DiscoveryDocument) GetAuthorizationEndpointOk() (*string, bool)`

GetAuthorizationEndpointOk returns a tuple with the AuthorizationEndpoint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAuthorizationEndpoint

`func (o *DiscoveryDocument) SetAuthorizationEndpoint(v string)`

SetAuthorizationEndpoint sets AuthorizationEndpoint field to given value.


### GetTokenEndpoint

`func (o *DiscoveryDocument) GetTokenEndpoint() string`

GetTokenEndpoint returns the TokenEndpoint field if non-nil, zero value otherwise.

### GetTokenEndpointOk

`func (o *DiscoveryDocument) GetTokenEndpointOk() (*string, bool)`

GetTokenEndpointOk returns a tuple with the TokenEndpoint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTokenEndpoint

`func (o *DiscoveryDocument) SetTokenEndpoint(v string)`

SetTokenEndpoint sets TokenEndpoint field to given value.


### GetRegistrationEndpoint

`func (o *DiscoveryDocument) GetRegistrationEndpoint() string`

GetRegistrationEndpoint returns the RegistrationEndpoint field if non-nil, zero value otherwise.

### GetRegistrationEndpointOk

`func (o *DiscoveryDocument) GetRegistrationEndpointOk() (*string, bool)`

GetRegistrationEndpointOk returns a tuple with the RegistrationEndpoint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegistrationEndpoint

`func (o *DiscoveryDocument) SetRegistrationEndpoint(v string)`

SetRegistrationEndpoint sets RegistrationEndpoint field to given value.

### HasRegistrationEndpoint

`func (o *DiscoveryDocument) HasRegistrationEndpoint() bool`

HasRegistrationEndpoint returns a boolean if a field has been set.

### GetIntrospectionEndpoint

`func (o *DiscoveryDocument) GetIntrospectionEndpoint() string`

GetIntrospectionEndpoint returns the IntrospectionEndpoint field if non-nil, zero value otherwise.

### GetIntrospectionEndpointOk

`func (o *DiscoveryDocument) GetIntrospectionEndpointOk() (*string, bool)`

GetIntrospectionEndpointOk returns a tuple with the IntrospectionEndpoint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIntrospectionEndpoint

`func (o *DiscoveryDocument) SetIntrospectionEndpoint(v string)`

SetIntrospectionEndpoint sets IntrospectionEndpoint field to given value.

### HasIntrospectionEndpoint

`func (o *DiscoveryDocument) HasIntrospectionEndpoint() bool`

HasIntrospectionEndpoint returns a boolean if a field has been set.

### GetRevocationEndpoint

`func (o *DiscoveryDocument) GetRevocationEndpoint() string`

GetRevocationEndpoint returns the RevocationEndpoint field if non-nil, zero value otherwise.

### GetRevocationEndpointOk

`func (o *DiscoveryDocument) GetRevocationEndpointOk() (*string, bool)`

GetRevocationEndpointOk returns a tuple with the RevocationEndpoint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRevocationEndpoint

`func (o *DiscoveryDocument) SetRevocationEndpoint(v string)`

SetRevocationEndpoint sets RevocationEndpoint field to given value.

### HasRevocationEndpoint

`func (o *DiscoveryDocument) HasRevocationEndpoint() bool`

HasRevocationEndpoint returns a boolean if a field has been set.

### GetUserinfoEndpoint

`func (o *DiscoveryDocument) GetUserinfoEndpoint() string`

GetUserinfoEndpoint returns the UserinfoEndpoint field if non-nil, zero value otherwise.

### GetUserinfoEndpointOk

`func (o *DiscoveryDocument) GetUserinfoEndpointOk() (*string, bool)`

GetUserinfoEndpointOk returns a tuple with the UserinfoEndpoint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserinfoEndpoint

`func (o *DiscoveryDocument) SetUserinfoEndpoint(v string)`

SetUserinfoEndpoint sets UserinfoEndpoint field to given value.

### HasUserinfoEndpoint

`func (o *DiscoveryDocument) HasUserinfoEndpoint() bool`

HasUserinfoEndpoint returns a boolean if a field has been set.

### GetJwksUri

`func (o *DiscoveryDocument) GetJwksUri() string`

GetJwksUri returns the JwksUri field if non-nil, zero value otherwise.

### GetJwksUriOk

`func (o *DiscoveryDocument) GetJwksUriOk() (*string, bool)`

GetJwksUriOk returns a tuple with the JwksUri field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJwksUri

`func (o *DiscoveryDocument) SetJwksUri(v string)`

SetJwksUri sets JwksUri field to given value.


### GetResponseTypesSupported

`func (o *DiscoveryDocument) GetResponseTypesSupported() []string`

GetResponseTypesSupported returns the ResponseTypesSupported field if non-nil, zero value otherwise.

### GetResponseTypesSupportedOk

`func (o *DiscoveryDocument) GetResponseTypesSupportedOk() (*[]string, bool)`

GetResponseTypesSupportedOk returns a tuple with the ResponseTypesSupported field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseTypesSupported

`func (o *DiscoveryDocument) SetResponseTypesSupported(v []string)`

SetResponseTypesSupported sets ResponseTypesSupported field to given value.

### HasResponseTypesSupported

`func (o *DiscoveryDocument) HasResponseTypesSupported() bool`

HasResponseTypesSupported returns a boolean if a field has been set.

### GetGrantTypesSupported

`func (o *DiscoveryDocument) GetGrantTypesSupported() []string`

GetGrantTypesSupported returns the GrantTypesSupported field if non-nil, zero value otherwise.

### GetGrantTypesSupportedOk

`func (o *DiscoveryDocument) GetGrantTypesSupportedOk() (*[]string, bool)`

GetGrantTypesSupportedOk returns a tuple with the GrantTypesSupported field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGrantTypesSupported

`func (o *DiscoveryDocument) SetGrantTypesSupported(v []string)`

SetGrantTypesSupported sets GrantTypesSupported field to given value.

### HasGrantTypesSupported

`func (o *DiscoveryDocument) HasGrantTypesSupported() bool`

HasGrantTypesSupported returns a boolean if a field has been set.

### GetTokenEndpointAuthMethodsSupported

`func (o *DiscoveryDocument) GetTokenEndpointAuthMethodsSupported() []string`

GetTokenEndpointAuthMethodsSupported returns the TokenEndpointAuthMethodsSupported field if non-nil, zero value otherwise.

### GetTokenEndpointAuthMethodsSupportedOk

`func (o *DiscoveryDocument) GetTokenEndpointAuthMethodsSupportedOk() (*[]string, bool)`

GetTokenEndpointAuthMethodsSupportedOk returns a tuple with the TokenEndpointAuthMethodsSupported field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTokenEndpointAuthMethodsSupported

`func (o *DiscoveryDocument) SetTokenEndpointAuthMethodsSupported(v []string)`

SetTokenEndpointAuthMethodsSupported sets TokenEndpointAuthMethodsSupported field to given value.

### HasTokenEndpointAuthMethodsSupported

`func (o *DiscoveryDocument) HasTokenEndpointAuthMethodsSupported() bool`

HasTokenEndpointAuthMethodsSupported returns a boolean if a field has been set.

### GetCodeChallengeMethodsSupported

`func (o *DiscoveryDocument) GetCodeChallengeMethodsSupported() []string`

GetCodeChallengeMethodsSupported returns the CodeChallengeMethodsSupported field if non-nil, zero value otherwise.

### GetCodeChallengeMethodsSupportedOk

`func (o *DiscoveryDocument) GetCodeChallengeMethodsSupportedOk() (*[]string, bool)`

GetCodeChallengeMethodsSupportedOk returns a tuple with the CodeChallengeMethodsSupported field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCodeChallengeMethodsSupported

`func (o *DiscoveryDocument) SetCodeChallengeMethodsSupported(v []string)`

SetCodeChallengeMethodsSupported sets CodeChallengeMethodsSupported field to given value.

### HasCodeChallengeMethodsSupported

`func (o *DiscoveryDocument) HasCodeChallengeMethodsSupported() bool`

HasCodeChallengeMethodsSupported returns a boolean if a field has been set.

### GetScopesSupported

`func (o *DiscoveryDocument) GetScopesSupported() []string`

GetScopesSupported returns the ScopesSupported field if non-nil, zero value otherwise.

### GetScopesSupportedOk

`func (o *DiscoveryDocument) GetScopesSupportedOk() (*[]string, bool)`

GetScopesSupportedOk returns a tuple with the ScopesSupported field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScopesSupported

`func (o *DiscoveryDocument) SetScopesSupported(v []string)`

SetScopesSupported sets ScopesSupported field to given value.


### GetSubjectTypesSupported

`func (o *DiscoveryDocument) GetSubjectTypesSupported() []string`

GetSubjectTypesSupported returns the SubjectTypesSupported field if non-nil, zero value otherwise.

### GetSubjectTypesSupportedOk

`func (o *DiscoveryDocument) GetSubjectTypesSupportedOk() (*[]string, bool)`

GetSubjectTypesSupportedOk returns a tuple with the SubjectTypesSupported field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubjectTypesSupported

`func (o *DiscoveryDocument) SetSubjectTypesSupported(v []string)`

SetSubjectTypesSupported sets SubjectTypesSupported field to given value.

### HasSubjectTypesSupported

`func (o *DiscoveryDocument) HasSubjectTypesSupported() bool`

HasSubjectTypesSupported returns a boolean if a field has been set.

### GetIdTokenSigningAlgValuesSupported

`func (o *DiscoveryDocument) GetIdTokenSigningAlgValuesSupported() []string`

GetIdTokenSigningAlgValuesSupported returns the IdTokenSigningAlgValuesSupported field if non-nil, zero value otherwise.

### GetIdTokenSigningAlgValuesSupportedOk

`func (o *DiscoveryDocument) GetIdTokenSigningAlgValuesSupportedOk() (*[]string, bool)`

GetIdTokenSigningAlgValuesSupportedOk returns a tuple with the IdTokenSigningAlgValuesSupported field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIdTokenSigningAlgValuesSupported

`func (o *DiscoveryDocument) SetIdTokenSigningAlgValuesSupported(v []string)`

SetIdTokenSigningAlgValuesSupported sets IdTokenSigningAlgValuesSupported field to given value.

### HasIdTokenSigningAlgValuesSupported

`func (o *DiscoveryDocument) HasIdTokenSigningAlgValuesSupported() bool`

HasIdTokenSigningAlgValuesSupported returns a boolean if a field has been set.

### GetPromptValuesSupported

`func (o *DiscoveryDocument) GetPromptValuesSupported() []string`

GetPromptValuesSupported returns the PromptValuesSupported field if non-nil, zero value otherwise.

### GetPromptValuesSupportedOk

`func (o *DiscoveryDocument) GetPromptValuesSupportedOk() (*[]string, bool)`

GetPromptValuesSupportedOk returns a tuple with the PromptValuesSupported field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPromptValuesSupported

`func (o *DiscoveryDocument) SetPromptValuesSupported(v []string)`

SetPromptValuesSupported sets PromptValuesSupported field to given value.

### HasPromptValuesSupported

`func (o *DiscoveryDocument) HasPromptValuesSupported() bool`

HasPromptValuesSupported returns a boolean if a field has been set.

### GetClaimsSupported

`func (o *DiscoveryDocument) GetClaimsSupported() []string`

GetClaimsSupported returns the ClaimsSupported field if non-nil, zero value otherwise.

### GetClaimsSupportedOk

`func (o *DiscoveryDocument) GetClaimsSupportedOk() (*[]string, bool)`

GetClaimsSupportedOk returns a tuple with the ClaimsSupported field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClaimsSupported

`func (o *DiscoveryDocument) SetClaimsSupported(v []string)`

SetClaimsSupported sets ClaimsSupported field to given value.

### HasClaimsSupported

`func (o *DiscoveryDocument) HasClaimsSupported() bool`

HasClaimsSupported returns a boolean if a field has been set.

### GetServiceDocumentation

`func (o *DiscoveryDocument) GetServiceDocumentation() string`

GetServiceDocumentation returns the ServiceDocumentation field if non-nil, zero value otherwise.

### GetServiceDocumentationOk

`func (o *DiscoveryDocument) GetServiceDocumentationOk() (*string, bool)`

GetServiceDocumentationOk returns a tuple with the ServiceDocumentation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetServiceDocumentation

`func (o *DiscoveryDocument) SetServiceDocumentation(v string)`

SetServiceDocumentation sets ServiceDocumentation field to given value.

### HasServiceDocumentation

`func (o *DiscoveryDocument) HasServiceDocumentation() bool`

HasServiceDocumentation returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


