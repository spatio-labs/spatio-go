# IssueCollaborationTokenRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Room** | Pointer to **string** | Optional &#x60;&lt;type&gt;:&lt;id&gt;&#x60; room identifier (e.g. &#x60;note:abc123&#x60;). When set, the JWT only authorizes this single room.  | [optional] 

## Methods

### NewIssueCollaborationTokenRequest

`func NewIssueCollaborationTokenRequest() *IssueCollaborationTokenRequest`

NewIssueCollaborationTokenRequest instantiates a new IssueCollaborationTokenRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewIssueCollaborationTokenRequestWithDefaults

`func NewIssueCollaborationTokenRequestWithDefaults() *IssueCollaborationTokenRequest`

NewIssueCollaborationTokenRequestWithDefaults instantiates a new IssueCollaborationTokenRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRoom

`func (o *IssueCollaborationTokenRequest) GetRoom() string`

GetRoom returns the Room field if non-nil, zero value otherwise.

### GetRoomOk

`func (o *IssueCollaborationTokenRequest) GetRoomOk() (*string, bool)`

GetRoomOk returns a tuple with the Room field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRoom

`func (o *IssueCollaborationTokenRequest) SetRoom(v string)`

SetRoom sets Room field to given value.

### HasRoom

`func (o *IssueCollaborationTokenRequest) HasRoom() bool`

HasRoom returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


