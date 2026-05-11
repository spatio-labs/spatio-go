# CreateEventRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AccountId** | **string** |  | 
**CalendarId** | Pointer to **string** | Specific calendar within the account; omit for the default. | [optional] 
**Event** | [**SpatioEvent**](SpatioEvent.md) |  | 
**SendUpdates** | Pointer to **string** | Notification policy passed through to the provider. | [optional] 
**ConferenceType** | Pointer to **string** | When set, the platform will auto-attach a conference link of the matching type (&#x60;spatio&#x60;, &#x60;meet&#x60;, &#x60;zoom&#x60;, &#x60;teams&#x60;).  | [optional] 

## Methods

### NewCreateEventRequest

`func NewCreateEventRequest(accountId string, event SpatioEvent, ) *CreateEventRequest`

NewCreateEventRequest instantiates a new CreateEventRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateEventRequestWithDefaults

`func NewCreateEventRequestWithDefaults() *CreateEventRequest`

NewCreateEventRequestWithDefaults instantiates a new CreateEventRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAccountId

`func (o *CreateEventRequest) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *CreateEventRequest) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *CreateEventRequest) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.


### GetCalendarId

`func (o *CreateEventRequest) GetCalendarId() string`

GetCalendarId returns the CalendarId field if non-nil, zero value otherwise.

### GetCalendarIdOk

`func (o *CreateEventRequest) GetCalendarIdOk() (*string, bool)`

GetCalendarIdOk returns a tuple with the CalendarId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCalendarId

`func (o *CreateEventRequest) SetCalendarId(v string)`

SetCalendarId sets CalendarId field to given value.

### HasCalendarId

`func (o *CreateEventRequest) HasCalendarId() bool`

HasCalendarId returns a boolean if a field has been set.

### GetEvent

`func (o *CreateEventRequest) GetEvent() SpatioEvent`

GetEvent returns the Event field if non-nil, zero value otherwise.

### GetEventOk

`func (o *CreateEventRequest) GetEventOk() (*SpatioEvent, bool)`

GetEventOk returns a tuple with the Event field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEvent

`func (o *CreateEventRequest) SetEvent(v SpatioEvent)`

SetEvent sets Event field to given value.


### GetSendUpdates

`func (o *CreateEventRequest) GetSendUpdates() string`

GetSendUpdates returns the SendUpdates field if non-nil, zero value otherwise.

### GetSendUpdatesOk

`func (o *CreateEventRequest) GetSendUpdatesOk() (*string, bool)`

GetSendUpdatesOk returns a tuple with the SendUpdates field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSendUpdates

`func (o *CreateEventRequest) SetSendUpdates(v string)`

SetSendUpdates sets SendUpdates field to given value.

### HasSendUpdates

`func (o *CreateEventRequest) HasSendUpdates() bool`

HasSendUpdates returns a boolean if a field has been set.

### GetConferenceType

`func (o *CreateEventRequest) GetConferenceType() string`

GetConferenceType returns the ConferenceType field if non-nil, zero value otherwise.

### GetConferenceTypeOk

`func (o *CreateEventRequest) GetConferenceTypeOk() (*string, bool)`

GetConferenceTypeOk returns a tuple with the ConferenceType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConferenceType

`func (o *CreateEventRequest) SetConferenceType(v string)`

SetConferenceType sets ConferenceType field to given value.

### HasConferenceType

`func (o *CreateEventRequest) HasConferenceType() bool`

HasConferenceType returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


