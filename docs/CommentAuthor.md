# CommentAuthor

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Name** | **string** |  | 
**Email** | **string** |  | 
**ProfilePhoto** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewCommentAuthor

`func NewCommentAuthor(id string, name string, email string, ) *CommentAuthor`

NewCommentAuthor instantiates a new CommentAuthor object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCommentAuthorWithDefaults

`func NewCommentAuthorWithDefaults() *CommentAuthor`

NewCommentAuthorWithDefaults instantiates a new CommentAuthor object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *CommentAuthor) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *CommentAuthor) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *CommentAuthor) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *CommentAuthor) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CommentAuthor) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CommentAuthor) SetName(v string)`

SetName sets Name field to given value.


### GetEmail

`func (o *CommentAuthor) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *CommentAuthor) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *CommentAuthor) SetEmail(v string)`

SetEmail sets Email field to given value.


### GetProfilePhoto

`func (o *CommentAuthor) GetProfilePhoto() string`

GetProfilePhoto returns the ProfilePhoto field if non-nil, zero value otherwise.

### GetProfilePhotoOk

`func (o *CommentAuthor) GetProfilePhotoOk() (*string, bool)`

GetProfilePhotoOk returns a tuple with the ProfilePhoto field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProfilePhoto

`func (o *CommentAuthor) SetProfilePhoto(v string)`

SetProfilePhoto sets ProfilePhoto field to given value.

### HasProfilePhoto

`func (o *CommentAuthor) HasProfilePhoto() bool`

HasProfilePhoto returns a boolean if a field has been set.

### SetProfilePhotoNil

`func (o *CommentAuthor) SetProfilePhotoNil(b bool)`

 SetProfilePhotoNil sets the value for ProfilePhoto to be an explicit nil

### UnsetProfilePhoto
`func (o *CommentAuthor) UnsetProfilePhoto()`

UnsetProfilePhoto ensures that no value is present for ProfilePhoto, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


