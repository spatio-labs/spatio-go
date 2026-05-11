# IntrospectionResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Active** | **bool** |  | 
**TokenType** | Pointer to **string** | &#x60;oauth&#x60; or &#x60;pat&#x60;. | [optional] 
**ClientId** | Pointer to **string** |  | [optional] 
**UserId** | Pointer to **string** |  | [optional] 
**WorkspaceId** | Pointer to **string** |  | [optional] 
**Scope** | Pointer to **string** |  | [optional] 
**Exp** | Pointer to **int32** |  | [optional] 

## Methods

### NewIntrospectionResponse

`func NewIntrospectionResponse(active bool, ) *IntrospectionResponse`

NewIntrospectionResponse instantiates a new IntrospectionResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewIntrospectionResponseWithDefaults

`func NewIntrospectionResponseWithDefaults() *IntrospectionResponse`

NewIntrospectionResponseWithDefaults instantiates a new IntrospectionResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetActive

`func (o *IntrospectionResponse) GetActive() bool`

GetActive returns the Active field if non-nil, zero value otherwise.

### GetActiveOk

`func (o *IntrospectionResponse) GetActiveOk() (*bool, bool)`

GetActiveOk returns a tuple with the Active field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActive

`func (o *IntrospectionResponse) SetActive(v bool)`

SetActive sets Active field to given value.


### GetTokenType

`func (o *IntrospectionResponse) GetTokenType() string`

GetTokenType returns the TokenType field if non-nil, zero value otherwise.

### GetTokenTypeOk

`func (o *IntrospectionResponse) GetTokenTypeOk() (*string, bool)`

GetTokenTypeOk returns a tuple with the TokenType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTokenType

`func (o *IntrospectionResponse) SetTokenType(v string)`

SetTokenType sets TokenType field to given value.

### HasTokenType

`func (o *IntrospectionResponse) HasTokenType() bool`

HasTokenType returns a boolean if a field has been set.

### GetClientId

`func (o *IntrospectionResponse) GetClientId() string`

GetClientId returns the ClientId field if non-nil, zero value otherwise.

### GetClientIdOk

`func (o *IntrospectionResponse) GetClientIdOk() (*string, bool)`

GetClientIdOk returns a tuple with the ClientId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientId

`func (o *IntrospectionResponse) SetClientId(v string)`

SetClientId sets ClientId field to given value.

### HasClientId

`func (o *IntrospectionResponse) HasClientId() bool`

HasClientId returns a boolean if a field has been set.

### GetUserId

`func (o *IntrospectionResponse) GetUserId() string`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *IntrospectionResponse) GetUserIdOk() (*string, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *IntrospectionResponse) SetUserId(v string)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *IntrospectionResponse) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetWorkspaceId

`func (o *IntrospectionResponse) GetWorkspaceId() string`

GetWorkspaceId returns the WorkspaceId field if non-nil, zero value otherwise.

### GetWorkspaceIdOk

`func (o *IntrospectionResponse) GetWorkspaceIdOk() (*string, bool)`

GetWorkspaceIdOk returns a tuple with the WorkspaceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWorkspaceId

`func (o *IntrospectionResponse) SetWorkspaceId(v string)`

SetWorkspaceId sets WorkspaceId field to given value.

### HasWorkspaceId

`func (o *IntrospectionResponse) HasWorkspaceId() bool`

HasWorkspaceId returns a boolean if a field has been set.

### GetScope

`func (o *IntrospectionResponse) GetScope() string`

GetScope returns the Scope field if non-nil, zero value otherwise.

### GetScopeOk

`func (o *IntrospectionResponse) GetScopeOk() (*string, bool)`

GetScopeOk returns a tuple with the Scope field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScope

`func (o *IntrospectionResponse) SetScope(v string)`

SetScope sets Scope field to given value.

### HasScope

`func (o *IntrospectionResponse) HasScope() bool`

HasScope returns a boolean if a field has been set.

### GetExp

`func (o *IntrospectionResponse) GetExp() int32`

GetExp returns the Exp field if non-nil, zero value otherwise.

### GetExpOk

`func (o *IntrospectionResponse) GetExpOk() (*int32, bool)`

GetExpOk returns a tuple with the Exp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExp

`func (o *IntrospectionResponse) SetExp(v int32)`

SetExp sets Exp field to given value.

### HasExp

`func (o *IntrospectionResponse) HasExp() bool`

HasExp returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


