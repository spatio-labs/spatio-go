# SpatioCall

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Title** | Pointer to **string** |  | [optional] 
**Status** | Pointer to **string** |  | [optional] 
**HostUserId** | Pointer to **string** |  | [optional] 
**WorkspaceId** | Pointer to **string** |  | [optional] 
**RoomId** | Pointer to **string** |  | [optional] 
**Participants** | Pointer to **[]map[string]interface{}** |  | [optional] 
**Metadata** | Pointer to **map[string]interface{}** |  | [optional] 
**StartedAt** | Pointer to **time.Time** |  | [optional] 
**EndedAt** | Pointer to **NullableTime** |  | [optional] 
**CreatedAt** | Pointer to **time.Time** |  | [optional] 

## Methods

### NewSpatioCall

`func NewSpatioCall(id string, ) *SpatioCall`

NewSpatioCall instantiates a new SpatioCall object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSpatioCallWithDefaults

`func NewSpatioCallWithDefaults() *SpatioCall`

NewSpatioCallWithDefaults instantiates a new SpatioCall object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *SpatioCall) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *SpatioCall) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *SpatioCall) SetId(v string)`

SetId sets Id field to given value.


### GetTitle

`func (o *SpatioCall) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *SpatioCall) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *SpatioCall) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *SpatioCall) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### GetStatus

`func (o *SpatioCall) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *SpatioCall) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *SpatioCall) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *SpatioCall) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetHostUserId

`func (o *SpatioCall) GetHostUserId() string`

GetHostUserId returns the HostUserId field if non-nil, zero value otherwise.

### GetHostUserIdOk

`func (o *SpatioCall) GetHostUserIdOk() (*string, bool)`

GetHostUserIdOk returns a tuple with the HostUserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHostUserId

`func (o *SpatioCall) SetHostUserId(v string)`

SetHostUserId sets HostUserId field to given value.

### HasHostUserId

`func (o *SpatioCall) HasHostUserId() bool`

HasHostUserId returns a boolean if a field has been set.

### GetWorkspaceId

`func (o *SpatioCall) GetWorkspaceId() string`

GetWorkspaceId returns the WorkspaceId field if non-nil, zero value otherwise.

### GetWorkspaceIdOk

`func (o *SpatioCall) GetWorkspaceIdOk() (*string, bool)`

GetWorkspaceIdOk returns a tuple with the WorkspaceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWorkspaceId

`func (o *SpatioCall) SetWorkspaceId(v string)`

SetWorkspaceId sets WorkspaceId field to given value.

### HasWorkspaceId

`func (o *SpatioCall) HasWorkspaceId() bool`

HasWorkspaceId returns a boolean if a field has been set.

### GetRoomId

`func (o *SpatioCall) GetRoomId() string`

GetRoomId returns the RoomId field if non-nil, zero value otherwise.

### GetRoomIdOk

`func (o *SpatioCall) GetRoomIdOk() (*string, bool)`

GetRoomIdOk returns a tuple with the RoomId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRoomId

`func (o *SpatioCall) SetRoomId(v string)`

SetRoomId sets RoomId field to given value.

### HasRoomId

`func (o *SpatioCall) HasRoomId() bool`

HasRoomId returns a boolean if a field has been set.

### GetParticipants

`func (o *SpatioCall) GetParticipants() []map[string]interface{}`

GetParticipants returns the Participants field if non-nil, zero value otherwise.

### GetParticipantsOk

`func (o *SpatioCall) GetParticipantsOk() (*[]map[string]interface{}, bool)`

GetParticipantsOk returns a tuple with the Participants field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetParticipants

`func (o *SpatioCall) SetParticipants(v []map[string]interface{})`

SetParticipants sets Participants field to given value.

### HasParticipants

`func (o *SpatioCall) HasParticipants() bool`

HasParticipants returns a boolean if a field has been set.

### GetMetadata

`func (o *SpatioCall) GetMetadata() map[string]interface{}`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *SpatioCall) GetMetadataOk() (*map[string]interface{}, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *SpatioCall) SetMetadata(v map[string]interface{})`

SetMetadata sets Metadata field to given value.

### HasMetadata

`func (o *SpatioCall) HasMetadata() bool`

HasMetadata returns a boolean if a field has been set.

### GetStartedAt

`func (o *SpatioCall) GetStartedAt() time.Time`

GetStartedAt returns the StartedAt field if non-nil, zero value otherwise.

### GetStartedAtOk

`func (o *SpatioCall) GetStartedAtOk() (*time.Time, bool)`

GetStartedAtOk returns a tuple with the StartedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStartedAt

`func (o *SpatioCall) SetStartedAt(v time.Time)`

SetStartedAt sets StartedAt field to given value.

### HasStartedAt

`func (o *SpatioCall) HasStartedAt() bool`

HasStartedAt returns a boolean if a field has been set.

### GetEndedAt

`func (o *SpatioCall) GetEndedAt() time.Time`

GetEndedAt returns the EndedAt field if non-nil, zero value otherwise.

### GetEndedAtOk

`func (o *SpatioCall) GetEndedAtOk() (*time.Time, bool)`

GetEndedAtOk returns a tuple with the EndedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndedAt

`func (o *SpatioCall) SetEndedAt(v time.Time)`

SetEndedAt sets EndedAt field to given value.

### HasEndedAt

`func (o *SpatioCall) HasEndedAt() bool`

HasEndedAt returns a boolean if a field has been set.

### SetEndedAtNil

`func (o *SpatioCall) SetEndedAtNil(b bool)`

 SetEndedAtNil sets the value for EndedAt to be an explicit nil

### UnsetEndedAt
`func (o *SpatioCall) UnsetEndedAt()`

UnsetEndedAt ensures that no value is present for EndedAt, not even an explicit nil
### GetCreatedAt

`func (o *SpatioCall) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *SpatioCall) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *SpatioCall) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *SpatioCall) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


