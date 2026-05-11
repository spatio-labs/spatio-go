# SpatioFile

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Provider** | Pointer to **string** |  | [optional] 
**AccountId** | Pointer to **string** |  | [optional] 
**Name** | **string** |  | 
**Size** | **int64** | Bytes. | 
**MimeType** | **string** |  | 
**FolderId** | Pointer to **NullableString** |  | [optional] 
**StorageType** | **string** | Backing storage class — &#x60;r2&#x60;, &#x60;gdrive&#x60;, &#x60;dropbox&#x60;, etc. Provider-specific; treat as opaque.  | 
**DownloadUrl** | Pointer to **string** | Pre-signed download URL when one is cached on the row. Use &#x60;GET /v1/files/{id}/download&#x60; for a guaranteed-fresh URL — this field can lag past expiry.  | [optional] 
**Metadata** | Pointer to **map[string]interface{}** |  | [optional] 
**CreatedAt** | **time.Time** |  | 
**UpdatedAt** | **time.Time** |  | 

## Methods

### NewSpatioFile

`func NewSpatioFile(id string, name string, size int64, mimeType string, storageType string, createdAt time.Time, updatedAt time.Time, ) *SpatioFile`

NewSpatioFile instantiates a new SpatioFile object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSpatioFileWithDefaults

`func NewSpatioFileWithDefaults() *SpatioFile`

NewSpatioFileWithDefaults instantiates a new SpatioFile object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *SpatioFile) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *SpatioFile) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *SpatioFile) SetId(v string)`

SetId sets Id field to given value.


### GetProvider

`func (o *SpatioFile) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *SpatioFile) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *SpatioFile) SetProvider(v string)`

SetProvider sets Provider field to given value.

### HasProvider

`func (o *SpatioFile) HasProvider() bool`

HasProvider returns a boolean if a field has been set.

### GetAccountId

`func (o *SpatioFile) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *SpatioFile) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *SpatioFile) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *SpatioFile) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.

### GetName

`func (o *SpatioFile) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *SpatioFile) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *SpatioFile) SetName(v string)`

SetName sets Name field to given value.


### GetSize

`func (o *SpatioFile) GetSize() int64`

GetSize returns the Size field if non-nil, zero value otherwise.

### GetSizeOk

`func (o *SpatioFile) GetSizeOk() (*int64, bool)`

GetSizeOk returns a tuple with the Size field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSize

`func (o *SpatioFile) SetSize(v int64)`

SetSize sets Size field to given value.


### GetMimeType

`func (o *SpatioFile) GetMimeType() string`

GetMimeType returns the MimeType field if non-nil, zero value otherwise.

### GetMimeTypeOk

`func (o *SpatioFile) GetMimeTypeOk() (*string, bool)`

GetMimeTypeOk returns a tuple with the MimeType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMimeType

`func (o *SpatioFile) SetMimeType(v string)`

SetMimeType sets MimeType field to given value.


### GetFolderId

`func (o *SpatioFile) GetFolderId() string`

GetFolderId returns the FolderId field if non-nil, zero value otherwise.

### GetFolderIdOk

`func (o *SpatioFile) GetFolderIdOk() (*string, bool)`

GetFolderIdOk returns a tuple with the FolderId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFolderId

`func (o *SpatioFile) SetFolderId(v string)`

SetFolderId sets FolderId field to given value.

### HasFolderId

`func (o *SpatioFile) HasFolderId() bool`

HasFolderId returns a boolean if a field has been set.

### SetFolderIdNil

`func (o *SpatioFile) SetFolderIdNil(b bool)`

 SetFolderIdNil sets the value for FolderId to be an explicit nil

### UnsetFolderId
`func (o *SpatioFile) UnsetFolderId()`

UnsetFolderId ensures that no value is present for FolderId, not even an explicit nil
### GetStorageType

`func (o *SpatioFile) GetStorageType() string`

GetStorageType returns the StorageType field if non-nil, zero value otherwise.

### GetStorageTypeOk

`func (o *SpatioFile) GetStorageTypeOk() (*string, bool)`

GetStorageTypeOk returns a tuple with the StorageType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStorageType

`func (o *SpatioFile) SetStorageType(v string)`

SetStorageType sets StorageType field to given value.


### GetDownloadUrl

`func (o *SpatioFile) GetDownloadUrl() string`

GetDownloadUrl returns the DownloadUrl field if non-nil, zero value otherwise.

### GetDownloadUrlOk

`func (o *SpatioFile) GetDownloadUrlOk() (*string, bool)`

GetDownloadUrlOk returns a tuple with the DownloadUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDownloadUrl

`func (o *SpatioFile) SetDownloadUrl(v string)`

SetDownloadUrl sets DownloadUrl field to given value.

### HasDownloadUrl

`func (o *SpatioFile) HasDownloadUrl() bool`

HasDownloadUrl returns a boolean if a field has been set.

### GetMetadata

`func (o *SpatioFile) GetMetadata() map[string]interface{}`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *SpatioFile) GetMetadataOk() (*map[string]interface{}, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *SpatioFile) SetMetadata(v map[string]interface{})`

SetMetadata sets Metadata field to given value.

### HasMetadata

`func (o *SpatioFile) HasMetadata() bool`

HasMetadata returns a boolean if a field has been set.

### GetCreatedAt

`func (o *SpatioFile) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *SpatioFile) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *SpatioFile) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *SpatioFile) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *SpatioFile) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *SpatioFile) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


