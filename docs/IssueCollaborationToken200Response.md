# IssueCollaborationToken200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Token** | **string** | HS256 JWT, signed with the shared platform/worker secret. | 
**WsUrl** | **string** | Base WebSocket URL of the Yjs worker. | 
**Room** | Pointer to **string** |  | [optional] 
**ExpiresAt** | **time.Time** |  | 
**ExpiresIn** | **int32** | Seconds until the token expires. | 

## Methods

### NewIssueCollaborationToken200Response

`func NewIssueCollaborationToken200Response(token string, wsUrl string, expiresAt time.Time, expiresIn int32, ) *IssueCollaborationToken200Response`

NewIssueCollaborationToken200Response instantiates a new IssueCollaborationToken200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewIssueCollaborationToken200ResponseWithDefaults

`func NewIssueCollaborationToken200ResponseWithDefaults() *IssueCollaborationToken200Response`

NewIssueCollaborationToken200ResponseWithDefaults instantiates a new IssueCollaborationToken200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetToken

`func (o *IssueCollaborationToken200Response) GetToken() string`

GetToken returns the Token field if non-nil, zero value otherwise.

### GetTokenOk

`func (o *IssueCollaborationToken200Response) GetTokenOk() (*string, bool)`

GetTokenOk returns a tuple with the Token field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetToken

`func (o *IssueCollaborationToken200Response) SetToken(v string)`

SetToken sets Token field to given value.


### GetWsUrl

`func (o *IssueCollaborationToken200Response) GetWsUrl() string`

GetWsUrl returns the WsUrl field if non-nil, zero value otherwise.

### GetWsUrlOk

`func (o *IssueCollaborationToken200Response) GetWsUrlOk() (*string, bool)`

GetWsUrlOk returns a tuple with the WsUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWsUrl

`func (o *IssueCollaborationToken200Response) SetWsUrl(v string)`

SetWsUrl sets WsUrl field to given value.


### GetRoom

`func (o *IssueCollaborationToken200Response) GetRoom() string`

GetRoom returns the Room field if non-nil, zero value otherwise.

### GetRoomOk

`func (o *IssueCollaborationToken200Response) GetRoomOk() (*string, bool)`

GetRoomOk returns a tuple with the Room field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRoom

`func (o *IssueCollaborationToken200Response) SetRoom(v string)`

SetRoom sets Room field to given value.

### HasRoom

`func (o *IssueCollaborationToken200Response) HasRoom() bool`

HasRoom returns a boolean if a field has been set.

### GetExpiresAt

`func (o *IssueCollaborationToken200Response) GetExpiresAt() time.Time`

GetExpiresAt returns the ExpiresAt field if non-nil, zero value otherwise.

### GetExpiresAtOk

`func (o *IssueCollaborationToken200Response) GetExpiresAtOk() (*time.Time, bool)`

GetExpiresAtOk returns a tuple with the ExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresAt

`func (o *IssueCollaborationToken200Response) SetExpiresAt(v time.Time)`

SetExpiresAt sets ExpiresAt field to given value.


### GetExpiresIn

`func (o *IssueCollaborationToken200Response) GetExpiresIn() int32`

GetExpiresIn returns the ExpiresIn field if non-nil, zero value otherwise.

### GetExpiresInOk

`func (o *IssueCollaborationToken200Response) GetExpiresInOk() (*int32, bool)`

GetExpiresInOk returns a tuple with the ExpiresIn field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresIn

`func (o *IssueCollaborationToken200Response) SetExpiresIn(v int32)`

SetExpiresIn sets ExpiresIn field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


