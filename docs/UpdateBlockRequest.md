# UpdateBlockRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Content** | Pointer to [**BlockContent**](BlockContent.md) |  | [optional] 
**Properties** | Pointer to **map[string]interface{}** |  | [optional] 
**Archived** | Pointer to **bool** |  | [optional] 

## Methods

### NewUpdateBlockRequest

`func NewUpdateBlockRequest() *UpdateBlockRequest`

NewUpdateBlockRequest instantiates a new UpdateBlockRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateBlockRequestWithDefaults

`func NewUpdateBlockRequestWithDefaults() *UpdateBlockRequest`

NewUpdateBlockRequestWithDefaults instantiates a new UpdateBlockRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetContent

`func (o *UpdateBlockRequest) GetContent() BlockContent`

GetContent returns the Content field if non-nil, zero value otherwise.

### GetContentOk

`func (o *UpdateBlockRequest) GetContentOk() (*BlockContent, bool)`

GetContentOk returns a tuple with the Content field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContent

`func (o *UpdateBlockRequest) SetContent(v BlockContent)`

SetContent sets Content field to given value.

### HasContent

`func (o *UpdateBlockRequest) HasContent() bool`

HasContent returns a boolean if a field has been set.

### GetProperties

`func (o *UpdateBlockRequest) GetProperties() map[string]interface{}`

GetProperties returns the Properties field if non-nil, zero value otherwise.

### GetPropertiesOk

`func (o *UpdateBlockRequest) GetPropertiesOk() (*map[string]interface{}, bool)`

GetPropertiesOk returns a tuple with the Properties field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProperties

`func (o *UpdateBlockRequest) SetProperties(v map[string]interface{})`

SetProperties sets Properties field to given value.

### HasProperties

`func (o *UpdateBlockRequest) HasProperties() bool`

HasProperties returns a boolean if a field has been set.

### GetArchived

`func (o *UpdateBlockRequest) GetArchived() bool`

GetArchived returns the Archived field if non-nil, zero value otherwise.

### GetArchivedOk

`func (o *UpdateBlockRequest) GetArchivedOk() (*bool, bool)`

GetArchivedOk returns a tuple with the Archived field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArchived

`func (o *UpdateBlockRequest) SetArchived(v bool)`

SetArchived sets Archived field to given value.

### HasArchived

`func (o *UpdateBlockRequest) HasArchived() bool`

HasArchived returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


