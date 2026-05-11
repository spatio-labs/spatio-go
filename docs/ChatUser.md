# ChatUser

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Provider** | Pointer to **string** |  | [optional] 
**AccountId** | Pointer to **string** |  | [optional] 
**Name** | **string** |  | 
**RealName** | Pointer to **string** |  | [optional] 
**Email** | Pointer to **string** |  | [optional] 
**Avatar** | Pointer to **string** |  | [optional] 
**IsBot** | **bool** |  | 
**IsActive** | **bool** |  | 

## Methods

### NewChatUser

`func NewChatUser(id string, name string, isBot bool, isActive bool, ) *ChatUser`

NewChatUser instantiates a new ChatUser object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewChatUserWithDefaults

`func NewChatUserWithDefaults() *ChatUser`

NewChatUserWithDefaults instantiates a new ChatUser object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ChatUser) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ChatUser) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ChatUser) SetId(v string)`

SetId sets Id field to given value.


### GetProvider

`func (o *ChatUser) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *ChatUser) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *ChatUser) SetProvider(v string)`

SetProvider sets Provider field to given value.

### HasProvider

`func (o *ChatUser) HasProvider() bool`

HasProvider returns a boolean if a field has been set.

### GetAccountId

`func (o *ChatUser) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *ChatUser) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *ChatUser) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *ChatUser) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.

### GetName

`func (o *ChatUser) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ChatUser) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ChatUser) SetName(v string)`

SetName sets Name field to given value.


### GetRealName

`func (o *ChatUser) GetRealName() string`

GetRealName returns the RealName field if non-nil, zero value otherwise.

### GetRealNameOk

`func (o *ChatUser) GetRealNameOk() (*string, bool)`

GetRealNameOk returns a tuple with the RealName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRealName

`func (o *ChatUser) SetRealName(v string)`

SetRealName sets RealName field to given value.

### HasRealName

`func (o *ChatUser) HasRealName() bool`

HasRealName returns a boolean if a field has been set.

### GetEmail

`func (o *ChatUser) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *ChatUser) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *ChatUser) SetEmail(v string)`

SetEmail sets Email field to given value.

### HasEmail

`func (o *ChatUser) HasEmail() bool`

HasEmail returns a boolean if a field has been set.

### GetAvatar

`func (o *ChatUser) GetAvatar() string`

GetAvatar returns the Avatar field if non-nil, zero value otherwise.

### GetAvatarOk

`func (o *ChatUser) GetAvatarOk() (*string, bool)`

GetAvatarOk returns a tuple with the Avatar field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAvatar

`func (o *ChatUser) SetAvatar(v string)`

SetAvatar sets Avatar field to given value.

### HasAvatar

`func (o *ChatUser) HasAvatar() bool`

HasAvatar returns a boolean if a field has been set.

### GetIsBot

`func (o *ChatUser) GetIsBot() bool`

GetIsBot returns the IsBot field if non-nil, zero value otherwise.

### GetIsBotOk

`func (o *ChatUser) GetIsBotOk() (*bool, bool)`

GetIsBotOk returns a tuple with the IsBot field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsBot

`func (o *ChatUser) SetIsBot(v bool)`

SetIsBot sets IsBot field to given value.


### GetIsActive

`func (o *ChatUser) GetIsActive() bool`

GetIsActive returns the IsActive field if non-nil, zero value otherwise.

### GetIsActiveOk

`func (o *ChatUser) GetIsActiveOk() (*bool, bool)`

GetIsActiveOk returns a tuple with the IsActive field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsActive

`func (o *ChatUser) SetIsActive(v bool)`

SetIsActive sets IsActive field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


