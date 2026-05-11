# DMAttachRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Kind** | **string** | Attachment kind (&#x60;image&#x60;, &#x60;file&#x60;, &#x60;audio&#x60;, &#x60;video&#x60;, etc.). | 
**Url** | **string** |  | 
**Filename** | Pointer to **string** |  | [optional] 
**SizeBytes** | Pointer to **int64** |  | [optional] 
**MimeType** | Pointer to **string** |  | [optional] 
**ThumbnailUrl** | Pointer to **string** |  | [optional] 
**Width** | Pointer to **int32** |  | [optional] 
**Height** | Pointer to **int32** |  | [optional] 
**AccountId** | Pointer to **string** |  | [optional] 

## Methods

### NewDMAttachRequest

`func NewDMAttachRequest(kind string, url string, ) *DMAttachRequest`

NewDMAttachRequest instantiates a new DMAttachRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDMAttachRequestWithDefaults

`func NewDMAttachRequestWithDefaults() *DMAttachRequest`

NewDMAttachRequestWithDefaults instantiates a new DMAttachRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetKind

`func (o *DMAttachRequest) GetKind() string`

GetKind returns the Kind field if non-nil, zero value otherwise.

### GetKindOk

`func (o *DMAttachRequest) GetKindOk() (*string, bool)`

GetKindOk returns a tuple with the Kind field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKind

`func (o *DMAttachRequest) SetKind(v string)`

SetKind sets Kind field to given value.


### GetUrl

`func (o *DMAttachRequest) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *DMAttachRequest) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *DMAttachRequest) SetUrl(v string)`

SetUrl sets Url field to given value.


### GetFilename

`func (o *DMAttachRequest) GetFilename() string`

GetFilename returns the Filename field if non-nil, zero value otherwise.

### GetFilenameOk

`func (o *DMAttachRequest) GetFilenameOk() (*string, bool)`

GetFilenameOk returns a tuple with the Filename field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilename

`func (o *DMAttachRequest) SetFilename(v string)`

SetFilename sets Filename field to given value.

### HasFilename

`func (o *DMAttachRequest) HasFilename() bool`

HasFilename returns a boolean if a field has been set.

### GetSizeBytes

`func (o *DMAttachRequest) GetSizeBytes() int64`

GetSizeBytes returns the SizeBytes field if non-nil, zero value otherwise.

### GetSizeBytesOk

`func (o *DMAttachRequest) GetSizeBytesOk() (*int64, bool)`

GetSizeBytesOk returns a tuple with the SizeBytes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSizeBytes

`func (o *DMAttachRequest) SetSizeBytes(v int64)`

SetSizeBytes sets SizeBytes field to given value.

### HasSizeBytes

`func (o *DMAttachRequest) HasSizeBytes() bool`

HasSizeBytes returns a boolean if a field has been set.

### GetMimeType

`func (o *DMAttachRequest) GetMimeType() string`

GetMimeType returns the MimeType field if non-nil, zero value otherwise.

### GetMimeTypeOk

`func (o *DMAttachRequest) GetMimeTypeOk() (*string, bool)`

GetMimeTypeOk returns a tuple with the MimeType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMimeType

`func (o *DMAttachRequest) SetMimeType(v string)`

SetMimeType sets MimeType field to given value.

### HasMimeType

`func (o *DMAttachRequest) HasMimeType() bool`

HasMimeType returns a boolean if a field has been set.

### GetThumbnailUrl

`func (o *DMAttachRequest) GetThumbnailUrl() string`

GetThumbnailUrl returns the ThumbnailUrl field if non-nil, zero value otherwise.

### GetThumbnailUrlOk

`func (o *DMAttachRequest) GetThumbnailUrlOk() (*string, bool)`

GetThumbnailUrlOk returns a tuple with the ThumbnailUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetThumbnailUrl

`func (o *DMAttachRequest) SetThumbnailUrl(v string)`

SetThumbnailUrl sets ThumbnailUrl field to given value.

### HasThumbnailUrl

`func (o *DMAttachRequest) HasThumbnailUrl() bool`

HasThumbnailUrl returns a boolean if a field has been set.

### GetWidth

`func (o *DMAttachRequest) GetWidth() int32`

GetWidth returns the Width field if non-nil, zero value otherwise.

### GetWidthOk

`func (o *DMAttachRequest) GetWidthOk() (*int32, bool)`

GetWidthOk returns a tuple with the Width field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWidth

`func (o *DMAttachRequest) SetWidth(v int32)`

SetWidth sets Width field to given value.

### HasWidth

`func (o *DMAttachRequest) HasWidth() bool`

HasWidth returns a boolean if a field has been set.

### GetHeight

`func (o *DMAttachRequest) GetHeight() int32`

GetHeight returns the Height field if non-nil, zero value otherwise.

### GetHeightOk

`func (o *DMAttachRequest) GetHeightOk() (*int32, bool)`

GetHeightOk returns a tuple with the Height field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHeight

`func (o *DMAttachRequest) SetHeight(v int32)`

SetHeight sets Height field to given value.

### HasHeight

`func (o *DMAttachRequest) HasHeight() bool`

HasHeight returns a boolean if a field has been set.

### GetAccountId

`func (o *DMAttachRequest) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *DMAttachRequest) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *DMAttachRequest) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *DMAttachRequest) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


