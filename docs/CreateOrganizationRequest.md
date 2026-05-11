# CreateOrganizationRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** |  | 
**Slug** | Pointer to **string** | Auto-generated from &#x60;name&#x60; if omitted. Slug collisions are auto-suffixed with &#x60;-2&#x60;, &#x60;-3&#x60;, etc.  | [optional] 
**Description** | Pointer to **string** |  | [optional] 
**LogoUrl** | Pointer to **string** |  | [optional] 
**CreateDefaultWorkspace** | Pointer to **bool** | &#x60;true&#x60; (default) creates a default workspace alongside the org. | [optional] 
**DefaultWorkspaceName** | Pointer to **string** |  | [optional] 

## Methods

### NewCreateOrganizationRequest

`func NewCreateOrganizationRequest(name string, ) *CreateOrganizationRequest`

NewCreateOrganizationRequest instantiates a new CreateOrganizationRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateOrganizationRequestWithDefaults

`func NewCreateOrganizationRequestWithDefaults() *CreateOrganizationRequest`

NewCreateOrganizationRequestWithDefaults instantiates a new CreateOrganizationRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *CreateOrganizationRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateOrganizationRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateOrganizationRequest) SetName(v string)`

SetName sets Name field to given value.


### GetSlug

`func (o *CreateOrganizationRequest) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *CreateOrganizationRequest) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *CreateOrganizationRequest) SetSlug(v string)`

SetSlug sets Slug field to given value.

### HasSlug

`func (o *CreateOrganizationRequest) HasSlug() bool`

HasSlug returns a boolean if a field has been set.

### GetDescription

`func (o *CreateOrganizationRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *CreateOrganizationRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *CreateOrganizationRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *CreateOrganizationRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetLogoUrl

`func (o *CreateOrganizationRequest) GetLogoUrl() string`

GetLogoUrl returns the LogoUrl field if non-nil, zero value otherwise.

### GetLogoUrlOk

`func (o *CreateOrganizationRequest) GetLogoUrlOk() (*string, bool)`

GetLogoUrlOk returns a tuple with the LogoUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogoUrl

`func (o *CreateOrganizationRequest) SetLogoUrl(v string)`

SetLogoUrl sets LogoUrl field to given value.

### HasLogoUrl

`func (o *CreateOrganizationRequest) HasLogoUrl() bool`

HasLogoUrl returns a boolean if a field has been set.

### GetCreateDefaultWorkspace

`func (o *CreateOrganizationRequest) GetCreateDefaultWorkspace() bool`

GetCreateDefaultWorkspace returns the CreateDefaultWorkspace field if non-nil, zero value otherwise.

### GetCreateDefaultWorkspaceOk

`func (o *CreateOrganizationRequest) GetCreateDefaultWorkspaceOk() (*bool, bool)`

GetCreateDefaultWorkspaceOk returns a tuple with the CreateDefaultWorkspace field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreateDefaultWorkspace

`func (o *CreateOrganizationRequest) SetCreateDefaultWorkspace(v bool)`

SetCreateDefaultWorkspace sets CreateDefaultWorkspace field to given value.

### HasCreateDefaultWorkspace

`func (o *CreateOrganizationRequest) HasCreateDefaultWorkspace() bool`

HasCreateDefaultWorkspace returns a boolean if a field has been set.

### GetDefaultWorkspaceName

`func (o *CreateOrganizationRequest) GetDefaultWorkspaceName() string`

GetDefaultWorkspaceName returns the DefaultWorkspaceName field if non-nil, zero value otherwise.

### GetDefaultWorkspaceNameOk

`func (o *CreateOrganizationRequest) GetDefaultWorkspaceNameOk() (*string, bool)`

GetDefaultWorkspaceNameOk returns a tuple with the DefaultWorkspaceName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultWorkspaceName

`func (o *CreateOrganizationRequest) SetDefaultWorkspaceName(v string)`

SetDefaultWorkspaceName sets DefaultWorkspaceName field to given value.

### HasDefaultWorkspaceName

`func (o *CreateOrganizationRequest) HasDefaultWorkspaceName() bool`

HasDefaultWorkspaceName returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


