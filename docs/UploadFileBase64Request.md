# UploadFileBase64Request

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AccountId** | Pointer to **string** |  | [optional] 
**Name** | **string** |  | 
**Content** | **string** | Base64-encoded file bytes. | 
**MimeType** | **string** |  | 
**FolderId** | Pointer to **NullableString** |  | [optional] 
**WorkspaceId** | Pointer to **string** |  | [optional] 
**OrganizationId** | Pointer to **string** |  | [optional] 
**Metadata** | Pointer to **map[string]interface{}** |  | [optional] 

## Methods

### NewUploadFileBase64Request

`func NewUploadFileBase64Request(name string, content string, mimeType string, ) *UploadFileBase64Request`

NewUploadFileBase64Request instantiates a new UploadFileBase64Request object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUploadFileBase64RequestWithDefaults

`func NewUploadFileBase64RequestWithDefaults() *UploadFileBase64Request`

NewUploadFileBase64RequestWithDefaults instantiates a new UploadFileBase64Request object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAccountId

`func (o *UploadFileBase64Request) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *UploadFileBase64Request) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *UploadFileBase64Request) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *UploadFileBase64Request) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.

### GetName

`func (o *UploadFileBase64Request) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *UploadFileBase64Request) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *UploadFileBase64Request) SetName(v string)`

SetName sets Name field to given value.


### GetContent

`func (o *UploadFileBase64Request) GetContent() string`

GetContent returns the Content field if non-nil, zero value otherwise.

### GetContentOk

`func (o *UploadFileBase64Request) GetContentOk() (*string, bool)`

GetContentOk returns a tuple with the Content field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContent

`func (o *UploadFileBase64Request) SetContent(v string)`

SetContent sets Content field to given value.


### GetMimeType

`func (o *UploadFileBase64Request) GetMimeType() string`

GetMimeType returns the MimeType field if non-nil, zero value otherwise.

### GetMimeTypeOk

`func (o *UploadFileBase64Request) GetMimeTypeOk() (*string, bool)`

GetMimeTypeOk returns a tuple with the MimeType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMimeType

`func (o *UploadFileBase64Request) SetMimeType(v string)`

SetMimeType sets MimeType field to given value.


### GetFolderId

`func (o *UploadFileBase64Request) GetFolderId() string`

GetFolderId returns the FolderId field if non-nil, zero value otherwise.

### GetFolderIdOk

`func (o *UploadFileBase64Request) GetFolderIdOk() (*string, bool)`

GetFolderIdOk returns a tuple with the FolderId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFolderId

`func (o *UploadFileBase64Request) SetFolderId(v string)`

SetFolderId sets FolderId field to given value.

### HasFolderId

`func (o *UploadFileBase64Request) HasFolderId() bool`

HasFolderId returns a boolean if a field has been set.

### SetFolderIdNil

`func (o *UploadFileBase64Request) SetFolderIdNil(b bool)`

 SetFolderIdNil sets the value for FolderId to be an explicit nil

### UnsetFolderId
`func (o *UploadFileBase64Request) UnsetFolderId()`

UnsetFolderId ensures that no value is present for FolderId, not even an explicit nil
### GetWorkspaceId

`func (o *UploadFileBase64Request) GetWorkspaceId() string`

GetWorkspaceId returns the WorkspaceId field if non-nil, zero value otherwise.

### GetWorkspaceIdOk

`func (o *UploadFileBase64Request) GetWorkspaceIdOk() (*string, bool)`

GetWorkspaceIdOk returns a tuple with the WorkspaceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWorkspaceId

`func (o *UploadFileBase64Request) SetWorkspaceId(v string)`

SetWorkspaceId sets WorkspaceId field to given value.

### HasWorkspaceId

`func (o *UploadFileBase64Request) HasWorkspaceId() bool`

HasWorkspaceId returns a boolean if a field has been set.

### GetOrganizationId

`func (o *UploadFileBase64Request) GetOrganizationId() string`

GetOrganizationId returns the OrganizationId field if non-nil, zero value otherwise.

### GetOrganizationIdOk

`func (o *UploadFileBase64Request) GetOrganizationIdOk() (*string, bool)`

GetOrganizationIdOk returns a tuple with the OrganizationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrganizationId

`func (o *UploadFileBase64Request) SetOrganizationId(v string)`

SetOrganizationId sets OrganizationId field to given value.

### HasOrganizationId

`func (o *UploadFileBase64Request) HasOrganizationId() bool`

HasOrganizationId returns a boolean if a field has been set.

### GetMetadata

`func (o *UploadFileBase64Request) GetMetadata() map[string]interface{}`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *UploadFileBase64Request) GetMetadataOk() (*map[string]interface{}, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *UploadFileBase64Request) SetMetadata(v map[string]interface{})`

SetMetadata sets Metadata field to given value.

### HasMetadata

`func (o *UploadFileBase64Request) HasMetadata() bool`

HasMetadata returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


