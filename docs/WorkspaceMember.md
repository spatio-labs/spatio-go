# WorkspaceMember

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Role** | **string** |  | 
**Email** | Pointer to **string** |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**Avatar** | Pointer to **string** |  | [optional] 
**JoinedAt** | **time.Time** |  | 
**User** | Pointer to **map[string]interface{}** |  | [optional] 

## Methods

### NewWorkspaceMember

`func NewWorkspaceMember(id string, role string, joinedAt time.Time, ) *WorkspaceMember`

NewWorkspaceMember instantiates a new WorkspaceMember object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWorkspaceMemberWithDefaults

`func NewWorkspaceMemberWithDefaults() *WorkspaceMember`

NewWorkspaceMemberWithDefaults instantiates a new WorkspaceMember object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *WorkspaceMember) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *WorkspaceMember) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *WorkspaceMember) SetId(v string)`

SetId sets Id field to given value.


### GetRole

`func (o *WorkspaceMember) GetRole() string`

GetRole returns the Role field if non-nil, zero value otherwise.

### GetRoleOk

`func (o *WorkspaceMember) GetRoleOk() (*string, bool)`

GetRoleOk returns a tuple with the Role field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRole

`func (o *WorkspaceMember) SetRole(v string)`

SetRole sets Role field to given value.


### GetEmail

`func (o *WorkspaceMember) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *WorkspaceMember) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *WorkspaceMember) SetEmail(v string)`

SetEmail sets Email field to given value.

### HasEmail

`func (o *WorkspaceMember) HasEmail() bool`

HasEmail returns a boolean if a field has been set.

### GetName

`func (o *WorkspaceMember) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *WorkspaceMember) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *WorkspaceMember) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *WorkspaceMember) HasName() bool`

HasName returns a boolean if a field has been set.

### GetAvatar

`func (o *WorkspaceMember) GetAvatar() string`

GetAvatar returns the Avatar field if non-nil, zero value otherwise.

### GetAvatarOk

`func (o *WorkspaceMember) GetAvatarOk() (*string, bool)`

GetAvatarOk returns a tuple with the Avatar field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAvatar

`func (o *WorkspaceMember) SetAvatar(v string)`

SetAvatar sets Avatar field to given value.

### HasAvatar

`func (o *WorkspaceMember) HasAvatar() bool`

HasAvatar returns a boolean if a field has been set.

### GetJoinedAt

`func (o *WorkspaceMember) GetJoinedAt() time.Time`

GetJoinedAt returns the JoinedAt field if non-nil, zero value otherwise.

### GetJoinedAtOk

`func (o *WorkspaceMember) GetJoinedAtOk() (*time.Time, bool)`

GetJoinedAtOk returns a tuple with the JoinedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJoinedAt

`func (o *WorkspaceMember) SetJoinedAt(v time.Time)`

SetJoinedAt sets JoinedAt field to given value.


### GetUser

`func (o *WorkspaceMember) GetUser() map[string]interface{}`

GetUser returns the User field if non-nil, zero value otherwise.

### GetUserOk

`func (o *WorkspaceMember) GetUserOk() (*map[string]interface{}, bool)`

GetUserOk returns a tuple with the User field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUser

`func (o *WorkspaceMember) SetUser(v map[string]interface{})`

SetUser sets User field to given value.

### HasUser

`func (o *WorkspaceMember) HasUser() bool`

HasUser returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


