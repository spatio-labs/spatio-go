# Presentation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Provider** | Pointer to **string** |  | [optional] 
**AccountId** | Pointer to **string** |  | [optional] 
**OwnerUserId** | Pointer to **string** |  | [optional] 
**Title** | **string** |  | 
**Description** | Pointer to **string** |  | [optional] 
**Theme** | Pointer to **string** | Free-form theme id; provider-specific. | [optional] 
**ThumbnailUrl** | Pointer to **string** |  | [optional] 
**CreatedAt** | **time.Time** |  | 
**UpdatedAt** | **time.Time** |  | 
**LastViewedAt** | Pointer to **NullableTime** |  | [optional] 

## Methods

### NewPresentation

`func NewPresentation(id string, title string, createdAt time.Time, updatedAt time.Time, ) *Presentation`

NewPresentation instantiates a new Presentation object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPresentationWithDefaults

`func NewPresentationWithDefaults() *Presentation`

NewPresentationWithDefaults instantiates a new Presentation object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Presentation) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Presentation) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Presentation) SetId(v string)`

SetId sets Id field to given value.


### GetProvider

`func (o *Presentation) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *Presentation) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *Presentation) SetProvider(v string)`

SetProvider sets Provider field to given value.

### HasProvider

`func (o *Presentation) HasProvider() bool`

HasProvider returns a boolean if a field has been set.

### GetAccountId

`func (o *Presentation) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *Presentation) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *Presentation) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *Presentation) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.

### GetOwnerUserId

`func (o *Presentation) GetOwnerUserId() string`

GetOwnerUserId returns the OwnerUserId field if non-nil, zero value otherwise.

### GetOwnerUserIdOk

`func (o *Presentation) GetOwnerUserIdOk() (*string, bool)`

GetOwnerUserIdOk returns a tuple with the OwnerUserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOwnerUserId

`func (o *Presentation) SetOwnerUserId(v string)`

SetOwnerUserId sets OwnerUserId field to given value.

### HasOwnerUserId

`func (o *Presentation) HasOwnerUserId() bool`

HasOwnerUserId returns a boolean if a field has been set.

### GetTitle

`func (o *Presentation) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *Presentation) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *Presentation) SetTitle(v string)`

SetTitle sets Title field to given value.


### GetDescription

`func (o *Presentation) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *Presentation) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *Presentation) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *Presentation) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetTheme

`func (o *Presentation) GetTheme() string`

GetTheme returns the Theme field if non-nil, zero value otherwise.

### GetThemeOk

`func (o *Presentation) GetThemeOk() (*string, bool)`

GetThemeOk returns a tuple with the Theme field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTheme

`func (o *Presentation) SetTheme(v string)`

SetTheme sets Theme field to given value.

### HasTheme

`func (o *Presentation) HasTheme() bool`

HasTheme returns a boolean if a field has been set.

### GetThumbnailUrl

`func (o *Presentation) GetThumbnailUrl() string`

GetThumbnailUrl returns the ThumbnailUrl field if non-nil, zero value otherwise.

### GetThumbnailUrlOk

`func (o *Presentation) GetThumbnailUrlOk() (*string, bool)`

GetThumbnailUrlOk returns a tuple with the ThumbnailUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetThumbnailUrl

`func (o *Presentation) SetThumbnailUrl(v string)`

SetThumbnailUrl sets ThumbnailUrl field to given value.

### HasThumbnailUrl

`func (o *Presentation) HasThumbnailUrl() bool`

HasThumbnailUrl returns a boolean if a field has been set.

### GetCreatedAt

`func (o *Presentation) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Presentation) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Presentation) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *Presentation) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *Presentation) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *Presentation) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.


### GetLastViewedAt

`func (o *Presentation) GetLastViewedAt() time.Time`

GetLastViewedAt returns the LastViewedAt field if non-nil, zero value otherwise.

### GetLastViewedAtOk

`func (o *Presentation) GetLastViewedAtOk() (*time.Time, bool)`

GetLastViewedAtOk returns a tuple with the LastViewedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastViewedAt

`func (o *Presentation) SetLastViewedAt(v time.Time)`

SetLastViewedAt sets LastViewedAt field to given value.

### HasLastViewedAt

`func (o *Presentation) HasLastViewedAt() bool`

HasLastViewedAt returns a boolean if a field has been set.

### SetLastViewedAtNil

`func (o *Presentation) SetLastViewedAtNil(b bool)`

 SetLastViewedAtNil sets the value for LastViewedAt to be an explicit nil

### UnsetLastViewedAt
`func (o *Presentation) UnsetLastViewedAt()`

UnsetLastViewedAt ensures that no value is present for LastViewedAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


