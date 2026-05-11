# BulkDeleteFilesRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**FileIds** | Pointer to **[]string** |  | [optional] 
**AccountIds** | Pointer to **[]string** | Parallel slice with fileIds — accountIds[i] targets fileIds[i]. | [optional] 
**FileId** | Pointer to **string** |  | [optional] 
**AccountId** | Pointer to **string** |  | [optional] 

## Methods

### NewBulkDeleteFilesRequest

`func NewBulkDeleteFilesRequest() *BulkDeleteFilesRequest`

NewBulkDeleteFilesRequest instantiates a new BulkDeleteFilesRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBulkDeleteFilesRequestWithDefaults

`func NewBulkDeleteFilesRequestWithDefaults() *BulkDeleteFilesRequest`

NewBulkDeleteFilesRequestWithDefaults instantiates a new BulkDeleteFilesRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFileIds

`func (o *BulkDeleteFilesRequest) GetFileIds() []string`

GetFileIds returns the FileIds field if non-nil, zero value otherwise.

### GetFileIdsOk

`func (o *BulkDeleteFilesRequest) GetFileIdsOk() (*[]string, bool)`

GetFileIdsOk returns a tuple with the FileIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileIds

`func (o *BulkDeleteFilesRequest) SetFileIds(v []string)`

SetFileIds sets FileIds field to given value.

### HasFileIds

`func (o *BulkDeleteFilesRequest) HasFileIds() bool`

HasFileIds returns a boolean if a field has been set.

### GetAccountIds

`func (o *BulkDeleteFilesRequest) GetAccountIds() []string`

GetAccountIds returns the AccountIds field if non-nil, zero value otherwise.

### GetAccountIdsOk

`func (o *BulkDeleteFilesRequest) GetAccountIdsOk() (*[]string, bool)`

GetAccountIdsOk returns a tuple with the AccountIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountIds

`func (o *BulkDeleteFilesRequest) SetAccountIds(v []string)`

SetAccountIds sets AccountIds field to given value.

### HasAccountIds

`func (o *BulkDeleteFilesRequest) HasAccountIds() bool`

HasAccountIds returns a boolean if a field has been set.

### GetFileId

`func (o *BulkDeleteFilesRequest) GetFileId() string`

GetFileId returns the FileId field if non-nil, zero value otherwise.

### GetFileIdOk

`func (o *BulkDeleteFilesRequest) GetFileIdOk() (*string, bool)`

GetFileIdOk returns a tuple with the FileId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileId

`func (o *BulkDeleteFilesRequest) SetFileId(v string)`

SetFileId sets FileId field to given value.

### HasFileId

`func (o *BulkDeleteFilesRequest) HasFileId() bool`

HasFileId returns a boolean if a field has been set.

### GetAccountId

`func (o *BulkDeleteFilesRequest) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *BulkDeleteFilesRequest) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *BulkDeleteFilesRequest) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *BulkDeleteFilesRequest) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


