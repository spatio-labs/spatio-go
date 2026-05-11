# PersonalAccessToken

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Name** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **string** |  | [optional] 
**Scopes** | Pointer to **[]string** |  | [optional] 
**WorkspaceId** | Pointer to **NullableString** |  | [optional] 
**CreatedAt** | Pointer to **time.Time** |  | [optional] 
**LastUsedAt** | Pointer to **NullableTime** |  | [optional] 
**ExpiresAt** | Pointer to **NullableTime** |  | [optional] 
**TokenPrefix** | Pointer to **string** |  | [optional] 

## Methods

### NewPersonalAccessToken

`func NewPersonalAccessToken(id string, ) *PersonalAccessToken`

NewPersonalAccessToken instantiates a new PersonalAccessToken object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPersonalAccessTokenWithDefaults

`func NewPersonalAccessTokenWithDefaults() *PersonalAccessToken`

NewPersonalAccessTokenWithDefaults instantiates a new PersonalAccessToken object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *PersonalAccessToken) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *PersonalAccessToken) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *PersonalAccessToken) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *PersonalAccessToken) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *PersonalAccessToken) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *PersonalAccessToken) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *PersonalAccessToken) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDescription

`func (o *PersonalAccessToken) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *PersonalAccessToken) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *PersonalAccessToken) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *PersonalAccessToken) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetScopes

`func (o *PersonalAccessToken) GetScopes() []string`

GetScopes returns the Scopes field if non-nil, zero value otherwise.

### GetScopesOk

`func (o *PersonalAccessToken) GetScopesOk() (*[]string, bool)`

GetScopesOk returns a tuple with the Scopes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScopes

`func (o *PersonalAccessToken) SetScopes(v []string)`

SetScopes sets Scopes field to given value.

### HasScopes

`func (o *PersonalAccessToken) HasScopes() bool`

HasScopes returns a boolean if a field has been set.

### GetWorkspaceId

`func (o *PersonalAccessToken) GetWorkspaceId() string`

GetWorkspaceId returns the WorkspaceId field if non-nil, zero value otherwise.

### GetWorkspaceIdOk

`func (o *PersonalAccessToken) GetWorkspaceIdOk() (*string, bool)`

GetWorkspaceIdOk returns a tuple with the WorkspaceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWorkspaceId

`func (o *PersonalAccessToken) SetWorkspaceId(v string)`

SetWorkspaceId sets WorkspaceId field to given value.

### HasWorkspaceId

`func (o *PersonalAccessToken) HasWorkspaceId() bool`

HasWorkspaceId returns a boolean if a field has been set.

### SetWorkspaceIdNil

`func (o *PersonalAccessToken) SetWorkspaceIdNil(b bool)`

 SetWorkspaceIdNil sets the value for WorkspaceId to be an explicit nil

### UnsetWorkspaceId
`func (o *PersonalAccessToken) UnsetWorkspaceId()`

UnsetWorkspaceId ensures that no value is present for WorkspaceId, not even an explicit nil
### GetCreatedAt

`func (o *PersonalAccessToken) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *PersonalAccessToken) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *PersonalAccessToken) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *PersonalAccessToken) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetLastUsedAt

`func (o *PersonalAccessToken) GetLastUsedAt() time.Time`

GetLastUsedAt returns the LastUsedAt field if non-nil, zero value otherwise.

### GetLastUsedAtOk

`func (o *PersonalAccessToken) GetLastUsedAtOk() (*time.Time, bool)`

GetLastUsedAtOk returns a tuple with the LastUsedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastUsedAt

`func (o *PersonalAccessToken) SetLastUsedAt(v time.Time)`

SetLastUsedAt sets LastUsedAt field to given value.

### HasLastUsedAt

`func (o *PersonalAccessToken) HasLastUsedAt() bool`

HasLastUsedAt returns a boolean if a field has been set.

### SetLastUsedAtNil

`func (o *PersonalAccessToken) SetLastUsedAtNil(b bool)`

 SetLastUsedAtNil sets the value for LastUsedAt to be an explicit nil

### UnsetLastUsedAt
`func (o *PersonalAccessToken) UnsetLastUsedAt()`

UnsetLastUsedAt ensures that no value is present for LastUsedAt, not even an explicit nil
### GetExpiresAt

`func (o *PersonalAccessToken) GetExpiresAt() time.Time`

GetExpiresAt returns the ExpiresAt field if non-nil, zero value otherwise.

### GetExpiresAtOk

`func (o *PersonalAccessToken) GetExpiresAtOk() (*time.Time, bool)`

GetExpiresAtOk returns a tuple with the ExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresAt

`func (o *PersonalAccessToken) SetExpiresAt(v time.Time)`

SetExpiresAt sets ExpiresAt field to given value.

### HasExpiresAt

`func (o *PersonalAccessToken) HasExpiresAt() bool`

HasExpiresAt returns a boolean if a field has been set.

### SetExpiresAtNil

`func (o *PersonalAccessToken) SetExpiresAtNil(b bool)`

 SetExpiresAtNil sets the value for ExpiresAt to be an explicit nil

### UnsetExpiresAt
`func (o *PersonalAccessToken) UnsetExpiresAt()`

UnsetExpiresAt ensures that no value is present for ExpiresAt, not even an explicit nil
### GetTokenPrefix

`func (o *PersonalAccessToken) GetTokenPrefix() string`

GetTokenPrefix returns the TokenPrefix field if non-nil, zero value otherwise.

### GetTokenPrefixOk

`func (o *PersonalAccessToken) GetTokenPrefixOk() (*string, bool)`

GetTokenPrefixOk returns a tuple with the TokenPrefix field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTokenPrefix

`func (o *PersonalAccessToken) SetTokenPrefix(v string)`

SetTokenPrefix sets TokenPrefix field to given value.

### HasTokenPrefix

`func (o *PersonalAccessToken) HasTokenPrefix() bool`

HasTokenPrefix returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


