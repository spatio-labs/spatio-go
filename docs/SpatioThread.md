# SpatioThread

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Messages** | [**[]Email**](Email.md) |  | 
**Snippet** | Pointer to **string** |  | [optional] 
**Labels** | Pointer to **[]string** |  | [optional] 

## Methods

### NewSpatioThread

`func NewSpatioThread(id string, messages []Email, ) *SpatioThread`

NewSpatioThread instantiates a new SpatioThread object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSpatioThreadWithDefaults

`func NewSpatioThreadWithDefaults() *SpatioThread`

NewSpatioThreadWithDefaults instantiates a new SpatioThread object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *SpatioThread) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *SpatioThread) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *SpatioThread) SetId(v string)`

SetId sets Id field to given value.


### GetMessages

`func (o *SpatioThread) GetMessages() []Email`

GetMessages returns the Messages field if non-nil, zero value otherwise.

### GetMessagesOk

`func (o *SpatioThread) GetMessagesOk() (*[]Email, bool)`

GetMessagesOk returns a tuple with the Messages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessages

`func (o *SpatioThread) SetMessages(v []Email)`

SetMessages sets Messages field to given value.


### GetSnippet

`func (o *SpatioThread) GetSnippet() string`

GetSnippet returns the Snippet field if non-nil, zero value otherwise.

### GetSnippetOk

`func (o *SpatioThread) GetSnippetOk() (*string, bool)`

GetSnippetOk returns a tuple with the Snippet field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSnippet

`func (o *SpatioThread) SetSnippet(v string)`

SetSnippet sets Snippet field to given value.

### HasSnippet

`func (o *SpatioThread) HasSnippet() bool`

HasSnippet returns a boolean if a field has been set.

### GetLabels

`func (o *SpatioThread) GetLabels() []string`

GetLabels returns the Labels field if non-nil, zero value otherwise.

### GetLabelsOk

`func (o *SpatioThread) GetLabelsOk() (*[]string, bool)`

GetLabelsOk returns a tuple with the Labels field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabels

`func (o *SpatioThread) SetLabels(v []string)`

SetLabels sets Labels field to given value.

### HasLabels

`func (o *SpatioThread) HasLabels() bool`

HasLabels returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


