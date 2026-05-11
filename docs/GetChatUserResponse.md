# GetChatUserResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**User** | [**ChatUser**](ChatUser.md) |  | 
**Provider** | **string** |  | 

## Methods

### NewGetChatUserResponse

`func NewGetChatUserResponse(user ChatUser, provider string, ) *GetChatUserResponse`

NewGetChatUserResponse instantiates a new GetChatUserResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGetChatUserResponseWithDefaults

`func NewGetChatUserResponseWithDefaults() *GetChatUserResponse`

NewGetChatUserResponseWithDefaults instantiates a new GetChatUserResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUser

`func (o *GetChatUserResponse) GetUser() ChatUser`

GetUser returns the User field if non-nil, zero value otherwise.

### GetUserOk

`func (o *GetChatUserResponse) GetUserOk() (*ChatUser, bool)`

GetUserOk returns a tuple with the User field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUser

`func (o *GetChatUserResponse) SetUser(v ChatUser)`

SetUser sets User field to given value.


### GetProvider

`func (o *GetChatUserResponse) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *GetChatUserResponse) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *GetChatUserResponse) SetProvider(v string)`

SetProvider sets Provider field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


