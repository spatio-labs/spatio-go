# ConferenceData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | **string** |  | 
**Uri** | **string** |  | 
**MeetingId** | Pointer to **string** |  | [optional] 
**Passcode** | Pointer to **string** |  | [optional] 
**AccessCode** | Pointer to **string** |  | [optional] 
**DialIn** | Pointer to **[]string** |  | [optional] 

## Methods

### NewConferenceData

`func NewConferenceData(type_ string, uri string, ) *ConferenceData`

NewConferenceData instantiates a new ConferenceData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewConferenceDataWithDefaults

`func NewConferenceDataWithDefaults() *ConferenceData`

NewConferenceDataWithDefaults instantiates a new ConferenceData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *ConferenceData) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ConferenceData) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ConferenceData) SetType(v string)`

SetType sets Type field to given value.


### GetUri

`func (o *ConferenceData) GetUri() string`

GetUri returns the Uri field if non-nil, zero value otherwise.

### GetUriOk

`func (o *ConferenceData) GetUriOk() (*string, bool)`

GetUriOk returns a tuple with the Uri field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUri

`func (o *ConferenceData) SetUri(v string)`

SetUri sets Uri field to given value.


### GetMeetingId

`func (o *ConferenceData) GetMeetingId() string`

GetMeetingId returns the MeetingId field if non-nil, zero value otherwise.

### GetMeetingIdOk

`func (o *ConferenceData) GetMeetingIdOk() (*string, bool)`

GetMeetingIdOk returns a tuple with the MeetingId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMeetingId

`func (o *ConferenceData) SetMeetingId(v string)`

SetMeetingId sets MeetingId field to given value.

### HasMeetingId

`func (o *ConferenceData) HasMeetingId() bool`

HasMeetingId returns a boolean if a field has been set.

### GetPasscode

`func (o *ConferenceData) GetPasscode() string`

GetPasscode returns the Passcode field if non-nil, zero value otherwise.

### GetPasscodeOk

`func (o *ConferenceData) GetPasscodeOk() (*string, bool)`

GetPasscodeOk returns a tuple with the Passcode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPasscode

`func (o *ConferenceData) SetPasscode(v string)`

SetPasscode sets Passcode field to given value.

### HasPasscode

`func (o *ConferenceData) HasPasscode() bool`

HasPasscode returns a boolean if a field has been set.

### GetAccessCode

`func (o *ConferenceData) GetAccessCode() string`

GetAccessCode returns the AccessCode field if non-nil, zero value otherwise.

### GetAccessCodeOk

`func (o *ConferenceData) GetAccessCodeOk() (*string, bool)`

GetAccessCodeOk returns a tuple with the AccessCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessCode

`func (o *ConferenceData) SetAccessCode(v string)`

SetAccessCode sets AccessCode field to given value.

### HasAccessCode

`func (o *ConferenceData) HasAccessCode() bool`

HasAccessCode returns a boolean if a field has been set.

### GetDialIn

`func (o *ConferenceData) GetDialIn() []string`

GetDialIn returns the DialIn field if non-nil, zero value otherwise.

### GetDialInOk

`func (o *ConferenceData) GetDialInOk() (*[]string, bool)`

GetDialInOk returns a tuple with the DialIn field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDialIn

`func (o *ConferenceData) SetDialIn(v []string)`

SetDialIn sets DialIn field to given value.

### HasDialIn

`func (o *ConferenceData) HasDialIn() bool`

HasDialIn returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


