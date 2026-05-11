# Block

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**NoteId** | **string** |  | 
**ParentId** | Pointer to **NullableString** |  | [optional] 
**Type** | [**BlockType**](BlockType.md) |  | 
**Content** | [**BlockContent**](BlockContent.md) |  | 
**Properties** | Pointer to **map[string]interface{}** |  | [optional] 
**Position** | **int32** | Order within the parent (0-indexed). | 
**HasChildren** | **bool** |  | 
**CreatedAt** | **time.Time** |  | 
**UpdatedAt** | **time.Time** |  | 

## Methods

### NewBlock

`func NewBlock(id string, noteId string, type_ BlockType, content BlockContent, position int32, hasChildren bool, createdAt time.Time, updatedAt time.Time, ) *Block`

NewBlock instantiates a new Block object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBlockWithDefaults

`func NewBlockWithDefaults() *Block`

NewBlockWithDefaults instantiates a new Block object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Block) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Block) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Block) SetId(v string)`

SetId sets Id field to given value.


### GetNoteId

`func (o *Block) GetNoteId() string`

GetNoteId returns the NoteId field if non-nil, zero value otherwise.

### GetNoteIdOk

`func (o *Block) GetNoteIdOk() (*string, bool)`

GetNoteIdOk returns a tuple with the NoteId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNoteId

`func (o *Block) SetNoteId(v string)`

SetNoteId sets NoteId field to given value.


### GetParentId

`func (o *Block) GetParentId() string`

GetParentId returns the ParentId field if non-nil, zero value otherwise.

### GetParentIdOk

`func (o *Block) GetParentIdOk() (*string, bool)`

GetParentIdOk returns a tuple with the ParentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetParentId

`func (o *Block) SetParentId(v string)`

SetParentId sets ParentId field to given value.

### HasParentId

`func (o *Block) HasParentId() bool`

HasParentId returns a boolean if a field has been set.

### SetParentIdNil

`func (o *Block) SetParentIdNil(b bool)`

 SetParentIdNil sets the value for ParentId to be an explicit nil

### UnsetParentId
`func (o *Block) UnsetParentId()`

UnsetParentId ensures that no value is present for ParentId, not even an explicit nil
### GetType

`func (o *Block) GetType() BlockType`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *Block) GetTypeOk() (*BlockType, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *Block) SetType(v BlockType)`

SetType sets Type field to given value.


### GetContent

`func (o *Block) GetContent() BlockContent`

GetContent returns the Content field if non-nil, zero value otherwise.

### GetContentOk

`func (o *Block) GetContentOk() (*BlockContent, bool)`

GetContentOk returns a tuple with the Content field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContent

`func (o *Block) SetContent(v BlockContent)`

SetContent sets Content field to given value.


### GetProperties

`func (o *Block) GetProperties() map[string]interface{}`

GetProperties returns the Properties field if non-nil, zero value otherwise.

### GetPropertiesOk

`func (o *Block) GetPropertiesOk() (*map[string]interface{}, bool)`

GetPropertiesOk returns a tuple with the Properties field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProperties

`func (o *Block) SetProperties(v map[string]interface{})`

SetProperties sets Properties field to given value.

### HasProperties

`func (o *Block) HasProperties() bool`

HasProperties returns a boolean if a field has been set.

### GetPosition

`func (o *Block) GetPosition() int32`

GetPosition returns the Position field if non-nil, zero value otherwise.

### GetPositionOk

`func (o *Block) GetPositionOk() (*int32, bool)`

GetPositionOk returns a tuple with the Position field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPosition

`func (o *Block) SetPosition(v int32)`

SetPosition sets Position field to given value.


### GetHasChildren

`func (o *Block) GetHasChildren() bool`

GetHasChildren returns the HasChildren field if non-nil, zero value otherwise.

### GetHasChildrenOk

`func (o *Block) GetHasChildrenOk() (*bool, bool)`

GetHasChildrenOk returns a tuple with the HasChildren field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasChildren

`func (o *Block) SetHasChildren(v bool)`

SetHasChildren sets HasChildren field to given value.


### GetCreatedAt

`func (o *Block) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Block) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Block) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *Block) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *Block) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *Block) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


