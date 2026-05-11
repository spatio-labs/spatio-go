# EmailFolderListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Folders** | [**[]EmailFolder**](EmailFolder.md) |  | 

## Methods

### NewEmailFolderListResponse

`func NewEmailFolderListResponse(folders []EmailFolder, ) *EmailFolderListResponse`

NewEmailFolderListResponse instantiates a new EmailFolderListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEmailFolderListResponseWithDefaults

`func NewEmailFolderListResponseWithDefaults() *EmailFolderListResponse`

NewEmailFolderListResponseWithDefaults instantiates a new EmailFolderListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFolders

`func (o *EmailFolderListResponse) GetFolders() []EmailFolder`

GetFolders returns the Folders field if non-nil, zero value otherwise.

### GetFoldersOk

`func (o *EmailFolderListResponse) GetFoldersOk() (*[]EmailFolder, bool)`

GetFoldersOk returns a tuple with the Folders field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFolders

`func (o *EmailFolderListResponse) SetFolders(v []EmailFolder)`

SetFolders sets Folders field to given value.


### SetFoldersNil

`func (o *EmailFolderListResponse) SetFoldersNil(b bool)`

 SetFoldersNil sets the value for Folders to be an explicit nil

### UnsetFolders
`func (o *EmailFolderListResponse) UnsetFolders()`

UnsetFolders ensures that no value is present for Folders, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


