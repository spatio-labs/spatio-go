# Comment

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**NoteId** | **string** |  | 
**ParentCommentId** | Pointer to **NullableString** |  | [optional] 
**BlockId** | Pointer to **NullableString** |  | [optional] 
**Body** | **string** |  | 
**CreatedAt** | **time.Time** |  | 
**UpdatedAt** | **time.Time** |  | 
**Author** | [**CommentAuthor**](CommentAuthor.md) |  | 

## Methods

### NewComment

`func NewComment(id string, noteId string, body string, createdAt time.Time, updatedAt time.Time, author CommentAuthor, ) *Comment`

NewComment instantiates a new Comment object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCommentWithDefaults

`func NewCommentWithDefaults() *Comment`

NewCommentWithDefaults instantiates a new Comment object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Comment) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Comment) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Comment) SetId(v string)`

SetId sets Id field to given value.


### GetNoteId

`func (o *Comment) GetNoteId() string`

GetNoteId returns the NoteId field if non-nil, zero value otherwise.

### GetNoteIdOk

`func (o *Comment) GetNoteIdOk() (*string, bool)`

GetNoteIdOk returns a tuple with the NoteId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNoteId

`func (o *Comment) SetNoteId(v string)`

SetNoteId sets NoteId field to given value.


### GetParentCommentId

`func (o *Comment) GetParentCommentId() string`

GetParentCommentId returns the ParentCommentId field if non-nil, zero value otherwise.

### GetParentCommentIdOk

`func (o *Comment) GetParentCommentIdOk() (*string, bool)`

GetParentCommentIdOk returns a tuple with the ParentCommentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetParentCommentId

`func (o *Comment) SetParentCommentId(v string)`

SetParentCommentId sets ParentCommentId field to given value.

### HasParentCommentId

`func (o *Comment) HasParentCommentId() bool`

HasParentCommentId returns a boolean if a field has been set.

### SetParentCommentIdNil

`func (o *Comment) SetParentCommentIdNil(b bool)`

 SetParentCommentIdNil sets the value for ParentCommentId to be an explicit nil

### UnsetParentCommentId
`func (o *Comment) UnsetParentCommentId()`

UnsetParentCommentId ensures that no value is present for ParentCommentId, not even an explicit nil
### GetBlockId

`func (o *Comment) GetBlockId() string`

GetBlockId returns the BlockId field if non-nil, zero value otherwise.

### GetBlockIdOk

`func (o *Comment) GetBlockIdOk() (*string, bool)`

GetBlockIdOk returns a tuple with the BlockId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBlockId

`func (o *Comment) SetBlockId(v string)`

SetBlockId sets BlockId field to given value.

### HasBlockId

`func (o *Comment) HasBlockId() bool`

HasBlockId returns a boolean if a field has been set.

### SetBlockIdNil

`func (o *Comment) SetBlockIdNil(b bool)`

 SetBlockIdNil sets the value for BlockId to be an explicit nil

### UnsetBlockId
`func (o *Comment) UnsetBlockId()`

UnsetBlockId ensures that no value is present for BlockId, not even an explicit nil
### GetBody

`func (o *Comment) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *Comment) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *Comment) SetBody(v string)`

SetBody sets Body field to given value.


### GetCreatedAt

`func (o *Comment) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Comment) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Comment) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *Comment) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *Comment) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *Comment) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.


### GetAuthor

`func (o *Comment) GetAuthor() CommentAuthor`

GetAuthor returns the Author field if non-nil, zero value otherwise.

### GetAuthorOk

`func (o *Comment) GetAuthorOk() (*CommentAuthor, bool)`

GetAuthorOk returns a tuple with the Author field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAuthor

`func (o *Comment) SetAuthor(v CommentAuthor)`

SetAuthor sets Author field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


