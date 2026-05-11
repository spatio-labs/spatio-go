# ChatActionDefinition

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Name** | **string** |  | 
**Description** | Pointer to **string** |  | [optional] 
**Platform** | **string** |  | 
**Category** | Pointer to **string** | Common values: &#x60;read&#x60;, &#x60;write&#x60;, &#x60;delete&#x60;, &#x60;manage&#x60;, &#x60;sync&#x60;. | [optional] 
**InputType** | Pointer to **string** |  | [optional] 
**OutputType** | Pointer to **string** |  | [optional] 
**Scopes** | Pointer to **[]string** | &#x60;null&#x60; when no scopes are declared (Go nil-slice). | [optional] 
**Metadata** | Pointer to **map[string]interface{}** |  | [optional] 

## Methods

### NewChatActionDefinition

`func NewChatActionDefinition(id string, name string, platform string, ) *ChatActionDefinition`

NewChatActionDefinition instantiates a new ChatActionDefinition object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewChatActionDefinitionWithDefaults

`func NewChatActionDefinitionWithDefaults() *ChatActionDefinition`

NewChatActionDefinitionWithDefaults instantiates a new ChatActionDefinition object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ChatActionDefinition) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ChatActionDefinition) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ChatActionDefinition) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *ChatActionDefinition) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ChatActionDefinition) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ChatActionDefinition) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *ChatActionDefinition) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *ChatActionDefinition) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *ChatActionDefinition) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *ChatActionDefinition) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetPlatform

`func (o *ChatActionDefinition) GetPlatform() string`

GetPlatform returns the Platform field if non-nil, zero value otherwise.

### GetPlatformOk

`func (o *ChatActionDefinition) GetPlatformOk() (*string, bool)`

GetPlatformOk returns a tuple with the Platform field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPlatform

`func (o *ChatActionDefinition) SetPlatform(v string)`

SetPlatform sets Platform field to given value.


### GetCategory

`func (o *ChatActionDefinition) GetCategory() string`

GetCategory returns the Category field if non-nil, zero value otherwise.

### GetCategoryOk

`func (o *ChatActionDefinition) GetCategoryOk() (*string, bool)`

GetCategoryOk returns a tuple with the Category field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCategory

`func (o *ChatActionDefinition) SetCategory(v string)`

SetCategory sets Category field to given value.

### HasCategory

`func (o *ChatActionDefinition) HasCategory() bool`

HasCategory returns a boolean if a field has been set.

### GetInputType

`func (o *ChatActionDefinition) GetInputType() string`

GetInputType returns the InputType field if non-nil, zero value otherwise.

### GetInputTypeOk

`func (o *ChatActionDefinition) GetInputTypeOk() (*string, bool)`

GetInputTypeOk returns a tuple with the InputType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInputType

`func (o *ChatActionDefinition) SetInputType(v string)`

SetInputType sets InputType field to given value.

### HasInputType

`func (o *ChatActionDefinition) HasInputType() bool`

HasInputType returns a boolean if a field has been set.

### GetOutputType

`func (o *ChatActionDefinition) GetOutputType() string`

GetOutputType returns the OutputType field if non-nil, zero value otherwise.

### GetOutputTypeOk

`func (o *ChatActionDefinition) GetOutputTypeOk() (*string, bool)`

GetOutputTypeOk returns a tuple with the OutputType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOutputType

`func (o *ChatActionDefinition) SetOutputType(v string)`

SetOutputType sets OutputType field to given value.

### HasOutputType

`func (o *ChatActionDefinition) HasOutputType() bool`

HasOutputType returns a boolean if a field has been set.

### GetScopes

`func (o *ChatActionDefinition) GetScopes() []string`

GetScopes returns the Scopes field if non-nil, zero value otherwise.

### GetScopesOk

`func (o *ChatActionDefinition) GetScopesOk() (*[]string, bool)`

GetScopesOk returns a tuple with the Scopes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScopes

`func (o *ChatActionDefinition) SetScopes(v []string)`

SetScopes sets Scopes field to given value.

### HasScopes

`func (o *ChatActionDefinition) HasScopes() bool`

HasScopes returns a boolean if a field has been set.

### SetScopesNil

`func (o *ChatActionDefinition) SetScopesNil(b bool)`

 SetScopesNil sets the value for Scopes to be an explicit nil

### UnsetScopes
`func (o *ChatActionDefinition) UnsetScopes()`

UnsetScopes ensures that no value is present for Scopes, not even an explicit nil
### GetMetadata

`func (o *ChatActionDefinition) GetMetadata() map[string]interface{}`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *ChatActionDefinition) GetMetadataOk() (*map[string]interface{}, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *ChatActionDefinition) SetMetadata(v map[string]interface{})`

SetMetadata sets Metadata field to given value.

### HasMetadata

`func (o *ChatActionDefinition) HasMetadata() bool`

HasMetadata returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


