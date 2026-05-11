# CreateBlockRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | [**BlockType**](BlockType.md) |  | 
**Content** | [**BlockContent**](BlockContent.md) |  | 
**ParentId** | Pointer to **NullableString** | Parent block id for nested blocks. | [optional] 
**Position** | **int32** |  | 
**Properties** | Pointer to **map[string]interface{}** |  | [optional] 

## Methods

### NewCreateBlockRequest

`func NewCreateBlockRequest(type_ BlockType, content BlockContent, position int32, ) *CreateBlockRequest`

NewCreateBlockRequest instantiates a new CreateBlockRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateBlockRequestWithDefaults

`func NewCreateBlockRequestWithDefaults() *CreateBlockRequest`

NewCreateBlockRequestWithDefaults instantiates a new CreateBlockRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *CreateBlockRequest) GetType() BlockType`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *CreateBlockRequest) GetTypeOk() (*BlockType, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *CreateBlockRequest) SetType(v BlockType)`

SetType sets Type field to given value.


### GetContent

`func (o *CreateBlockRequest) GetContent() BlockContent`

GetContent returns the Content field if non-nil, zero value otherwise.

### GetContentOk

`func (o *CreateBlockRequest) GetContentOk() (*BlockContent, bool)`

GetContentOk returns a tuple with the Content field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContent

`func (o *CreateBlockRequest) SetContent(v BlockContent)`

SetContent sets Content field to given value.


### GetParentId

`func (o *CreateBlockRequest) GetParentId() string`

GetParentId returns the ParentId field if non-nil, zero value otherwise.

### GetParentIdOk

`func (o *CreateBlockRequest) GetParentIdOk() (*string, bool)`

GetParentIdOk returns a tuple with the ParentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetParentId

`func (o *CreateBlockRequest) SetParentId(v string)`

SetParentId sets ParentId field to given value.

### HasParentId

`func (o *CreateBlockRequest) HasParentId() bool`

HasParentId returns a boolean if a field has been set.

### SetParentIdNil

`func (o *CreateBlockRequest) SetParentIdNil(b bool)`

 SetParentIdNil sets the value for ParentId to be an explicit nil

### UnsetParentId
`func (o *CreateBlockRequest) UnsetParentId()`

UnsetParentId ensures that no value is present for ParentId, not even an explicit nil
### GetPosition

`func (o *CreateBlockRequest) GetPosition() int32`

GetPosition returns the Position field if non-nil, zero value otherwise.

### GetPositionOk

`func (o *CreateBlockRequest) GetPositionOk() (*int32, bool)`

GetPositionOk returns a tuple with the Position field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPosition

`func (o *CreateBlockRequest) SetPosition(v int32)`

SetPosition sets Position field to given value.


### GetProperties

`func (o *CreateBlockRequest) GetProperties() map[string]interface{}`

GetProperties returns the Properties field if non-nil, zero value otherwise.

### GetPropertiesOk

`func (o *CreateBlockRequest) GetPropertiesOk() (*map[string]interface{}, bool)`

GetPropertiesOk returns a tuple with the Properties field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProperties

`func (o *CreateBlockRequest) SetProperties(v map[string]interface{})`

SetProperties sets Properties field to given value.

### HasProperties

`func (o *CreateBlockRequest) HasProperties() bool`

HasProperties returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


