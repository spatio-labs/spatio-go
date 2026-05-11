# RecordType

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**OrganizationId** | **string** |  | 
**Slug** | Pointer to **string** |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**NamePlural** | Pointer to **string** |  | [optional] 
**Icon** | Pointer to **string** |  | [optional] 
**AttributeSchema** | Pointer to **[]map[string]interface{}** |  | [optional] 
**CreatedAt** | Pointer to **time.Time** |  | [optional] 
**UpdatedAt** | Pointer to **time.Time** |  | [optional] 

## Methods

### NewRecordType

`func NewRecordType(id string, organizationId string, ) *RecordType`

NewRecordType instantiates a new RecordType object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRecordTypeWithDefaults

`func NewRecordTypeWithDefaults() *RecordType`

NewRecordTypeWithDefaults instantiates a new RecordType object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *RecordType) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *RecordType) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *RecordType) SetId(v string)`

SetId sets Id field to given value.


### GetOrganizationId

`func (o *RecordType) GetOrganizationId() string`

GetOrganizationId returns the OrganizationId field if non-nil, zero value otherwise.

### GetOrganizationIdOk

`func (o *RecordType) GetOrganizationIdOk() (*string, bool)`

GetOrganizationIdOk returns a tuple with the OrganizationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrganizationId

`func (o *RecordType) SetOrganizationId(v string)`

SetOrganizationId sets OrganizationId field to given value.


### GetSlug

`func (o *RecordType) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *RecordType) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *RecordType) SetSlug(v string)`

SetSlug sets Slug field to given value.

### HasSlug

`func (o *RecordType) HasSlug() bool`

HasSlug returns a boolean if a field has been set.

### GetName

`func (o *RecordType) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *RecordType) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *RecordType) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *RecordType) HasName() bool`

HasName returns a boolean if a field has been set.

### GetNamePlural

`func (o *RecordType) GetNamePlural() string`

GetNamePlural returns the NamePlural field if non-nil, zero value otherwise.

### GetNamePluralOk

`func (o *RecordType) GetNamePluralOk() (*string, bool)`

GetNamePluralOk returns a tuple with the NamePlural field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNamePlural

`func (o *RecordType) SetNamePlural(v string)`

SetNamePlural sets NamePlural field to given value.

### HasNamePlural

`func (o *RecordType) HasNamePlural() bool`

HasNamePlural returns a boolean if a field has been set.

### GetIcon

`func (o *RecordType) GetIcon() string`

GetIcon returns the Icon field if non-nil, zero value otherwise.

### GetIconOk

`func (o *RecordType) GetIconOk() (*string, bool)`

GetIconOk returns a tuple with the Icon field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIcon

`func (o *RecordType) SetIcon(v string)`

SetIcon sets Icon field to given value.

### HasIcon

`func (o *RecordType) HasIcon() bool`

HasIcon returns a boolean if a field has been set.

### GetAttributeSchema

`func (o *RecordType) GetAttributeSchema() []map[string]interface{}`

GetAttributeSchema returns the AttributeSchema field if non-nil, zero value otherwise.

### GetAttributeSchemaOk

`func (o *RecordType) GetAttributeSchemaOk() (*[]map[string]interface{}, bool)`

GetAttributeSchemaOk returns a tuple with the AttributeSchema field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeSchema

`func (o *RecordType) SetAttributeSchema(v []map[string]interface{})`

SetAttributeSchema sets AttributeSchema field to given value.

### HasAttributeSchema

`func (o *RecordType) HasAttributeSchema() bool`

HasAttributeSchema returns a boolean if a field has been set.

### GetCreatedAt

`func (o *RecordType) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *RecordType) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *RecordType) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *RecordType) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetUpdatedAt

`func (o *RecordType) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *RecordType) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *RecordType) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *RecordType) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


