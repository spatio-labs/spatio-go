# Organization

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Name** | **string** |  | 
**Slug** | **string** |  | 
**Description** | Pointer to **NullableString** |  | [optional] 
**LogoUrl** | Pointer to **NullableString** |  | [optional] 
**Role** | **string** | The caller&#39;s role in this org (&#x60;owner&#x60;, &#x60;admin&#x60;, &#x60;billing_admin&#x60;, &#x60;member&#x60;). | 
**MemberCount** | Pointer to **int32** |  | [optional] 
**WorkspaceCount** | Pointer to **int32** |  | [optional] 
**Workspaces** | Pointer to [**[]OrganizationWorkspacesInner**](OrganizationWorkspacesInner.md) | Compact workspace summaries embedded in the org-list response. | [optional] 
**CreatedAt** | **time.Time** |  | 
**UpdatedAt** | **time.Time** |  | 

## Methods

### NewOrganization

`func NewOrganization(id string, name string, slug string, role string, createdAt time.Time, updatedAt time.Time, ) *Organization`

NewOrganization instantiates a new Organization object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewOrganizationWithDefaults

`func NewOrganizationWithDefaults() *Organization`

NewOrganizationWithDefaults instantiates a new Organization object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Organization) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Organization) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Organization) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *Organization) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Organization) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Organization) SetName(v string)`

SetName sets Name field to given value.


### GetSlug

`func (o *Organization) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *Organization) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *Organization) SetSlug(v string)`

SetSlug sets Slug field to given value.


### GetDescription

`func (o *Organization) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *Organization) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *Organization) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *Organization) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *Organization) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *Organization) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetLogoUrl

`func (o *Organization) GetLogoUrl() string`

GetLogoUrl returns the LogoUrl field if non-nil, zero value otherwise.

### GetLogoUrlOk

`func (o *Organization) GetLogoUrlOk() (*string, bool)`

GetLogoUrlOk returns a tuple with the LogoUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogoUrl

`func (o *Organization) SetLogoUrl(v string)`

SetLogoUrl sets LogoUrl field to given value.

### HasLogoUrl

`func (o *Organization) HasLogoUrl() bool`

HasLogoUrl returns a boolean if a field has been set.

### SetLogoUrlNil

`func (o *Organization) SetLogoUrlNil(b bool)`

 SetLogoUrlNil sets the value for LogoUrl to be an explicit nil

### UnsetLogoUrl
`func (o *Organization) UnsetLogoUrl()`

UnsetLogoUrl ensures that no value is present for LogoUrl, not even an explicit nil
### GetRole

`func (o *Organization) GetRole() string`

GetRole returns the Role field if non-nil, zero value otherwise.

### GetRoleOk

`func (o *Organization) GetRoleOk() (*string, bool)`

GetRoleOk returns a tuple with the Role field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRole

`func (o *Organization) SetRole(v string)`

SetRole sets Role field to given value.


### GetMemberCount

`func (o *Organization) GetMemberCount() int32`

GetMemberCount returns the MemberCount field if non-nil, zero value otherwise.

### GetMemberCountOk

`func (o *Organization) GetMemberCountOk() (*int32, bool)`

GetMemberCountOk returns a tuple with the MemberCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMemberCount

`func (o *Organization) SetMemberCount(v int32)`

SetMemberCount sets MemberCount field to given value.

### HasMemberCount

`func (o *Organization) HasMemberCount() bool`

HasMemberCount returns a boolean if a field has been set.

### GetWorkspaceCount

`func (o *Organization) GetWorkspaceCount() int32`

GetWorkspaceCount returns the WorkspaceCount field if non-nil, zero value otherwise.

### GetWorkspaceCountOk

`func (o *Organization) GetWorkspaceCountOk() (*int32, bool)`

GetWorkspaceCountOk returns a tuple with the WorkspaceCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWorkspaceCount

`func (o *Organization) SetWorkspaceCount(v int32)`

SetWorkspaceCount sets WorkspaceCount field to given value.

### HasWorkspaceCount

`func (o *Organization) HasWorkspaceCount() bool`

HasWorkspaceCount returns a boolean if a field has been set.

### GetWorkspaces

`func (o *Organization) GetWorkspaces() []OrganizationWorkspacesInner`

GetWorkspaces returns the Workspaces field if non-nil, zero value otherwise.

### GetWorkspacesOk

`func (o *Organization) GetWorkspacesOk() (*[]OrganizationWorkspacesInner, bool)`

GetWorkspacesOk returns a tuple with the Workspaces field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWorkspaces

`func (o *Organization) SetWorkspaces(v []OrganizationWorkspacesInner)`

SetWorkspaces sets Workspaces field to given value.

### HasWorkspaces

`func (o *Organization) HasWorkspaces() bool`

HasWorkspaces returns a boolean if a field has been set.

### GetCreatedAt

`func (o *Organization) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Organization) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Organization) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *Organization) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *Organization) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *Organization) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


