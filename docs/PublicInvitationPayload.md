# PublicInvitationPayload

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Kind** | **string** |  | 
**Id** | **string** |  | 
**WorkspaceId** | Pointer to **string** |  | [optional] 
**OrganizationId** | Pointer to **string** |  | [optional] 
**Email** | **string** |  | 
**Role** | **string** |  | 
**Status** | **string** |  | 
**ExpiresAt** | Pointer to **NullableTime** |  | [optional] 
**CreatedAt** | Pointer to **time.Time** |  | [optional] 
**Workspace** | Pointer to **map[string]interface{}** |  | [optional] 
**Organization** | Pointer to **map[string]interface{}** |  | [optional] 
**InvitedBy** | Pointer to **map[string]interface{}** |  | [optional] 

## Methods

### NewPublicInvitationPayload

`func NewPublicInvitationPayload(kind string, id string, email string, role string, status string, ) *PublicInvitationPayload`

NewPublicInvitationPayload instantiates a new PublicInvitationPayload object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPublicInvitationPayloadWithDefaults

`func NewPublicInvitationPayloadWithDefaults() *PublicInvitationPayload`

NewPublicInvitationPayloadWithDefaults instantiates a new PublicInvitationPayload object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetKind

`func (o *PublicInvitationPayload) GetKind() string`

GetKind returns the Kind field if non-nil, zero value otherwise.

### GetKindOk

`func (o *PublicInvitationPayload) GetKindOk() (*string, bool)`

GetKindOk returns a tuple with the Kind field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKind

`func (o *PublicInvitationPayload) SetKind(v string)`

SetKind sets Kind field to given value.


### GetId

`func (o *PublicInvitationPayload) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *PublicInvitationPayload) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *PublicInvitationPayload) SetId(v string)`

SetId sets Id field to given value.


### GetWorkspaceId

`func (o *PublicInvitationPayload) GetWorkspaceId() string`

GetWorkspaceId returns the WorkspaceId field if non-nil, zero value otherwise.

### GetWorkspaceIdOk

`func (o *PublicInvitationPayload) GetWorkspaceIdOk() (*string, bool)`

GetWorkspaceIdOk returns a tuple with the WorkspaceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWorkspaceId

`func (o *PublicInvitationPayload) SetWorkspaceId(v string)`

SetWorkspaceId sets WorkspaceId field to given value.

### HasWorkspaceId

`func (o *PublicInvitationPayload) HasWorkspaceId() bool`

HasWorkspaceId returns a boolean if a field has been set.

### GetOrganizationId

`func (o *PublicInvitationPayload) GetOrganizationId() string`

GetOrganizationId returns the OrganizationId field if non-nil, zero value otherwise.

### GetOrganizationIdOk

`func (o *PublicInvitationPayload) GetOrganizationIdOk() (*string, bool)`

GetOrganizationIdOk returns a tuple with the OrganizationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrganizationId

`func (o *PublicInvitationPayload) SetOrganizationId(v string)`

SetOrganizationId sets OrganizationId field to given value.

### HasOrganizationId

`func (o *PublicInvitationPayload) HasOrganizationId() bool`

HasOrganizationId returns a boolean if a field has been set.

### GetEmail

`func (o *PublicInvitationPayload) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *PublicInvitationPayload) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *PublicInvitationPayload) SetEmail(v string)`

SetEmail sets Email field to given value.


### GetRole

`func (o *PublicInvitationPayload) GetRole() string`

GetRole returns the Role field if non-nil, zero value otherwise.

### GetRoleOk

`func (o *PublicInvitationPayload) GetRoleOk() (*string, bool)`

GetRoleOk returns a tuple with the Role field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRole

`func (o *PublicInvitationPayload) SetRole(v string)`

SetRole sets Role field to given value.


### GetStatus

`func (o *PublicInvitationPayload) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *PublicInvitationPayload) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *PublicInvitationPayload) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetExpiresAt

`func (o *PublicInvitationPayload) GetExpiresAt() time.Time`

GetExpiresAt returns the ExpiresAt field if non-nil, zero value otherwise.

### GetExpiresAtOk

`func (o *PublicInvitationPayload) GetExpiresAtOk() (*time.Time, bool)`

GetExpiresAtOk returns a tuple with the ExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresAt

`func (o *PublicInvitationPayload) SetExpiresAt(v time.Time)`

SetExpiresAt sets ExpiresAt field to given value.

### HasExpiresAt

`func (o *PublicInvitationPayload) HasExpiresAt() bool`

HasExpiresAt returns a boolean if a field has been set.

### SetExpiresAtNil

`func (o *PublicInvitationPayload) SetExpiresAtNil(b bool)`

 SetExpiresAtNil sets the value for ExpiresAt to be an explicit nil

### UnsetExpiresAt
`func (o *PublicInvitationPayload) UnsetExpiresAt()`

UnsetExpiresAt ensures that no value is present for ExpiresAt, not even an explicit nil
### GetCreatedAt

`func (o *PublicInvitationPayload) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *PublicInvitationPayload) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *PublicInvitationPayload) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *PublicInvitationPayload) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetWorkspace

`func (o *PublicInvitationPayload) GetWorkspace() map[string]interface{}`

GetWorkspace returns the Workspace field if non-nil, zero value otherwise.

### GetWorkspaceOk

`func (o *PublicInvitationPayload) GetWorkspaceOk() (*map[string]interface{}, bool)`

GetWorkspaceOk returns a tuple with the Workspace field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWorkspace

`func (o *PublicInvitationPayload) SetWorkspace(v map[string]interface{})`

SetWorkspace sets Workspace field to given value.

### HasWorkspace

`func (o *PublicInvitationPayload) HasWorkspace() bool`

HasWorkspace returns a boolean if a field has been set.

### GetOrganization

`func (o *PublicInvitationPayload) GetOrganization() map[string]interface{}`

GetOrganization returns the Organization field if non-nil, zero value otherwise.

### GetOrganizationOk

`func (o *PublicInvitationPayload) GetOrganizationOk() (*map[string]interface{}, bool)`

GetOrganizationOk returns a tuple with the Organization field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrganization

`func (o *PublicInvitationPayload) SetOrganization(v map[string]interface{})`

SetOrganization sets Organization field to given value.

### HasOrganization

`func (o *PublicInvitationPayload) HasOrganization() bool`

HasOrganization returns a boolean if a field has been set.

### GetInvitedBy

`func (o *PublicInvitationPayload) GetInvitedBy() map[string]interface{}`

GetInvitedBy returns the InvitedBy field if non-nil, zero value otherwise.

### GetInvitedByOk

`func (o *PublicInvitationPayload) GetInvitedByOk() (*map[string]interface{}, bool)`

GetInvitedByOk returns a tuple with the InvitedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInvitedBy

`func (o *PublicInvitationPayload) SetInvitedBy(v map[string]interface{})`

SetInvitedBy sets InvitedBy field to given value.

### HasInvitedBy

`func (o *PublicInvitationPayload) HasInvitedBy() bool`

HasInvitedBy returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


