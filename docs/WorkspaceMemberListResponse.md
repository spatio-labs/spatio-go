# WorkspaceMemberListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Members** | [**[]WorkspaceMember**](WorkspaceMember.md) |  | 
**Total** | Pointer to **int32** |  | [optional] 

## Methods

### NewWorkspaceMemberListResponse

`func NewWorkspaceMemberListResponse(members []WorkspaceMember, ) *WorkspaceMemberListResponse`

NewWorkspaceMemberListResponse instantiates a new WorkspaceMemberListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWorkspaceMemberListResponseWithDefaults

`func NewWorkspaceMemberListResponseWithDefaults() *WorkspaceMemberListResponse`

NewWorkspaceMemberListResponseWithDefaults instantiates a new WorkspaceMemberListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMembers

`func (o *WorkspaceMemberListResponse) GetMembers() []WorkspaceMember`

GetMembers returns the Members field if non-nil, zero value otherwise.

### GetMembersOk

`func (o *WorkspaceMemberListResponse) GetMembersOk() (*[]WorkspaceMember, bool)`

GetMembersOk returns a tuple with the Members field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMembers

`func (o *WorkspaceMemberListResponse) SetMembers(v []WorkspaceMember)`

SetMembers sets Members field to given value.


### GetTotal

`func (o *WorkspaceMemberListResponse) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *WorkspaceMemberListResponse) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *WorkspaceMemberListResponse) SetTotal(v int32)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *WorkspaceMemberListResponse) HasTotal() bool`

HasTotal returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


