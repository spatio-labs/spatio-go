# Attachment

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** |  | [optional] 
**Title** | **string** |  | 
**MimeType** | Pointer to **string** |  | [optional] 
**Url** | **string** |  | 
**Size** | Pointer to **int64** |  | [optional] 

## Methods

### NewAttachment

`func NewAttachment(title string, url string, ) *Attachment`

NewAttachment instantiates a new Attachment object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAttachmentWithDefaults

`func NewAttachmentWithDefaults() *Attachment`

NewAttachmentWithDefaults instantiates a new Attachment object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Attachment) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Attachment) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Attachment) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *Attachment) HasId() bool`

HasId returns a boolean if a field has been set.

### GetTitle

`func (o *Attachment) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *Attachment) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *Attachment) SetTitle(v string)`

SetTitle sets Title field to given value.


### GetMimeType

`func (o *Attachment) GetMimeType() string`

GetMimeType returns the MimeType field if non-nil, zero value otherwise.

### GetMimeTypeOk

`func (o *Attachment) GetMimeTypeOk() (*string, bool)`

GetMimeTypeOk returns a tuple with the MimeType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMimeType

`func (o *Attachment) SetMimeType(v string)`

SetMimeType sets MimeType field to given value.

### HasMimeType

`func (o *Attachment) HasMimeType() bool`

HasMimeType returns a boolean if a field has been set.

### GetUrl

`func (o *Attachment) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *Attachment) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *Attachment) SetUrl(v string)`

SetUrl sets Url field to given value.


### GetSize

`func (o *Attachment) GetSize() int64`

GetSize returns the Size field if non-nil, zero value otherwise.

### GetSizeOk

`func (o *Attachment) GetSizeOk() (*int64, bool)`

GetSizeOk returns a tuple with the Size field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSize

`func (o *Attachment) SetSize(v int64)`

SetSize sets Size field to given value.

### HasSize

`func (o *Attachment) HasSize() bool`

HasSize returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


