# WorkspaceListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Workspaces** | [**[]Workspace**](Workspace.md) |  | 
**Total** | Pointer to **int32** |  | [optional] 

## Methods

### NewWorkspaceListResponse

`func NewWorkspaceListResponse(workspaces []Workspace, ) *WorkspaceListResponse`

NewWorkspaceListResponse instantiates a new WorkspaceListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWorkspaceListResponseWithDefaults

`func NewWorkspaceListResponseWithDefaults() *WorkspaceListResponse`

NewWorkspaceListResponseWithDefaults instantiates a new WorkspaceListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetWorkspaces

`func (o *WorkspaceListResponse) GetWorkspaces() []Workspace`

GetWorkspaces returns the Workspaces field if non-nil, zero value otherwise.

### GetWorkspacesOk

`func (o *WorkspaceListResponse) GetWorkspacesOk() (*[]Workspace, bool)`

GetWorkspacesOk returns a tuple with the Workspaces field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWorkspaces

`func (o *WorkspaceListResponse) SetWorkspaces(v []Workspace)`

SetWorkspaces sets Workspaces field to given value.


### GetTotal

`func (o *WorkspaceListResponse) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *WorkspaceListResponse) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *WorkspaceListResponse) SetTotal(v int32)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *WorkspaceListResponse) HasTotal() bool`

HasTotal returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


