# Workspace

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Name** | **string** |  | 
**Slug** | **string** |  | 
**Description** | Pointer to **NullableString** |  | [optional] 
**LogoUrl** | Pointer to **NullableString** |  | [optional] 
**OrganizationId** | Pointer to **string** |  | [optional] 
**Organization** | Pointer to [**WorkspaceOrganization**](WorkspaceOrganization.md) |  | [optional] 
**Role** | Pointer to **string** | The caller&#39;s role in this workspace (&#x60;owner&#x60;, &#x60;admin&#x60;, &#x60;member&#x60;, &#x60;guest&#x60;). | [optional] 
**Settings** | Pointer to **interface{}** | Per-workspace settings. Currently emitted as either an object (&#x60;{language, timezone, ...}&#x60;) on &#x60;GET /v1/workspaces/{id}&#x60; or a JSON-encoded string on &#x60;GET /v1/organizations/{id}/workspaces&#x60;. Treat as opaque and parse defensively.  | [optional] 
**IsDefault** | Pointer to **bool** |  | [optional] 
**MemberCount** | Pointer to **int32** |  | [optional] 
**BillingTier** | Pointer to **string** |  | [optional] 
**CreatedAt** | Pointer to **time.Time** |  | [optional] 
**UpdatedAt** | Pointer to **time.Time** |  | [optional] 

## Methods

### NewWorkspace

`func NewWorkspace(id string, name string, slug string, ) *Workspace`

NewWorkspace instantiates a new Workspace object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWorkspaceWithDefaults

`func NewWorkspaceWithDefaults() *Workspace`

NewWorkspaceWithDefaults instantiates a new Workspace object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Workspace) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Workspace) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Workspace) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *Workspace) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Workspace) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Workspace) SetName(v string)`

SetName sets Name field to given value.


### GetSlug

`func (o *Workspace) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *Workspace) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *Workspace) SetSlug(v string)`

SetSlug sets Slug field to given value.


### GetDescription

`func (o *Workspace) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *Workspace) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *Workspace) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *Workspace) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *Workspace) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *Workspace) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetLogoUrl

`func (o *Workspace) GetLogoUrl() string`

GetLogoUrl returns the LogoUrl field if non-nil, zero value otherwise.

### GetLogoUrlOk

`func (o *Workspace) GetLogoUrlOk() (*string, bool)`

GetLogoUrlOk returns a tuple with the LogoUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogoUrl

`func (o *Workspace) SetLogoUrl(v string)`

SetLogoUrl sets LogoUrl field to given value.

### HasLogoUrl

`func (o *Workspace) HasLogoUrl() bool`

HasLogoUrl returns a boolean if a field has been set.

### SetLogoUrlNil

`func (o *Workspace) SetLogoUrlNil(b bool)`

 SetLogoUrlNil sets the value for LogoUrl to be an explicit nil

### UnsetLogoUrl
`func (o *Workspace) UnsetLogoUrl()`

UnsetLogoUrl ensures that no value is present for LogoUrl, not even an explicit nil
### GetOrganizationId

`func (o *Workspace) GetOrganizationId() string`

GetOrganizationId returns the OrganizationId field if non-nil, zero value otherwise.

### GetOrganizationIdOk

`func (o *Workspace) GetOrganizationIdOk() (*string, bool)`

GetOrganizationIdOk returns a tuple with the OrganizationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrganizationId

`func (o *Workspace) SetOrganizationId(v string)`

SetOrganizationId sets OrganizationId field to given value.

### HasOrganizationId

`func (o *Workspace) HasOrganizationId() bool`

HasOrganizationId returns a boolean if a field has been set.

### GetOrganization

`func (o *Workspace) GetOrganization() WorkspaceOrganization`

GetOrganization returns the Organization field if non-nil, zero value otherwise.

### GetOrganizationOk

`func (o *Workspace) GetOrganizationOk() (*WorkspaceOrganization, bool)`

GetOrganizationOk returns a tuple with the Organization field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrganization

`func (o *Workspace) SetOrganization(v WorkspaceOrganization)`

SetOrganization sets Organization field to given value.

### HasOrganization

`func (o *Workspace) HasOrganization() bool`

HasOrganization returns a boolean if a field has been set.

### GetRole

`func (o *Workspace) GetRole() string`

GetRole returns the Role field if non-nil, zero value otherwise.

### GetRoleOk

`func (o *Workspace) GetRoleOk() (*string, bool)`

GetRoleOk returns a tuple with the Role field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRole

`func (o *Workspace) SetRole(v string)`

SetRole sets Role field to given value.

### HasRole

`func (o *Workspace) HasRole() bool`

HasRole returns a boolean if a field has been set.

### GetSettings

`func (o *Workspace) GetSettings() interface{}`

GetSettings returns the Settings field if non-nil, zero value otherwise.

### GetSettingsOk

`func (o *Workspace) GetSettingsOk() (*interface{}, bool)`

GetSettingsOk returns a tuple with the Settings field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSettings

`func (o *Workspace) SetSettings(v interface{})`

SetSettings sets Settings field to given value.

### HasSettings

`func (o *Workspace) HasSettings() bool`

HasSettings returns a boolean if a field has been set.

### SetSettingsNil

`func (o *Workspace) SetSettingsNil(b bool)`

 SetSettingsNil sets the value for Settings to be an explicit nil

### UnsetSettings
`func (o *Workspace) UnsetSettings()`

UnsetSettings ensures that no value is present for Settings, not even an explicit nil
### GetIsDefault

`func (o *Workspace) GetIsDefault() bool`

GetIsDefault returns the IsDefault field if non-nil, zero value otherwise.

### GetIsDefaultOk

`func (o *Workspace) GetIsDefaultOk() (*bool, bool)`

GetIsDefaultOk returns a tuple with the IsDefault field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDefault

`func (o *Workspace) SetIsDefault(v bool)`

SetIsDefault sets IsDefault field to given value.

### HasIsDefault

`func (o *Workspace) HasIsDefault() bool`

HasIsDefault returns a boolean if a field has been set.

### GetMemberCount

`func (o *Workspace) GetMemberCount() int32`

GetMemberCount returns the MemberCount field if non-nil, zero value otherwise.

### GetMemberCountOk

`func (o *Workspace) GetMemberCountOk() (*int32, bool)`

GetMemberCountOk returns a tuple with the MemberCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMemberCount

`func (o *Workspace) SetMemberCount(v int32)`

SetMemberCount sets MemberCount field to given value.

### HasMemberCount

`func (o *Workspace) HasMemberCount() bool`

HasMemberCount returns a boolean if a field has been set.

### GetBillingTier

`func (o *Workspace) GetBillingTier() string`

GetBillingTier returns the BillingTier field if non-nil, zero value otherwise.

### GetBillingTierOk

`func (o *Workspace) GetBillingTierOk() (*string, bool)`

GetBillingTierOk returns a tuple with the BillingTier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBillingTier

`func (o *Workspace) SetBillingTier(v string)`

SetBillingTier sets BillingTier field to given value.

### HasBillingTier

`func (o *Workspace) HasBillingTier() bool`

HasBillingTier returns a boolean if a field has been set.

### GetCreatedAt

`func (o *Workspace) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Workspace) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Workspace) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *Workspace) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetUpdatedAt

`func (o *Workspace) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *Workspace) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *Workspace) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *Workspace) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


