# CreateRecordTypeRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OrganizationId** | Pointer to **string** |  | [optional] 
**Slug** | Pointer to **string** |  | [optional] 
**Name** | **string** |  | 
**NamePlural** | Pointer to **string** |  | [optional] 
**Icon** | Pointer to **string** |  | [optional] 
**AttributeSchema** | Pointer to **[]map[string]interface{}** |  | [optional] 

## Methods

### NewCreateRecordTypeRequest

`func NewCreateRecordTypeRequest(name string, ) *CreateRecordTypeRequest`

NewCreateRecordTypeRequest instantiates a new CreateRecordTypeRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateRecordTypeRequestWithDefaults

`func NewCreateRecordTypeRequestWithDefaults() *CreateRecordTypeRequest`

NewCreateRecordTypeRequestWithDefaults instantiates a new CreateRecordTypeRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetOrganizationId

`func (o *CreateRecordTypeRequest) GetOrganizationId() string`

GetOrganizationId returns the OrganizationId field if non-nil, zero value otherwise.

### GetOrganizationIdOk

`func (o *CreateRecordTypeRequest) GetOrganizationIdOk() (*string, bool)`

GetOrganizationIdOk returns a tuple with the OrganizationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrganizationId

`func (o *CreateRecordTypeRequest) SetOrganizationId(v string)`

SetOrganizationId sets OrganizationId field to given value.

### HasOrganizationId

`func (o *CreateRecordTypeRequest) HasOrganizationId() bool`

HasOrganizationId returns a boolean if a field has been set.

### GetSlug

`func (o *CreateRecordTypeRequest) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *CreateRecordTypeRequest) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *CreateRecordTypeRequest) SetSlug(v string)`

SetSlug sets Slug field to given value.

### HasSlug

`func (o *CreateRecordTypeRequest) HasSlug() bool`

HasSlug returns a boolean if a field has been set.

### GetName

`func (o *CreateRecordTypeRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateRecordTypeRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateRecordTypeRequest) SetName(v string)`

SetName sets Name field to given value.


### GetNamePlural

`func (o *CreateRecordTypeRequest) GetNamePlural() string`

GetNamePlural returns the NamePlural field if non-nil, zero value otherwise.

### GetNamePluralOk

`func (o *CreateRecordTypeRequest) GetNamePluralOk() (*string, bool)`

GetNamePluralOk returns a tuple with the NamePlural field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNamePlural

`func (o *CreateRecordTypeRequest) SetNamePlural(v string)`

SetNamePlural sets NamePlural field to given value.

### HasNamePlural

`func (o *CreateRecordTypeRequest) HasNamePlural() bool`

HasNamePlural returns a boolean if a field has been set.

### GetIcon

`func (o *CreateRecordTypeRequest) GetIcon() string`

GetIcon returns the Icon field if non-nil, zero value otherwise.

### GetIconOk

`func (o *CreateRecordTypeRequest) GetIconOk() (*string, bool)`

GetIconOk returns a tuple with the Icon field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIcon

`func (o *CreateRecordTypeRequest) SetIcon(v string)`

SetIcon sets Icon field to given value.

### HasIcon

`func (o *CreateRecordTypeRequest) HasIcon() bool`

HasIcon returns a boolean if a field has been set.

### GetAttributeSchema

`func (o *CreateRecordTypeRequest) GetAttributeSchema() []map[string]interface{}`

GetAttributeSchema returns the AttributeSchema field if non-nil, zero value otherwise.

### GetAttributeSchemaOk

`func (o *CreateRecordTypeRequest) GetAttributeSchemaOk() (*[]map[string]interface{}, bool)`

GetAttributeSchemaOk returns a tuple with the AttributeSchema field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeSchema

`func (o *CreateRecordTypeRequest) SetAttributeSchema(v []map[string]interface{})`

SetAttributeSchema sets AttributeSchema field to given value.

### HasAttributeSchema

`func (o *CreateRecordTypeRequest) HasAttributeSchema() bool`

HasAttributeSchema returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


