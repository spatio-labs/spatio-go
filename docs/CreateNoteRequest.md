# CreateNoteRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Title** | **string** |  | 
**Content** | Pointer to **string** |  | [optional] 
**Icon** | Pointer to **string** |  | [optional] 
**CoverImage** | Pointer to **string** |  | [optional] 
**ParentId** | Pointer to **NullableString** |  | [optional] 
**Properties** | Pointer to **map[string]interface{}** |  | [optional] 
**AccountId** | Pointer to **string** | Optional override for the target connected account. May also be passed as a &#x60;?accountId&#x3D;&#x60; query param.  | [optional] 
**Provider** | Pointer to **string** | Optional provider id (alternative to &#x60;accountId&#x60; when only one account exists for the provider). May also be passed as a &#x60;?provider&#x3D;&#x60; query param.  | [optional] 

## Methods

### NewCreateNoteRequest

`func NewCreateNoteRequest(title string, ) *CreateNoteRequest`

NewCreateNoteRequest instantiates a new CreateNoteRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateNoteRequestWithDefaults

`func NewCreateNoteRequestWithDefaults() *CreateNoteRequest`

NewCreateNoteRequestWithDefaults instantiates a new CreateNoteRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTitle

`func (o *CreateNoteRequest) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *CreateNoteRequest) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *CreateNoteRequest) SetTitle(v string)`

SetTitle sets Title field to given value.


### GetContent

`func (o *CreateNoteRequest) GetContent() string`

GetContent returns the Content field if non-nil, zero value otherwise.

### GetContentOk

`func (o *CreateNoteRequest) GetContentOk() (*string, bool)`

GetContentOk returns a tuple with the Content field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContent

`func (o *CreateNoteRequest) SetContent(v string)`

SetContent sets Content field to given value.

### HasContent

`func (o *CreateNoteRequest) HasContent() bool`

HasContent returns a boolean if a field has been set.

### GetIcon

`func (o *CreateNoteRequest) GetIcon() string`

GetIcon returns the Icon field if non-nil, zero value otherwise.

### GetIconOk

`func (o *CreateNoteRequest) GetIconOk() (*string, bool)`

GetIconOk returns a tuple with the Icon field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIcon

`func (o *CreateNoteRequest) SetIcon(v string)`

SetIcon sets Icon field to given value.

### HasIcon

`func (o *CreateNoteRequest) HasIcon() bool`

HasIcon returns a boolean if a field has been set.

### GetCoverImage

`func (o *CreateNoteRequest) GetCoverImage() string`

GetCoverImage returns the CoverImage field if non-nil, zero value otherwise.

### GetCoverImageOk

`func (o *CreateNoteRequest) GetCoverImageOk() (*string, bool)`

GetCoverImageOk returns a tuple with the CoverImage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCoverImage

`func (o *CreateNoteRequest) SetCoverImage(v string)`

SetCoverImage sets CoverImage field to given value.

### HasCoverImage

`func (o *CreateNoteRequest) HasCoverImage() bool`

HasCoverImage returns a boolean if a field has been set.

### GetParentId

`func (o *CreateNoteRequest) GetParentId() string`

GetParentId returns the ParentId field if non-nil, zero value otherwise.

### GetParentIdOk

`func (o *CreateNoteRequest) GetParentIdOk() (*string, bool)`

GetParentIdOk returns a tuple with the ParentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetParentId

`func (o *CreateNoteRequest) SetParentId(v string)`

SetParentId sets ParentId field to given value.

### HasParentId

`func (o *CreateNoteRequest) HasParentId() bool`

HasParentId returns a boolean if a field has been set.

### SetParentIdNil

`func (o *CreateNoteRequest) SetParentIdNil(b bool)`

 SetParentIdNil sets the value for ParentId to be an explicit nil

### UnsetParentId
`func (o *CreateNoteRequest) UnsetParentId()`

UnsetParentId ensures that no value is present for ParentId, not even an explicit nil
### GetProperties

`func (o *CreateNoteRequest) GetProperties() map[string]interface{}`

GetProperties returns the Properties field if non-nil, zero value otherwise.

### GetPropertiesOk

`func (o *CreateNoteRequest) GetPropertiesOk() (*map[string]interface{}, bool)`

GetPropertiesOk returns a tuple with the Properties field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProperties

`func (o *CreateNoteRequest) SetProperties(v map[string]interface{})`

SetProperties sets Properties field to given value.

### HasProperties

`func (o *CreateNoteRequest) HasProperties() bool`

HasProperties returns a boolean if a field has been set.

### GetAccountId

`func (o *CreateNoteRequest) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *CreateNoteRequest) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *CreateNoteRequest) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *CreateNoteRequest) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.

### GetProvider

`func (o *CreateNoteRequest) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *CreateNoteRequest) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *CreateNoteRequest) SetProvider(v string)`

SetProvider sets Provider field to given value.

### HasProvider

`func (o *CreateNoteRequest) HasProvider() bool`

HasProvider returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


