# CreateOrganizationInvitationRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Email** | **string** |  | 
**Role** | **string** |  | 
**WorkspaceId** | Pointer to **string** | Optional — the invitee will also be added to this workspace on accept. Defaults to the org&#39;s default workspace.  | [optional] 

## Methods

### NewCreateOrganizationInvitationRequest

`func NewCreateOrganizationInvitationRequest(email string, role string, ) *CreateOrganizationInvitationRequest`

NewCreateOrganizationInvitationRequest instantiates a new CreateOrganizationInvitationRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateOrganizationInvitationRequestWithDefaults

`func NewCreateOrganizationInvitationRequestWithDefaults() *CreateOrganizationInvitationRequest`

NewCreateOrganizationInvitationRequestWithDefaults instantiates a new CreateOrganizationInvitationRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEmail

`func (o *CreateOrganizationInvitationRequest) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *CreateOrganizationInvitationRequest) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *CreateOrganizationInvitationRequest) SetEmail(v string)`

SetEmail sets Email field to given value.


### GetRole

`func (o *CreateOrganizationInvitationRequest) GetRole() string`

GetRole returns the Role field if non-nil, zero value otherwise.

### GetRoleOk

`func (o *CreateOrganizationInvitationRequest) GetRoleOk() (*string, bool)`

GetRoleOk returns a tuple with the Role field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRole

`func (o *CreateOrganizationInvitationRequest) SetRole(v string)`

SetRole sets Role field to given value.


### GetWorkspaceId

`func (o *CreateOrganizationInvitationRequest) GetWorkspaceId() string`

GetWorkspaceId returns the WorkspaceId field if non-nil, zero value otherwise.

### GetWorkspaceIdOk

`func (o *CreateOrganizationInvitationRequest) GetWorkspaceIdOk() (*string, bool)`

GetWorkspaceIdOk returns a tuple with the WorkspaceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWorkspaceId

`func (o *CreateOrganizationInvitationRequest) SetWorkspaceId(v string)`

SetWorkspaceId sets WorkspaceId field to given value.

### HasWorkspaceId

`func (o *CreateOrganizationInvitationRequest) HasWorkspaceId() bool`

HasWorkspaceId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


