# InitChunkedUploadRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**FileName** | **string** |  | 
**TotalSize** | **int64** |  | 
**MimeType** | **string** |  | 
**ExpectedBlocks** | **[]string** | Hashes of every block the client intends to upload. | 
**FolderId** | Pointer to **NullableString** |  | [optional] 
**WorkspaceId** | Pointer to **string** |  | [optional] 
**OrganizationId** | Pointer to **string** |  | [optional] 

## Methods

### NewInitChunkedUploadRequest

`func NewInitChunkedUploadRequest(fileName string, totalSize int64, mimeType string, expectedBlocks []string, ) *InitChunkedUploadRequest`

NewInitChunkedUploadRequest instantiates a new InitChunkedUploadRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInitChunkedUploadRequestWithDefaults

`func NewInitChunkedUploadRequestWithDefaults() *InitChunkedUploadRequest`

NewInitChunkedUploadRequestWithDefaults instantiates a new InitChunkedUploadRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFileName

`func (o *InitChunkedUploadRequest) GetFileName() string`

GetFileName returns the FileName field if non-nil, zero value otherwise.

### GetFileNameOk

`func (o *InitChunkedUploadRequest) GetFileNameOk() (*string, bool)`

GetFileNameOk returns a tuple with the FileName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileName

`func (o *InitChunkedUploadRequest) SetFileName(v string)`

SetFileName sets FileName field to given value.


### GetTotalSize

`func (o *InitChunkedUploadRequest) GetTotalSize() int64`

GetTotalSize returns the TotalSize field if non-nil, zero value otherwise.

### GetTotalSizeOk

`func (o *InitChunkedUploadRequest) GetTotalSizeOk() (*int64, bool)`

GetTotalSizeOk returns a tuple with the TotalSize field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalSize

`func (o *InitChunkedUploadRequest) SetTotalSize(v int64)`

SetTotalSize sets TotalSize field to given value.


### GetMimeType

`func (o *InitChunkedUploadRequest) GetMimeType() string`

GetMimeType returns the MimeType field if non-nil, zero value otherwise.

### GetMimeTypeOk

`func (o *InitChunkedUploadRequest) GetMimeTypeOk() (*string, bool)`

GetMimeTypeOk returns a tuple with the MimeType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMimeType

`func (o *InitChunkedUploadRequest) SetMimeType(v string)`

SetMimeType sets MimeType field to given value.


### GetExpectedBlocks

`func (o *InitChunkedUploadRequest) GetExpectedBlocks() []string`

GetExpectedBlocks returns the ExpectedBlocks field if non-nil, zero value otherwise.

### GetExpectedBlocksOk

`func (o *InitChunkedUploadRequest) GetExpectedBlocksOk() (*[]string, bool)`

GetExpectedBlocksOk returns a tuple with the ExpectedBlocks field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpectedBlocks

`func (o *InitChunkedUploadRequest) SetExpectedBlocks(v []string)`

SetExpectedBlocks sets ExpectedBlocks field to given value.


### GetFolderId

`func (o *InitChunkedUploadRequest) GetFolderId() string`

GetFolderId returns the FolderId field if non-nil, zero value otherwise.

### GetFolderIdOk

`func (o *InitChunkedUploadRequest) GetFolderIdOk() (*string, bool)`

GetFolderIdOk returns a tuple with the FolderId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFolderId

`func (o *InitChunkedUploadRequest) SetFolderId(v string)`

SetFolderId sets FolderId field to given value.

### HasFolderId

`func (o *InitChunkedUploadRequest) HasFolderId() bool`

HasFolderId returns a boolean if a field has been set.

### SetFolderIdNil

`func (o *InitChunkedUploadRequest) SetFolderIdNil(b bool)`

 SetFolderIdNil sets the value for FolderId to be an explicit nil

### UnsetFolderId
`func (o *InitChunkedUploadRequest) UnsetFolderId()`

UnsetFolderId ensures that no value is present for FolderId, not even an explicit nil
### GetWorkspaceId

`func (o *InitChunkedUploadRequest) GetWorkspaceId() string`

GetWorkspaceId returns the WorkspaceId field if non-nil, zero value otherwise.

### GetWorkspaceIdOk

`func (o *InitChunkedUploadRequest) GetWorkspaceIdOk() (*string, bool)`

GetWorkspaceIdOk returns a tuple with the WorkspaceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWorkspaceId

`func (o *InitChunkedUploadRequest) SetWorkspaceId(v string)`

SetWorkspaceId sets WorkspaceId field to given value.

### HasWorkspaceId

`func (o *InitChunkedUploadRequest) HasWorkspaceId() bool`

HasWorkspaceId returns a boolean if a field has been set.

### GetOrganizationId

`func (o *InitChunkedUploadRequest) GetOrganizationId() string`

GetOrganizationId returns the OrganizationId field if non-nil, zero value otherwise.

### GetOrganizationIdOk

`func (o *InitChunkedUploadRequest) GetOrganizationIdOk() (*string, bool)`

GetOrganizationIdOk returns a tuple with the OrganizationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrganizationId

`func (o *InitChunkedUploadRequest) SetOrganizationId(v string)`

SetOrganizationId sets OrganizationId field to given value.

### HasOrganizationId

`func (o *InitChunkedUploadRequest) HasOrganizationId() bool`

HasOrganizationId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


