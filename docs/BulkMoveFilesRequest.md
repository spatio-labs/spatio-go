# BulkMoveFilesRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**FileIds** | Pointer to **[]string** |  | [optional] 
**AccountIds** | Pointer to **[]string** |  | [optional] 
**AccountId** | Pointer to **string** |  | [optional] 
**TargetFolderId** | Pointer to **NullableString** |  | [optional] 
**FolderId** | Pointer to **NullableString** | Alias for &#x60;targetFolderId&#x60;. | [optional] 

## Methods

### NewBulkMoveFilesRequest

`func NewBulkMoveFilesRequest() *BulkMoveFilesRequest`

NewBulkMoveFilesRequest instantiates a new BulkMoveFilesRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBulkMoveFilesRequestWithDefaults

`func NewBulkMoveFilesRequestWithDefaults() *BulkMoveFilesRequest`

NewBulkMoveFilesRequestWithDefaults instantiates a new BulkMoveFilesRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFileIds

`func (o *BulkMoveFilesRequest) GetFileIds() []string`

GetFileIds returns the FileIds field if non-nil, zero value otherwise.

### GetFileIdsOk

`func (o *BulkMoveFilesRequest) GetFileIdsOk() (*[]string, bool)`

GetFileIdsOk returns a tuple with the FileIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileIds

`func (o *BulkMoveFilesRequest) SetFileIds(v []string)`

SetFileIds sets FileIds field to given value.

### HasFileIds

`func (o *BulkMoveFilesRequest) HasFileIds() bool`

HasFileIds returns a boolean if a field has been set.

### GetAccountIds

`func (o *BulkMoveFilesRequest) GetAccountIds() []string`

GetAccountIds returns the AccountIds field if non-nil, zero value otherwise.

### GetAccountIdsOk

`func (o *BulkMoveFilesRequest) GetAccountIdsOk() (*[]string, bool)`

GetAccountIdsOk returns a tuple with the AccountIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountIds

`func (o *BulkMoveFilesRequest) SetAccountIds(v []string)`

SetAccountIds sets AccountIds field to given value.

### HasAccountIds

`func (o *BulkMoveFilesRequest) HasAccountIds() bool`

HasAccountIds returns a boolean if a field has been set.

### GetAccountId

`func (o *BulkMoveFilesRequest) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *BulkMoveFilesRequest) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *BulkMoveFilesRequest) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *BulkMoveFilesRequest) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.

### GetTargetFolderId

`func (o *BulkMoveFilesRequest) GetTargetFolderId() string`

GetTargetFolderId returns the TargetFolderId field if non-nil, zero value otherwise.

### GetTargetFolderIdOk

`func (o *BulkMoveFilesRequest) GetTargetFolderIdOk() (*string, bool)`

GetTargetFolderIdOk returns a tuple with the TargetFolderId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTargetFolderId

`func (o *BulkMoveFilesRequest) SetTargetFolderId(v string)`

SetTargetFolderId sets TargetFolderId field to given value.

### HasTargetFolderId

`func (o *BulkMoveFilesRequest) HasTargetFolderId() bool`

HasTargetFolderId returns a boolean if a field has been set.

### SetTargetFolderIdNil

`func (o *BulkMoveFilesRequest) SetTargetFolderIdNil(b bool)`

 SetTargetFolderIdNil sets the value for TargetFolderId to be an explicit nil

### UnsetTargetFolderId
`func (o *BulkMoveFilesRequest) UnsetTargetFolderId()`

UnsetTargetFolderId ensures that no value is present for TargetFolderId, not even an explicit nil
### GetFolderId

`func (o *BulkMoveFilesRequest) GetFolderId() string`

GetFolderId returns the FolderId field if non-nil, zero value otherwise.

### GetFolderIdOk

`func (o *BulkMoveFilesRequest) GetFolderIdOk() (*string, bool)`

GetFolderIdOk returns a tuple with the FolderId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFolderId

`func (o *BulkMoveFilesRequest) SetFolderId(v string)`

SetFolderId sets FolderId field to given value.

### HasFolderId

`func (o *BulkMoveFilesRequest) HasFolderId() bool`

HasFolderId returns a boolean if a field has been set.

### SetFolderIdNil

`func (o *BulkMoveFilesRequest) SetFolderIdNil(b bool)`

 SetFolderIdNil sets the value for FolderId to be an explicit nil

### UnsetFolderId
`func (o *BulkMoveFilesRequest) UnsetFolderId()`

UnsetFolderId ensures that no value is present for FolderId, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


