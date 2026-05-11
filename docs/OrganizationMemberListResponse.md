# OrganizationMemberListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Members** | [**[]OrganizationMember**](OrganizationMember.md) |  | 
**Total** | **int32** |  | 

## Methods

### NewOrganizationMemberListResponse

`func NewOrganizationMemberListResponse(members []OrganizationMember, total int32, ) *OrganizationMemberListResponse`

NewOrganizationMemberListResponse instantiates a new OrganizationMemberListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewOrganizationMemberListResponseWithDefaults

`func NewOrganizationMemberListResponseWithDefaults() *OrganizationMemberListResponse`

NewOrganizationMemberListResponseWithDefaults instantiates a new OrganizationMemberListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMembers

`func (o *OrganizationMemberListResponse) GetMembers() []OrganizationMember`

GetMembers returns the Members field if non-nil, zero value otherwise.

### GetMembersOk

`func (o *OrganizationMemberListResponse) GetMembersOk() (*[]OrganizationMember, bool)`

GetMembersOk returns a tuple with the Members field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMembers

`func (o *OrganizationMemberListResponse) SetMembers(v []OrganizationMember)`

SetMembers sets Members field to given value.


### GetTotal

`func (o *OrganizationMemberListResponse) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *OrganizationMemberListResponse) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *OrganizationMemberListResponse) SetTotal(v int32)`

SetTotal sets Total field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


