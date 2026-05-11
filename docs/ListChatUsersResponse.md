# ListChatUsersResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Users** | Pointer to [**[]ChatUser**](ChatUser.md) |  | [optional] 
**Total** | **int32** |  | 
**NextCursor** | Pointer to **string** |  | [optional] 
**Provider** | **string** |  | 

## Methods

### NewListChatUsersResponse

`func NewListChatUsersResponse(total int32, provider string, ) *ListChatUsersResponse`

NewListChatUsersResponse instantiates a new ListChatUsersResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewListChatUsersResponseWithDefaults

`func NewListChatUsersResponseWithDefaults() *ListChatUsersResponse`

NewListChatUsersResponseWithDefaults instantiates a new ListChatUsersResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUsers

`func (o *ListChatUsersResponse) GetUsers() []ChatUser`

GetUsers returns the Users field if non-nil, zero value otherwise.

### GetUsersOk

`func (o *ListChatUsersResponse) GetUsersOk() (*[]ChatUser, bool)`

GetUsersOk returns a tuple with the Users field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUsers

`func (o *ListChatUsersResponse) SetUsers(v []ChatUser)`

SetUsers sets Users field to given value.

### HasUsers

`func (o *ListChatUsersResponse) HasUsers() bool`

HasUsers returns a boolean if a field has been set.

### SetUsersNil

`func (o *ListChatUsersResponse) SetUsersNil(b bool)`

 SetUsersNil sets the value for Users to be an explicit nil

### UnsetUsers
`func (o *ListChatUsersResponse) UnsetUsers()`

UnsetUsers ensures that no value is present for Users, not even an explicit nil
### GetTotal

`func (o *ListChatUsersResponse) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *ListChatUsersResponse) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *ListChatUsersResponse) SetTotal(v int32)`

SetTotal sets Total field to given value.


### GetNextCursor

`func (o *ListChatUsersResponse) GetNextCursor() string`

GetNextCursor returns the NextCursor field if non-nil, zero value otherwise.

### GetNextCursorOk

`func (o *ListChatUsersResponse) GetNextCursorOk() (*string, bool)`

GetNextCursorOk returns a tuple with the NextCursor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextCursor

`func (o *ListChatUsersResponse) SetNextCursor(v string)`

SetNextCursor sets NextCursor field to given value.

### HasNextCursor

`func (o *ListChatUsersResponse) HasNextCursor() bool`

HasNextCursor returns a boolean if a field has been set.

### GetProvider

`func (o *ListChatUsersResponse) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *ListChatUsersResponse) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *ListChatUsersResponse) SetProvider(v string)`

SetProvider sets Provider field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


