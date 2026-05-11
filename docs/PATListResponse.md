# PATListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Tokens** | [**[]PersonalAccessToken**](PersonalAccessToken.md) |  | 
**AvailableScopes** | Pointer to **[]string** |  | [optional] 

## Methods

### NewPATListResponse

`func NewPATListResponse(tokens []PersonalAccessToken, ) *PATListResponse`

NewPATListResponse instantiates a new PATListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPATListResponseWithDefaults

`func NewPATListResponseWithDefaults() *PATListResponse`

NewPATListResponseWithDefaults instantiates a new PATListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTokens

`func (o *PATListResponse) GetTokens() []PersonalAccessToken`

GetTokens returns the Tokens field if non-nil, zero value otherwise.

### GetTokensOk

`func (o *PATListResponse) GetTokensOk() (*[]PersonalAccessToken, bool)`

GetTokensOk returns a tuple with the Tokens field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTokens

`func (o *PATListResponse) SetTokens(v []PersonalAccessToken)`

SetTokens sets Tokens field to given value.


### GetAvailableScopes

`func (o *PATListResponse) GetAvailableScopes() []string`

GetAvailableScopes returns the AvailableScopes field if non-nil, zero value otherwise.

### GetAvailableScopesOk

`func (o *PATListResponse) GetAvailableScopesOk() (*[]string, bool)`

GetAvailableScopesOk returns a tuple with the AvailableScopes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAvailableScopes

`func (o *PATListResponse) SetAvailableScopes(v []string)`

SetAvailableScopes sets AvailableScopes field to given value.

### HasAvailableScopes

`func (o *PATListResponse) HasAvailableScopes() bool`

HasAvailableScopes returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


