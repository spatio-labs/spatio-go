# AttachmentInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Filename** | **string** |  | 
**ContentType** | **string** |  | 
**Data** | **string** | Base64-encoded bytes. | 
**Size** | Pointer to **int64** |  | [optional] 

## Methods

### NewAttachmentInput

`func NewAttachmentInput(filename string, contentType string, data string, ) *AttachmentInput`

NewAttachmentInput instantiates a new AttachmentInput object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAttachmentInputWithDefaults

`func NewAttachmentInputWithDefaults() *AttachmentInput`

NewAttachmentInputWithDefaults instantiates a new AttachmentInput object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFilename

`func (o *AttachmentInput) GetFilename() string`

GetFilename returns the Filename field if non-nil, zero value otherwise.

### GetFilenameOk

`func (o *AttachmentInput) GetFilenameOk() (*string, bool)`

GetFilenameOk returns a tuple with the Filename field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilename

`func (o *AttachmentInput) SetFilename(v string)`

SetFilename sets Filename field to given value.


### GetContentType

`func (o *AttachmentInput) GetContentType() string`

GetContentType returns the ContentType field if non-nil, zero value otherwise.

### GetContentTypeOk

`func (o *AttachmentInput) GetContentTypeOk() (*string, bool)`

GetContentTypeOk returns a tuple with the ContentType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContentType

`func (o *AttachmentInput) SetContentType(v string)`

SetContentType sets ContentType field to given value.


### GetData

`func (o *AttachmentInput) GetData() string`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *AttachmentInput) GetDataOk() (*string, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *AttachmentInput) SetData(v string)`

SetData sets Data field to given value.


### GetSize

`func (o *AttachmentInput) GetSize() int64`

GetSize returns the Size field if non-nil, zero value otherwise.

### GetSizeOk

`func (o *AttachmentInput) GetSizeOk() (*int64, bool)`

GetSizeOk returns a tuple with the Size field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSize

`func (o *AttachmentInput) SetSize(v int64)`

SetSize sets Size field to given value.

### HasSize

`func (o *AttachmentInput) HasSize() bool`

HasSize returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


