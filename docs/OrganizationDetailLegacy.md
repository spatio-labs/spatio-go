# OrganizationDetailLegacy

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ID** | **string** |  | 
**Name** | **string** |  | 
**Slug** | **string** |  | 
**Description** | Pointer to **NullableString** |  | [optional] 
**LogoURL** | Pointer to **NullableString** |  | [optional] 
**Settings** | Pointer to **string** | JSON-encoded settings string. Parse client-side. | [optional] 
**SubscriptionTier** | **string** |  | 
**DeploymentType** | **string** |  | 
**SubscriptionStatus** | **string** |  | 
**CreatedAt** | **time.Time** |  | 
**UpdatedAt** | **time.Time** |  | 

## Methods

### NewOrganizationDetailLegacy

`func NewOrganizationDetailLegacy(iD string, name string, slug string, subscriptionTier string, deploymentType string, subscriptionStatus string, createdAt time.Time, updatedAt time.Time, ) *OrganizationDetailLegacy`

NewOrganizationDetailLegacy instantiates a new OrganizationDetailLegacy object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewOrganizationDetailLegacyWithDefaults

`func NewOrganizationDetailLegacyWithDefaults() *OrganizationDetailLegacy`

NewOrganizationDetailLegacyWithDefaults instantiates a new OrganizationDetailLegacy object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetID

`func (o *OrganizationDetailLegacy) GetID() string`

GetID returns the ID field if non-nil, zero value otherwise.

### GetIDOk

`func (o *OrganizationDetailLegacy) GetIDOk() (*string, bool)`

GetIDOk returns a tuple with the ID field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetID

`func (o *OrganizationDetailLegacy) SetID(v string)`

SetID sets ID field to given value.


### GetName

`func (o *OrganizationDetailLegacy) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *OrganizationDetailLegacy) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *OrganizationDetailLegacy) SetName(v string)`

SetName sets Name field to given value.


### GetSlug

`func (o *OrganizationDetailLegacy) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *OrganizationDetailLegacy) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *OrganizationDetailLegacy) SetSlug(v string)`

SetSlug sets Slug field to given value.


### GetDescription

`func (o *OrganizationDetailLegacy) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *OrganizationDetailLegacy) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *OrganizationDetailLegacy) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *OrganizationDetailLegacy) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *OrganizationDetailLegacy) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *OrganizationDetailLegacy) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetLogoURL

`func (o *OrganizationDetailLegacy) GetLogoURL() string`

GetLogoURL returns the LogoURL field if non-nil, zero value otherwise.

### GetLogoURLOk

`func (o *OrganizationDetailLegacy) GetLogoURLOk() (*string, bool)`

GetLogoURLOk returns a tuple with the LogoURL field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogoURL

`func (o *OrganizationDetailLegacy) SetLogoURL(v string)`

SetLogoURL sets LogoURL field to given value.

### HasLogoURL

`func (o *OrganizationDetailLegacy) HasLogoURL() bool`

HasLogoURL returns a boolean if a field has been set.

### SetLogoURLNil

`func (o *OrganizationDetailLegacy) SetLogoURLNil(b bool)`

 SetLogoURLNil sets the value for LogoURL to be an explicit nil

### UnsetLogoURL
`func (o *OrganizationDetailLegacy) UnsetLogoURL()`

UnsetLogoURL ensures that no value is present for LogoURL, not even an explicit nil
### GetSettings

`func (o *OrganizationDetailLegacy) GetSettings() string`

GetSettings returns the Settings field if non-nil, zero value otherwise.

### GetSettingsOk

`func (o *OrganizationDetailLegacy) GetSettingsOk() (*string, bool)`

GetSettingsOk returns a tuple with the Settings field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSettings

`func (o *OrganizationDetailLegacy) SetSettings(v string)`

SetSettings sets Settings field to given value.

### HasSettings

`func (o *OrganizationDetailLegacy) HasSettings() bool`

HasSettings returns a boolean if a field has been set.

### GetSubscriptionTier

`func (o *OrganizationDetailLegacy) GetSubscriptionTier() string`

GetSubscriptionTier returns the SubscriptionTier field if non-nil, zero value otherwise.

### GetSubscriptionTierOk

`func (o *OrganizationDetailLegacy) GetSubscriptionTierOk() (*string, bool)`

GetSubscriptionTierOk returns a tuple with the SubscriptionTier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubscriptionTier

`func (o *OrganizationDetailLegacy) SetSubscriptionTier(v string)`

SetSubscriptionTier sets SubscriptionTier field to given value.


### GetDeploymentType

`func (o *OrganizationDetailLegacy) GetDeploymentType() string`

GetDeploymentType returns the DeploymentType field if non-nil, zero value otherwise.

### GetDeploymentTypeOk

`func (o *OrganizationDetailLegacy) GetDeploymentTypeOk() (*string, bool)`

GetDeploymentTypeOk returns a tuple with the DeploymentType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeploymentType

`func (o *OrganizationDetailLegacy) SetDeploymentType(v string)`

SetDeploymentType sets DeploymentType field to given value.


### GetSubscriptionStatus

`func (o *OrganizationDetailLegacy) GetSubscriptionStatus() string`

GetSubscriptionStatus returns the SubscriptionStatus field if non-nil, zero value otherwise.

### GetSubscriptionStatusOk

`func (o *OrganizationDetailLegacy) GetSubscriptionStatusOk() (*string, bool)`

GetSubscriptionStatusOk returns a tuple with the SubscriptionStatus field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubscriptionStatus

`func (o *OrganizationDetailLegacy) SetSubscriptionStatus(v string)`

SetSubscriptionStatus sets SubscriptionStatus field to given value.


### GetCreatedAt

`func (o *OrganizationDetailLegacy) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *OrganizationDetailLegacy) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *OrganizationDetailLegacy) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *OrganizationDetailLegacy) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *OrganizationDetailLegacy) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *OrganizationDetailLegacy) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


