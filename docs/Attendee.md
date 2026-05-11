# Attendee

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Email** | **string** |  | 
**Name** | Pointer to **string** |  | [optional] 
**Status** | [**AttendeeStatus**](AttendeeStatus.md) |  | 
**Role** | [**AttendeeRole**](AttendeeRole.md) |  | 
**Optional** | **bool** | Legacy boolean — superseded by &#x60;role&#x60; (&#x60;role: optional&#x60; carries the same signal). Kept on the wire for client compatibility.  | 
**Comment** | Pointer to **string** |  | [optional] 
**AdditionalGuests** | Pointer to **int32** |  | [optional] 

## Methods

### NewAttendee

`func NewAttendee(email string, status AttendeeStatus, role AttendeeRole, optional bool, ) *Attendee`

NewAttendee instantiates a new Attendee object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAttendeeWithDefaults

`func NewAttendeeWithDefaults() *Attendee`

NewAttendeeWithDefaults instantiates a new Attendee object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEmail

`func (o *Attendee) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *Attendee) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *Attendee) SetEmail(v string)`

SetEmail sets Email field to given value.


### GetName

`func (o *Attendee) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Attendee) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Attendee) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *Attendee) HasName() bool`

HasName returns a boolean if a field has been set.

### GetStatus

`func (o *Attendee) GetStatus() AttendeeStatus`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *Attendee) GetStatusOk() (*AttendeeStatus, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *Attendee) SetStatus(v AttendeeStatus)`

SetStatus sets Status field to given value.


### GetRole

`func (o *Attendee) GetRole() AttendeeRole`

GetRole returns the Role field if non-nil, zero value otherwise.

### GetRoleOk

`func (o *Attendee) GetRoleOk() (*AttendeeRole, bool)`

GetRoleOk returns a tuple with the Role field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRole

`func (o *Attendee) SetRole(v AttendeeRole)`

SetRole sets Role field to given value.


### GetOptional

`func (o *Attendee) GetOptional() bool`

GetOptional returns the Optional field if non-nil, zero value otherwise.

### GetOptionalOk

`func (o *Attendee) GetOptionalOk() (*bool, bool)`

GetOptionalOk returns a tuple with the Optional field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOptional

`func (o *Attendee) SetOptional(v bool)`

SetOptional sets Optional field to given value.


### GetComment

`func (o *Attendee) GetComment() string`

GetComment returns the Comment field if non-nil, zero value otherwise.

### GetCommentOk

`func (o *Attendee) GetCommentOk() (*string, bool)`

GetCommentOk returns a tuple with the Comment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetComment

`func (o *Attendee) SetComment(v string)`

SetComment sets Comment field to given value.

### HasComment

`func (o *Attendee) HasComment() bool`

HasComment returns a boolean if a field has been set.

### GetAdditionalGuests

`func (o *Attendee) GetAdditionalGuests() int32`

GetAdditionalGuests returns the AdditionalGuests field if non-nil, zero value otherwise.

### GetAdditionalGuestsOk

`func (o *Attendee) GetAdditionalGuestsOk() (*int32, bool)`

GetAdditionalGuestsOk returns a tuple with the AdditionalGuests field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdditionalGuests

`func (o *Attendee) SetAdditionalGuests(v int32)`

SetAdditionalGuests sets AdditionalGuests field to given value.

### HasAdditionalGuests

`func (o *Attendee) HasAdditionalGuests() bool`

HasAdditionalGuests returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


