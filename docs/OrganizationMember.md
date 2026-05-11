# OrganizationMember

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | &#x60;OrganizationMember&#x60; row id. | 
**UserId** | **string** |  | 
**Role** | **string** |  | 
**JoinedAt** | **time.Time** |  | 
**InvitedBy** | Pointer to [**OrganizationMemberInvitedBy**](OrganizationMemberInvitedBy.md) |  | [optional] 
**User** | Pointer to **map[string]interface{}** | Embedded user-profile fields (id, email, name, profilePhoto, ...). | [optional] 

## Methods

### NewOrganizationMember

`func NewOrganizationMember(id string, userId string, role string, joinedAt time.Time, ) *OrganizationMember`

NewOrganizationMember instantiates a new OrganizationMember object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewOrganizationMemberWithDefaults

`func NewOrganizationMemberWithDefaults() *OrganizationMember`

NewOrganizationMemberWithDefaults instantiates a new OrganizationMember object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *OrganizationMember) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *OrganizationMember) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *OrganizationMember) SetId(v string)`

SetId sets Id field to given value.


### GetUserId

`func (o *OrganizationMember) GetUserId() string`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *OrganizationMember) GetUserIdOk() (*string, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *OrganizationMember) SetUserId(v string)`

SetUserId sets UserId field to given value.


### GetRole

`func (o *OrganizationMember) GetRole() string`

GetRole returns the Role field if non-nil, zero value otherwise.

### GetRoleOk

`func (o *OrganizationMember) GetRoleOk() (*string, bool)`

GetRoleOk returns a tuple with the Role field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRole

`func (o *OrganizationMember) SetRole(v string)`

SetRole sets Role field to given value.


### GetJoinedAt

`func (o *OrganizationMember) GetJoinedAt() time.Time`

GetJoinedAt returns the JoinedAt field if non-nil, zero value otherwise.

### GetJoinedAtOk

`func (o *OrganizationMember) GetJoinedAtOk() (*time.Time, bool)`

GetJoinedAtOk returns a tuple with the JoinedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJoinedAt

`func (o *OrganizationMember) SetJoinedAt(v time.Time)`

SetJoinedAt sets JoinedAt field to given value.


### GetInvitedBy

`func (o *OrganizationMember) GetInvitedBy() OrganizationMemberInvitedBy`

GetInvitedBy returns the InvitedBy field if non-nil, zero value otherwise.

### GetInvitedByOk

`func (o *OrganizationMember) GetInvitedByOk() (*OrganizationMemberInvitedBy, bool)`

GetInvitedByOk returns a tuple with the InvitedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInvitedBy

`func (o *OrganizationMember) SetInvitedBy(v OrganizationMemberInvitedBy)`

SetInvitedBy sets InvitedBy field to given value.

### HasInvitedBy

`func (o *OrganizationMember) HasInvitedBy() bool`

HasInvitedBy returns a boolean if a field has been set.

### GetUser

`func (o *OrganizationMember) GetUser() map[string]interface{}`

GetUser returns the User field if non-nil, zero value otherwise.

### GetUserOk

`func (o *OrganizationMember) GetUserOk() (*map[string]interface{}, bool)`

GetUserOk returns a tuple with the User field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUser

`func (o *OrganizationMember) SetUser(v map[string]interface{})`

SetUser sets User field to given value.

### HasUser

`func (o *OrganizationMember) HasUser() bool`

HasUser returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


