# KeyBinding

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**ActionId** | **string** |  | 
**DisplayName** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **string** |  | [optional] 
**Key** | Pointer to **string** |  | [optional] 
**Modifiers** | Pointer to **[]string** |  | [optional] 
**Category** | Pointer to **string** |  | [optional] 
**Scope** | Pointer to **string** |  | [optional] 
**DisplayOrder** | Pointer to **int32** |  | [optional] 
**IsCustom** | Pointer to **bool** |  | [optional] 
**Metadata** | Pointer to **map[string]interface{}** |  | [optional] 

## Methods

### NewKeyBinding

`func NewKeyBinding(id string, actionId string, ) *KeyBinding`

NewKeyBinding instantiates a new KeyBinding object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewKeyBindingWithDefaults

`func NewKeyBindingWithDefaults() *KeyBinding`

NewKeyBindingWithDefaults instantiates a new KeyBinding object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *KeyBinding) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *KeyBinding) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *KeyBinding) SetId(v string)`

SetId sets Id field to given value.


### GetActionId

`func (o *KeyBinding) GetActionId() string`

GetActionId returns the ActionId field if non-nil, zero value otherwise.

### GetActionIdOk

`func (o *KeyBinding) GetActionIdOk() (*string, bool)`

GetActionIdOk returns a tuple with the ActionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActionId

`func (o *KeyBinding) SetActionId(v string)`

SetActionId sets ActionId field to given value.


### GetDisplayName

`func (o *KeyBinding) GetDisplayName() string`

GetDisplayName returns the DisplayName field if non-nil, zero value otherwise.

### GetDisplayNameOk

`func (o *KeyBinding) GetDisplayNameOk() (*string, bool)`

GetDisplayNameOk returns a tuple with the DisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayName

`func (o *KeyBinding) SetDisplayName(v string)`

SetDisplayName sets DisplayName field to given value.

### HasDisplayName

`func (o *KeyBinding) HasDisplayName() bool`

HasDisplayName returns a boolean if a field has been set.

### GetDescription

`func (o *KeyBinding) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *KeyBinding) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *KeyBinding) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *KeyBinding) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetKey

`func (o *KeyBinding) GetKey() string`

GetKey returns the Key field if non-nil, zero value otherwise.

### GetKeyOk

`func (o *KeyBinding) GetKeyOk() (*string, bool)`

GetKeyOk returns a tuple with the Key field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKey

`func (o *KeyBinding) SetKey(v string)`

SetKey sets Key field to given value.

### HasKey

`func (o *KeyBinding) HasKey() bool`

HasKey returns a boolean if a field has been set.

### GetModifiers

`func (o *KeyBinding) GetModifiers() []string`

GetModifiers returns the Modifiers field if non-nil, zero value otherwise.

### GetModifiersOk

`func (o *KeyBinding) GetModifiersOk() (*[]string, bool)`

GetModifiersOk returns a tuple with the Modifiers field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetModifiers

`func (o *KeyBinding) SetModifiers(v []string)`

SetModifiers sets Modifiers field to given value.

### HasModifiers

`func (o *KeyBinding) HasModifiers() bool`

HasModifiers returns a boolean if a field has been set.

### GetCategory

`func (o *KeyBinding) GetCategory() string`

GetCategory returns the Category field if non-nil, zero value otherwise.

### GetCategoryOk

`func (o *KeyBinding) GetCategoryOk() (*string, bool)`

GetCategoryOk returns a tuple with the Category field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCategory

`func (o *KeyBinding) SetCategory(v string)`

SetCategory sets Category field to given value.

### HasCategory

`func (o *KeyBinding) HasCategory() bool`

HasCategory returns a boolean if a field has been set.

### GetScope

`func (o *KeyBinding) GetScope() string`

GetScope returns the Scope field if non-nil, zero value otherwise.

### GetScopeOk

`func (o *KeyBinding) GetScopeOk() (*string, bool)`

GetScopeOk returns a tuple with the Scope field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScope

`func (o *KeyBinding) SetScope(v string)`

SetScope sets Scope field to given value.

### HasScope

`func (o *KeyBinding) HasScope() bool`

HasScope returns a boolean if a field has been set.

### GetDisplayOrder

`func (o *KeyBinding) GetDisplayOrder() int32`

GetDisplayOrder returns the DisplayOrder field if non-nil, zero value otherwise.

### GetDisplayOrderOk

`func (o *KeyBinding) GetDisplayOrderOk() (*int32, bool)`

GetDisplayOrderOk returns a tuple with the DisplayOrder field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayOrder

`func (o *KeyBinding) SetDisplayOrder(v int32)`

SetDisplayOrder sets DisplayOrder field to given value.

### HasDisplayOrder

`func (o *KeyBinding) HasDisplayOrder() bool`

HasDisplayOrder returns a boolean if a field has been set.

### GetIsCustom

`func (o *KeyBinding) GetIsCustom() bool`

GetIsCustom returns the IsCustom field if non-nil, zero value otherwise.

### GetIsCustomOk

`func (o *KeyBinding) GetIsCustomOk() (*bool, bool)`

GetIsCustomOk returns a tuple with the IsCustom field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsCustom

`func (o *KeyBinding) SetIsCustom(v bool)`

SetIsCustom sets IsCustom field to given value.

### HasIsCustom

`func (o *KeyBinding) HasIsCustom() bool`

HasIsCustom returns a boolean if a field has been set.

### GetMetadata

`func (o *KeyBinding) GetMetadata() map[string]interface{}`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *KeyBinding) GetMetadataOk() (*map[string]interface{}, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *KeyBinding) SetMetadata(v map[string]interface{})`

SetMetadata sets Metadata field to given value.

### HasMetadata

`func (o *KeyBinding) HasMetadata() bool`

HasMetadata returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


