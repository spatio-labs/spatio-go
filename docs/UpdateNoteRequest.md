# UpdateNoteRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Title** | Pointer to **string** |  | [optional] 
**Content** | Pointer to **string** |  | [optional] 
**Icon** | Pointer to **string** |  | [optional] 
**CoverImage** | Pointer to **string** |  | [optional] 
**ParentId** | Pointer to **NullableString** |  | [optional] 
**Properties** | Pointer to **map[string]interface{}** |  | [optional] 
**Archived** | Pointer to **bool** |  | [optional] 

## Methods

### NewUpdateNoteRequest

`func NewUpdateNoteRequest() *UpdateNoteRequest`

NewUpdateNoteRequest instantiates a new UpdateNoteRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateNoteRequestWithDefaults

`func NewUpdateNoteRequestWithDefaults() *UpdateNoteRequest`

NewUpdateNoteRequestWithDefaults instantiates a new UpdateNoteRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTitle

`func (o *UpdateNoteRequest) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *UpdateNoteRequest) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *UpdateNoteRequest) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *UpdateNoteRequest) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### GetContent

`func (o *UpdateNoteRequest) GetContent() string`

GetContent returns the Content field if non-nil, zero value otherwise.

### GetContentOk

`func (o *UpdateNoteRequest) GetContentOk() (*string, bool)`

GetContentOk returns a tuple with the Content field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContent

`func (o *UpdateNoteRequest) SetContent(v string)`

SetContent sets Content field to given value.

### HasContent

`func (o *UpdateNoteRequest) HasContent() bool`

HasContent returns a boolean if a field has been set.

### GetIcon

`func (o *UpdateNoteRequest) GetIcon() string`

GetIcon returns the Icon field if non-nil, zero value otherwise.

### GetIconOk

`func (o *UpdateNoteRequest) GetIconOk() (*string, bool)`

GetIconOk returns a tuple with the Icon field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIcon

`func (o *UpdateNoteRequest) SetIcon(v string)`

SetIcon sets Icon field to given value.

### HasIcon

`func (o *UpdateNoteRequest) HasIcon() bool`

HasIcon returns a boolean if a field has been set.

### GetCoverImage

`func (o *UpdateNoteRequest) GetCoverImage() string`

GetCoverImage returns the CoverImage field if non-nil, zero value otherwise.

### GetCoverImageOk

`func (o *UpdateNoteRequest) GetCoverImageOk() (*string, bool)`

GetCoverImageOk returns a tuple with the CoverImage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCoverImage

`func (o *UpdateNoteRequest) SetCoverImage(v string)`

SetCoverImage sets CoverImage field to given value.

### HasCoverImage

`func (o *UpdateNoteRequest) HasCoverImage() bool`

HasCoverImage returns a boolean if a field has been set.

### GetParentId

`func (o *UpdateNoteRequest) GetParentId() string`

GetParentId returns the ParentId field if non-nil, zero value otherwise.

### GetParentIdOk

`func (o *UpdateNoteRequest) GetParentIdOk() (*string, bool)`

GetParentIdOk returns a tuple with the ParentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetParentId

`func (o *UpdateNoteRequest) SetParentId(v string)`

SetParentId sets ParentId field to given value.

### HasParentId

`func (o *UpdateNoteRequest) HasParentId() bool`

HasParentId returns a boolean if a field has been set.

### SetParentIdNil

`func (o *UpdateNoteRequest) SetParentIdNil(b bool)`

 SetParentIdNil sets the value for ParentId to be an explicit nil

### UnsetParentId
`func (o *UpdateNoteRequest) UnsetParentId()`

UnsetParentId ensures that no value is present for ParentId, not even an explicit nil
### GetProperties

`func (o *UpdateNoteRequest) GetProperties() map[string]interface{}`

GetProperties returns the Properties field if non-nil, zero value otherwise.

### GetPropertiesOk

`func (o *UpdateNoteRequest) GetPropertiesOk() (*map[string]interface{}, bool)`

GetPropertiesOk returns a tuple with the Properties field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProperties

`func (o *UpdateNoteRequest) SetProperties(v map[string]interface{})`

SetProperties sets Properties field to given value.

### HasProperties

`func (o *UpdateNoteRequest) HasProperties() bool`

HasProperties returns a boolean if a field has been set.

### GetArchived

`func (o *UpdateNoteRequest) GetArchived() bool`

GetArchived returns the Archived field if non-nil, zero value otherwise.

### GetArchivedOk

`func (o *UpdateNoteRequest) GetArchivedOk() (*bool, bool)`

GetArchivedOk returns a tuple with the Archived field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArchived

`func (o *UpdateNoteRequest) SetArchived(v bool)`

SetArchived sets Archived field to given value.

### HasArchived

`func (o *UpdateNoteRequest) HasArchived() bool`

HasArchived returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


