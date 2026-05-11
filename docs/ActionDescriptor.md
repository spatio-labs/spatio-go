# ActionDescriptor

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**CanonicalId** | Pointer to **string** |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **string** |  | [optional] 
**Category** | Pointer to **string** |  | [optional] 
**InputType** | Pointer to **string** |  | [optional] 
**OutputType** | Pointer to **string** |  | [optional] 
**Metadata** | Pointer to **map[string]interface{}** |  | [optional] 

## Methods

### NewActionDescriptor

`func NewActionDescriptor(id string, ) *ActionDescriptor`

NewActionDescriptor instantiates a new ActionDescriptor object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewActionDescriptorWithDefaults

`func NewActionDescriptorWithDefaults() *ActionDescriptor`

NewActionDescriptorWithDefaults instantiates a new ActionDescriptor object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ActionDescriptor) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ActionDescriptor) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ActionDescriptor) SetId(v string)`

SetId sets Id field to given value.


### GetCanonicalId

`func (o *ActionDescriptor) GetCanonicalId() string`

GetCanonicalId returns the CanonicalId field if non-nil, zero value otherwise.

### GetCanonicalIdOk

`func (o *ActionDescriptor) GetCanonicalIdOk() (*string, bool)`

GetCanonicalIdOk returns a tuple with the CanonicalId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCanonicalId

`func (o *ActionDescriptor) SetCanonicalId(v string)`

SetCanonicalId sets CanonicalId field to given value.

### HasCanonicalId

`func (o *ActionDescriptor) HasCanonicalId() bool`

HasCanonicalId returns a boolean if a field has been set.

### GetName

`func (o *ActionDescriptor) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ActionDescriptor) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ActionDescriptor) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *ActionDescriptor) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDescription

`func (o *ActionDescriptor) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *ActionDescriptor) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *ActionDescriptor) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *ActionDescriptor) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetCategory

`func (o *ActionDescriptor) GetCategory() string`

GetCategory returns the Category field if non-nil, zero value otherwise.

### GetCategoryOk

`func (o *ActionDescriptor) GetCategoryOk() (*string, bool)`

GetCategoryOk returns a tuple with the Category field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCategory

`func (o *ActionDescriptor) SetCategory(v string)`

SetCategory sets Category field to given value.

### HasCategory

`func (o *ActionDescriptor) HasCategory() bool`

HasCategory returns a boolean if a field has been set.

### GetInputType

`func (o *ActionDescriptor) GetInputType() string`

GetInputType returns the InputType field if non-nil, zero value otherwise.

### GetInputTypeOk

`func (o *ActionDescriptor) GetInputTypeOk() (*string, bool)`

GetInputTypeOk returns a tuple with the InputType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInputType

`func (o *ActionDescriptor) SetInputType(v string)`

SetInputType sets InputType field to given value.

### HasInputType

`func (o *ActionDescriptor) HasInputType() bool`

HasInputType returns a boolean if a field has been set.

### GetOutputType

`func (o *ActionDescriptor) GetOutputType() string`

GetOutputType returns the OutputType field if non-nil, zero value otherwise.

### GetOutputTypeOk

`func (o *ActionDescriptor) GetOutputTypeOk() (*string, bool)`

GetOutputTypeOk returns a tuple with the OutputType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOutputType

`func (o *ActionDescriptor) SetOutputType(v string)`

SetOutputType sets OutputType field to given value.

### HasOutputType

`func (o *ActionDescriptor) HasOutputType() bool`

HasOutputType returns a boolean if a field has been set.

### GetMetadata

`func (o *ActionDescriptor) GetMetadata() map[string]interface{}`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *ActionDescriptor) GetMetadataOk() (*map[string]interface{}, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *ActionDescriptor) SetMetadata(v map[string]interface{})`

SetMetadata sets Metadata field to given value.

### HasMetadata

`func (o *ActionDescriptor) HasMetadata() bool`

HasMetadata returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


