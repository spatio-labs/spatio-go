# CommitChunkedUploadResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | **bool** |  | 
**FileId** | **string** |  | 
**ManifestId** | **string** |  | 
**Version** | **int32** |  | 
**TotalSize** | **int64** |  | 
**PhysicalSize** | Pointer to **int64** |  | [optional] 
**DeduplicationPct** | Pointer to **float64** |  | [optional] 
**TotalBlocks** | Pointer to **int32** |  | [optional] 
**NewBlocks** | Pointer to **int32** |  | [optional] 
**DeduplicatedBlocks** | Pointer to **int32** |  | [optional] 

## Methods

### NewCommitChunkedUploadResponse

`func NewCommitChunkedUploadResponse(success bool, fileId string, manifestId string, version int32, totalSize int64, ) *CommitChunkedUploadResponse`

NewCommitChunkedUploadResponse instantiates a new CommitChunkedUploadResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCommitChunkedUploadResponseWithDefaults

`func NewCommitChunkedUploadResponseWithDefaults() *CommitChunkedUploadResponse`

NewCommitChunkedUploadResponseWithDefaults instantiates a new CommitChunkedUploadResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *CommitChunkedUploadResponse) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *CommitChunkedUploadResponse) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *CommitChunkedUploadResponse) SetSuccess(v bool)`

SetSuccess sets Success field to given value.


### GetFileId

`func (o *CommitChunkedUploadResponse) GetFileId() string`

GetFileId returns the FileId field if non-nil, zero value otherwise.

### GetFileIdOk

`func (o *CommitChunkedUploadResponse) GetFileIdOk() (*string, bool)`

GetFileIdOk returns a tuple with the FileId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileId

`func (o *CommitChunkedUploadResponse) SetFileId(v string)`

SetFileId sets FileId field to given value.


### GetManifestId

`func (o *CommitChunkedUploadResponse) GetManifestId() string`

GetManifestId returns the ManifestId field if non-nil, zero value otherwise.

### GetManifestIdOk

`func (o *CommitChunkedUploadResponse) GetManifestIdOk() (*string, bool)`

GetManifestIdOk returns a tuple with the ManifestId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetManifestId

`func (o *CommitChunkedUploadResponse) SetManifestId(v string)`

SetManifestId sets ManifestId field to given value.


### GetVersion

`func (o *CommitChunkedUploadResponse) GetVersion() int32`

GetVersion returns the Version field if non-nil, zero value otherwise.

### GetVersionOk

`func (o *CommitChunkedUploadResponse) GetVersionOk() (*int32, bool)`

GetVersionOk returns a tuple with the Version field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersion

`func (o *CommitChunkedUploadResponse) SetVersion(v int32)`

SetVersion sets Version field to given value.


### GetTotalSize

`func (o *CommitChunkedUploadResponse) GetTotalSize() int64`

GetTotalSize returns the TotalSize field if non-nil, zero value otherwise.

### GetTotalSizeOk

`func (o *CommitChunkedUploadResponse) GetTotalSizeOk() (*int64, bool)`

GetTotalSizeOk returns a tuple with the TotalSize field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalSize

`func (o *CommitChunkedUploadResponse) SetTotalSize(v int64)`

SetTotalSize sets TotalSize field to given value.


### GetPhysicalSize

`func (o *CommitChunkedUploadResponse) GetPhysicalSize() int64`

GetPhysicalSize returns the PhysicalSize field if non-nil, zero value otherwise.

### GetPhysicalSizeOk

`func (o *CommitChunkedUploadResponse) GetPhysicalSizeOk() (*int64, bool)`

GetPhysicalSizeOk returns a tuple with the PhysicalSize field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPhysicalSize

`func (o *CommitChunkedUploadResponse) SetPhysicalSize(v int64)`

SetPhysicalSize sets PhysicalSize field to given value.

### HasPhysicalSize

`func (o *CommitChunkedUploadResponse) HasPhysicalSize() bool`

HasPhysicalSize returns a boolean if a field has been set.

### GetDeduplicationPct

`func (o *CommitChunkedUploadResponse) GetDeduplicationPct() float64`

GetDeduplicationPct returns the DeduplicationPct field if non-nil, zero value otherwise.

### GetDeduplicationPctOk

`func (o *CommitChunkedUploadResponse) GetDeduplicationPctOk() (*float64, bool)`

GetDeduplicationPctOk returns a tuple with the DeduplicationPct field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeduplicationPct

`func (o *CommitChunkedUploadResponse) SetDeduplicationPct(v float64)`

SetDeduplicationPct sets DeduplicationPct field to given value.

### HasDeduplicationPct

`func (o *CommitChunkedUploadResponse) HasDeduplicationPct() bool`

HasDeduplicationPct returns a boolean if a field has been set.

### GetTotalBlocks

`func (o *CommitChunkedUploadResponse) GetTotalBlocks() int32`

GetTotalBlocks returns the TotalBlocks field if non-nil, zero value otherwise.

### GetTotalBlocksOk

`func (o *CommitChunkedUploadResponse) GetTotalBlocksOk() (*int32, bool)`

GetTotalBlocksOk returns a tuple with the TotalBlocks field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalBlocks

`func (o *CommitChunkedUploadResponse) SetTotalBlocks(v int32)`

SetTotalBlocks sets TotalBlocks field to given value.

### HasTotalBlocks

`func (o *CommitChunkedUploadResponse) HasTotalBlocks() bool`

HasTotalBlocks returns a boolean if a field has been set.

### GetNewBlocks

`func (o *CommitChunkedUploadResponse) GetNewBlocks() int32`

GetNewBlocks returns the NewBlocks field if non-nil, zero value otherwise.

### GetNewBlocksOk

`func (o *CommitChunkedUploadResponse) GetNewBlocksOk() (*int32, bool)`

GetNewBlocksOk returns a tuple with the NewBlocks field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNewBlocks

`func (o *CommitChunkedUploadResponse) SetNewBlocks(v int32)`

SetNewBlocks sets NewBlocks field to given value.

### HasNewBlocks

`func (o *CommitChunkedUploadResponse) HasNewBlocks() bool`

HasNewBlocks returns a boolean if a field has been set.

### GetDeduplicatedBlocks

`func (o *CommitChunkedUploadResponse) GetDeduplicatedBlocks() int32`

GetDeduplicatedBlocks returns the DeduplicatedBlocks field if non-nil, zero value otherwise.

### GetDeduplicatedBlocksOk

`func (o *CommitChunkedUploadResponse) GetDeduplicatedBlocksOk() (*int32, bool)`

GetDeduplicatedBlocksOk returns a tuple with the DeduplicatedBlocks field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeduplicatedBlocks

`func (o *CommitChunkedUploadResponse) SetDeduplicatedBlocks(v int32)`

SetDeduplicatedBlocks sets DeduplicatedBlocks field to given value.

### HasDeduplicatedBlocks

`func (o *CommitChunkedUploadResponse) HasDeduplicatedBlocks() bool`

HasDeduplicatedBlocks returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


