# ChunkedFileManifest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ManifestId** | **string** |  | 
**FileId** | **string** |  | 
**FileName** | **string** |  | 
**Version** | **int32** |  | 
**TotalSize** | **int64** |  | 
**BlockCount** | **int32** |  | 
**ChunkingAlgorithm** | Pointer to **string** |  | [optional] 
**FileChecksum** | Pointer to **string** |  | [optional] 
**Blocks** | Pointer to **[]map[string]interface{}** |  | [optional] 

## Methods

### NewChunkedFileManifest

`func NewChunkedFileManifest(manifestId string, fileId string, fileName string, version int32, totalSize int64, blockCount int32, ) *ChunkedFileManifest`

NewChunkedFileManifest instantiates a new ChunkedFileManifest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewChunkedFileManifestWithDefaults

`func NewChunkedFileManifestWithDefaults() *ChunkedFileManifest`

NewChunkedFileManifestWithDefaults instantiates a new ChunkedFileManifest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetManifestId

`func (o *ChunkedFileManifest) GetManifestId() string`

GetManifestId returns the ManifestId field if non-nil, zero value otherwise.

### GetManifestIdOk

`func (o *ChunkedFileManifest) GetManifestIdOk() (*string, bool)`

GetManifestIdOk returns a tuple with the ManifestId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetManifestId

`func (o *ChunkedFileManifest) SetManifestId(v string)`

SetManifestId sets ManifestId field to given value.


### GetFileId

`func (o *ChunkedFileManifest) GetFileId() string`

GetFileId returns the FileId field if non-nil, zero value otherwise.

### GetFileIdOk

`func (o *ChunkedFileManifest) GetFileIdOk() (*string, bool)`

GetFileIdOk returns a tuple with the FileId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileId

`func (o *ChunkedFileManifest) SetFileId(v string)`

SetFileId sets FileId field to given value.


### GetFileName

`func (o *ChunkedFileManifest) GetFileName() string`

GetFileName returns the FileName field if non-nil, zero value otherwise.

### GetFileNameOk

`func (o *ChunkedFileManifest) GetFileNameOk() (*string, bool)`

GetFileNameOk returns a tuple with the FileName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileName

`func (o *ChunkedFileManifest) SetFileName(v string)`

SetFileName sets FileName field to given value.


### GetVersion

`func (o *ChunkedFileManifest) GetVersion() int32`

GetVersion returns the Version field if non-nil, zero value otherwise.

### GetVersionOk

`func (o *ChunkedFileManifest) GetVersionOk() (*int32, bool)`

GetVersionOk returns a tuple with the Version field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersion

`func (o *ChunkedFileManifest) SetVersion(v int32)`

SetVersion sets Version field to given value.


### GetTotalSize

`func (o *ChunkedFileManifest) GetTotalSize() int64`

GetTotalSize returns the TotalSize field if non-nil, zero value otherwise.

### GetTotalSizeOk

`func (o *ChunkedFileManifest) GetTotalSizeOk() (*int64, bool)`

GetTotalSizeOk returns a tuple with the TotalSize field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalSize

`func (o *ChunkedFileManifest) SetTotalSize(v int64)`

SetTotalSize sets TotalSize field to given value.


### GetBlockCount

`func (o *ChunkedFileManifest) GetBlockCount() int32`

GetBlockCount returns the BlockCount field if non-nil, zero value otherwise.

### GetBlockCountOk

`func (o *ChunkedFileManifest) GetBlockCountOk() (*int32, bool)`

GetBlockCountOk returns a tuple with the BlockCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBlockCount

`func (o *ChunkedFileManifest) SetBlockCount(v int32)`

SetBlockCount sets BlockCount field to given value.


### GetChunkingAlgorithm

`func (o *ChunkedFileManifest) GetChunkingAlgorithm() string`

GetChunkingAlgorithm returns the ChunkingAlgorithm field if non-nil, zero value otherwise.

### GetChunkingAlgorithmOk

`func (o *ChunkedFileManifest) GetChunkingAlgorithmOk() (*string, bool)`

GetChunkingAlgorithmOk returns a tuple with the ChunkingAlgorithm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChunkingAlgorithm

`func (o *ChunkedFileManifest) SetChunkingAlgorithm(v string)`

SetChunkingAlgorithm sets ChunkingAlgorithm field to given value.

### HasChunkingAlgorithm

`func (o *ChunkedFileManifest) HasChunkingAlgorithm() bool`

HasChunkingAlgorithm returns a boolean if a field has been set.

### GetFileChecksum

`func (o *ChunkedFileManifest) GetFileChecksum() string`

GetFileChecksum returns the FileChecksum field if non-nil, zero value otherwise.

### GetFileChecksumOk

`func (o *ChunkedFileManifest) GetFileChecksumOk() (*string, bool)`

GetFileChecksumOk returns a tuple with the FileChecksum field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileChecksum

`func (o *ChunkedFileManifest) SetFileChecksum(v string)`

SetFileChecksum sets FileChecksum field to given value.

### HasFileChecksum

`func (o *ChunkedFileManifest) HasFileChecksum() bool`

HasFileChecksum returns a boolean if a field has been set.

### GetBlocks

`func (o *ChunkedFileManifest) GetBlocks() []map[string]interface{}`

GetBlocks returns the Blocks field if non-nil, zero value otherwise.

### GetBlocksOk

`func (o *ChunkedFileManifest) GetBlocksOk() (*[]map[string]interface{}, bool)`

GetBlocksOk returns a tuple with the Blocks field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBlocks

`func (o *ChunkedFileManifest) SetBlocks(v []map[string]interface{})`

SetBlocks sets Blocks field to given value.

### HasBlocks

`func (o *ChunkedFileManifest) HasBlocks() bool`

HasBlocks returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


