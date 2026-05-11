# SessionListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Sessions** | [**[]Session**](Session.md) |  | 

## Methods

### NewSessionListResponse

`func NewSessionListResponse(sessions []Session, ) *SessionListResponse`

NewSessionListResponse instantiates a new SessionListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSessionListResponseWithDefaults

`func NewSessionListResponseWithDefaults() *SessionListResponse`

NewSessionListResponseWithDefaults instantiates a new SessionListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSessions

`func (o *SessionListResponse) GetSessions() []Session`

GetSessions returns the Sessions field if non-nil, zero value otherwise.

### GetSessionsOk

`func (o *SessionListResponse) GetSessionsOk() (*[]Session, bool)`

GetSessionsOk returns a tuple with the Sessions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSessions

`func (o *SessionListResponse) SetSessions(v []Session)`

SetSessions sets Sessions field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


