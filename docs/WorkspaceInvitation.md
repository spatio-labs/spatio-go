# WorkspaceInvitation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**WorkspaceId** | Pointer to **string** |  | [optional] 
**Email** | **string** |  | 
**Role** | **string** |  | 
**ExpiresAt** | Pointer to **NullableTime** |  | [optional] 
**CreatedAt** | **time.Time** |  | 
**AcceptedAt** | Pointer to **NullableTime** |  | [optional] 
**RevokedAt** | Pointer to **NullableTime** |  | [optional] 
**Status** | Pointer to **string** |  | [optional] 

## Methods

### NewWorkspaceInvitation

`func NewWorkspaceInvitation(id string, email string, role string, createdAt time.Time, ) *WorkspaceInvitation`

NewWorkspaceInvitation instantiates a new WorkspaceInvitation object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWorkspaceInvitationWithDefaults

`func NewWorkspaceInvitationWithDefaults() *WorkspaceInvitation`

NewWorkspaceInvitationWithDefaults instantiates a new WorkspaceInvitation object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *WorkspaceInvitation) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *WorkspaceInvitation) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *WorkspaceInvitation) SetId(v string)`

SetId sets Id field to given value.


### GetWorkspaceId

`func (o *WorkspaceInvitation) GetWorkspaceId() string`

GetWorkspaceId returns the WorkspaceId field if non-nil, zero value otherwise.

### GetWorkspaceIdOk

`func (o *WorkspaceInvitation) GetWorkspaceIdOk() (*string, bool)`

GetWorkspaceIdOk returns a tuple with the WorkspaceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWorkspaceId

`func (o *WorkspaceInvitation) SetWorkspaceId(v string)`

SetWorkspaceId sets WorkspaceId field to given value.

### HasWorkspaceId

`func (o *WorkspaceInvitation) HasWorkspaceId() bool`

HasWorkspaceId returns a boolean if a field has been set.

### GetEmail

`func (o *WorkspaceInvitation) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *WorkspaceInvitation) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *WorkspaceInvitation) SetEmail(v string)`

SetEmail sets Email field to given value.


### GetRole

`func (o *WorkspaceInvitation) GetRole() string`

GetRole returns the Role field if non-nil, zero value otherwise.

### GetRoleOk

`func (o *WorkspaceInvitation) GetRoleOk() (*string, bool)`

GetRoleOk returns a tuple with the Role field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRole

`func (o *WorkspaceInvitation) SetRole(v string)`

SetRole sets Role field to given value.


### GetExpiresAt

`func (o *WorkspaceInvitation) GetExpiresAt() time.Time`

GetExpiresAt returns the ExpiresAt field if non-nil, zero value otherwise.

### GetExpiresAtOk

`func (o *WorkspaceInvitation) GetExpiresAtOk() (*time.Time, bool)`

GetExpiresAtOk returns a tuple with the ExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresAt

`func (o *WorkspaceInvitation) SetExpiresAt(v time.Time)`

SetExpiresAt sets ExpiresAt field to given value.

### HasExpiresAt

`func (o *WorkspaceInvitation) HasExpiresAt() bool`

HasExpiresAt returns a boolean if a field has been set.

### SetExpiresAtNil

`func (o *WorkspaceInvitation) SetExpiresAtNil(b bool)`

 SetExpiresAtNil sets the value for ExpiresAt to be an explicit nil

### UnsetExpiresAt
`func (o *WorkspaceInvitation) UnsetExpiresAt()`

UnsetExpiresAt ensures that no value is present for ExpiresAt, not even an explicit nil
### GetCreatedAt

`func (o *WorkspaceInvitation) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *WorkspaceInvitation) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *WorkspaceInvitation) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetAcceptedAt

`func (o *WorkspaceInvitation) GetAcceptedAt() time.Time`

GetAcceptedAt returns the AcceptedAt field if non-nil, zero value otherwise.

### GetAcceptedAtOk

`func (o *WorkspaceInvitation) GetAcceptedAtOk() (*time.Time, bool)`

GetAcceptedAtOk returns a tuple with the AcceptedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAcceptedAt

`func (o *WorkspaceInvitation) SetAcceptedAt(v time.Time)`

SetAcceptedAt sets AcceptedAt field to given value.

### HasAcceptedAt

`func (o *WorkspaceInvitation) HasAcceptedAt() bool`

HasAcceptedAt returns a boolean if a field has been set.

### SetAcceptedAtNil

`func (o *WorkspaceInvitation) SetAcceptedAtNil(b bool)`

 SetAcceptedAtNil sets the value for AcceptedAt to be an explicit nil

### UnsetAcceptedAt
`func (o *WorkspaceInvitation) UnsetAcceptedAt()`

UnsetAcceptedAt ensures that no value is present for AcceptedAt, not even an explicit nil
### GetRevokedAt

`func (o *WorkspaceInvitation) GetRevokedAt() time.Time`

GetRevokedAt returns the RevokedAt field if non-nil, zero value otherwise.

### GetRevokedAtOk

`func (o *WorkspaceInvitation) GetRevokedAtOk() (*time.Time, bool)`

GetRevokedAtOk returns a tuple with the RevokedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRevokedAt

`func (o *WorkspaceInvitation) SetRevokedAt(v time.Time)`

SetRevokedAt sets RevokedAt field to given value.

### HasRevokedAt

`func (o *WorkspaceInvitation) HasRevokedAt() bool`

HasRevokedAt returns a boolean if a field has been set.

### SetRevokedAtNil

`func (o *WorkspaceInvitation) SetRevokedAtNil(b bool)`

 SetRevokedAtNil sets the value for RevokedAt to be an explicit nil

### UnsetRevokedAt
`func (o *WorkspaceInvitation) UnsetRevokedAt()`

UnsetRevokedAt ensures that no value is present for RevokedAt, not even an explicit nil
### GetStatus

`func (o *WorkspaceInvitation) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *WorkspaceInvitation) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *WorkspaceInvitation) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *WorkspaceInvitation) HasStatus() bool`

HasStatus returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


