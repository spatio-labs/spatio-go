# FilesAndFoldersResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Files** | Pointer to [**[]SpatioFile**](SpatioFile.md) |  | [optional] 
**Folders** | Pointer to [**[]Folder**](Folder.md) |  | [optional] 
**Accounts** | Pointer to [**[]AccountStatus**](AccountStatus.md) |  | [optional] 
**Total** | **int32** |  | 
**HasMore** | **bool** |  | 
**NextOffset** | Pointer to **int32** |  | [optional] 

## Methods

### NewFilesAndFoldersResponse

`func NewFilesAndFoldersResponse(total int32, hasMore bool, ) *FilesAndFoldersResponse`

NewFilesAndFoldersResponse instantiates a new FilesAndFoldersResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewFilesAndFoldersResponseWithDefaults

`func NewFilesAndFoldersResponseWithDefaults() *FilesAndFoldersResponse`

NewFilesAndFoldersResponseWithDefaults instantiates a new FilesAndFoldersResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFiles

`func (o *FilesAndFoldersResponse) GetFiles() []SpatioFile`

GetFiles returns the Files field if non-nil, zero value otherwise.

### GetFilesOk

`func (o *FilesAndFoldersResponse) GetFilesOk() (*[]SpatioFile, bool)`

GetFilesOk returns a tuple with the Files field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFiles

`func (o *FilesAndFoldersResponse) SetFiles(v []SpatioFile)`

SetFiles sets Files field to given value.

### HasFiles

`func (o *FilesAndFoldersResponse) HasFiles() bool`

HasFiles returns a boolean if a field has been set.

### SetFilesNil

`func (o *FilesAndFoldersResponse) SetFilesNil(b bool)`

 SetFilesNil sets the value for Files to be an explicit nil

### UnsetFiles
`func (o *FilesAndFoldersResponse) UnsetFiles()`

UnsetFiles ensures that no value is present for Files, not even an explicit nil
### GetFolders

`func (o *FilesAndFoldersResponse) GetFolders() []Folder`

GetFolders returns the Folders field if non-nil, zero value otherwise.

### GetFoldersOk

`func (o *FilesAndFoldersResponse) GetFoldersOk() (*[]Folder, bool)`

GetFoldersOk returns a tuple with the Folders field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFolders

`func (o *FilesAndFoldersResponse) SetFolders(v []Folder)`

SetFolders sets Folders field to given value.

### HasFolders

`func (o *FilesAndFoldersResponse) HasFolders() bool`

HasFolders returns a boolean if a field has been set.

### SetFoldersNil

`func (o *FilesAndFoldersResponse) SetFoldersNil(b bool)`

 SetFoldersNil sets the value for Folders to be an explicit nil

### UnsetFolders
`func (o *FilesAndFoldersResponse) UnsetFolders()`

UnsetFolders ensures that no value is present for Folders, not even an explicit nil
### GetAccounts

`func (o *FilesAndFoldersResponse) GetAccounts() []AccountStatus`

GetAccounts returns the Accounts field if non-nil, zero value otherwise.

### GetAccountsOk

`func (o *FilesAndFoldersResponse) GetAccountsOk() (*[]AccountStatus, bool)`

GetAccountsOk returns a tuple with the Accounts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccounts

`func (o *FilesAndFoldersResponse) SetAccounts(v []AccountStatus)`

SetAccounts sets Accounts field to given value.

### HasAccounts

`func (o *FilesAndFoldersResponse) HasAccounts() bool`

HasAccounts returns a boolean if a field has been set.

### GetTotal

`func (o *FilesAndFoldersResponse) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *FilesAndFoldersResponse) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *FilesAndFoldersResponse) SetTotal(v int32)`

SetTotal sets Total field to given value.


### GetHasMore

`func (o *FilesAndFoldersResponse) GetHasMore() bool`

GetHasMore returns the HasMore field if non-nil, zero value otherwise.

### GetHasMoreOk

`func (o *FilesAndFoldersResponse) GetHasMoreOk() (*bool, bool)`

GetHasMoreOk returns a tuple with the HasMore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasMore

`func (o *FilesAndFoldersResponse) SetHasMore(v bool)`

SetHasMore sets HasMore field to given value.


### GetNextOffset

`func (o *FilesAndFoldersResponse) GetNextOffset() int32`

GetNextOffset returns the NextOffset field if non-nil, zero value otherwise.

### GetNextOffsetOk

`func (o *FilesAndFoldersResponse) GetNextOffsetOk() (*int32, bool)`

GetNextOffsetOk returns a tuple with the NextOffset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextOffset

`func (o *FilesAndFoldersResponse) SetNextOffset(v int32)`

SetNextOffset sets NextOffset field to given value.

### HasNextOffset

`func (o *FilesAndFoldersResponse) HasNextOffset() bool`

HasNextOffset returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


