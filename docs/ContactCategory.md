# ContactCategory

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Name** | **string** |  | 
**Color** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **string** |  | [optional] 
**OrganizationId** | Pointer to **string** |  | [optional] 

## Methods

### NewContactCategory

`func NewContactCategory(id string, name string, ) *ContactCategory`

NewContactCategory instantiates a new ContactCategory object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewContactCategoryWithDefaults

`func NewContactCategoryWithDefaults() *ContactCategory`

NewContactCategoryWithDefaults instantiates a new ContactCategory object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ContactCategory) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ContactCategory) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ContactCategory) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *ContactCategory) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ContactCategory) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ContactCategory) SetName(v string)`

SetName sets Name field to given value.


### GetColor

`func (o *ContactCategory) GetColor() string`

GetColor returns the Color field if non-nil, zero value otherwise.

### GetColorOk

`func (o *ContactCategory) GetColorOk() (*string, bool)`

GetColorOk returns a tuple with the Color field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetColor

`func (o *ContactCategory) SetColor(v string)`

SetColor sets Color field to given value.

### HasColor

`func (o *ContactCategory) HasColor() bool`

HasColor returns a boolean if a field has been set.

### GetDescription

`func (o *ContactCategory) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *ContactCategory) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *ContactCategory) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *ContactCategory) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetOrganizationId

`func (o *ContactCategory) GetOrganizationId() string`

GetOrganizationId returns the OrganizationId field if non-nil, zero value otherwise.

### GetOrganizationIdOk

`func (o *ContactCategory) GetOrganizationIdOk() (*string, bool)`

GetOrganizationIdOk returns a tuple with the OrganizationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrganizationId

`func (o *ContactCategory) SetOrganizationId(v string)`

SetOrganizationId sets OrganizationId field to given value.

### HasOrganizationId

`func (o *ContactCategory) HasOrganizationId() bool`

HasOrganizationId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


