# AddOrganizationMemberRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Email** | **string** |  | 
**Role** | Pointer to **string** |  | [optional] 
**WorkspaceId** | Pointer to **string** |  | [optional] 

## Methods

### NewAddOrganizationMemberRequest

`func NewAddOrganizationMemberRequest(email string, ) *AddOrganizationMemberRequest`

NewAddOrganizationMemberRequest instantiates a new AddOrganizationMemberRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAddOrganizationMemberRequestWithDefaults

`func NewAddOrganizationMemberRequestWithDefaults() *AddOrganizationMemberRequest`

NewAddOrganizationMemberRequestWithDefaults instantiates a new AddOrganizationMemberRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEmail

`func (o *AddOrganizationMemberRequest) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *AddOrganizationMemberRequest) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *AddOrganizationMemberRequest) SetEmail(v string)`

SetEmail sets Email field to given value.


### GetRole

`func (o *AddOrganizationMemberRequest) GetRole() string`

GetRole returns the Role field if non-nil, zero value otherwise.

### GetRoleOk

`func (o *AddOrganizationMemberRequest) GetRoleOk() (*string, bool)`

GetRoleOk returns a tuple with the Role field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRole

`func (o *AddOrganizationMemberRequest) SetRole(v string)`

SetRole sets Role field to given value.

### HasRole

`func (o *AddOrganizationMemberRequest) HasRole() bool`

HasRole returns a boolean if a field has been set.

### GetWorkspaceId

`func (o *AddOrganizationMemberRequest) GetWorkspaceId() string`

GetWorkspaceId returns the WorkspaceId field if non-nil, zero value otherwise.

### GetWorkspaceIdOk

`func (o *AddOrganizationMemberRequest) GetWorkspaceIdOk() (*string, bool)`

GetWorkspaceIdOk returns a tuple with the WorkspaceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWorkspaceId

`func (o *AddOrganizationMemberRequest) SetWorkspaceId(v string)`

SetWorkspaceId sets WorkspaceId field to given value.

### HasWorkspaceId

`func (o *AddOrganizationMemberRequest) HasWorkspaceId() bool`

HasWorkspaceId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


