# Reminder

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Method** | [**ReminderMethod**](ReminderMethod.md) |  | 
**Minutes** | **int32** | Trigger time in minutes before the event start. | 

## Methods

### NewReminder

`func NewReminder(method ReminderMethod, minutes int32, ) *Reminder`

NewReminder instantiates a new Reminder object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewReminderWithDefaults

`func NewReminderWithDefaults() *Reminder`

NewReminderWithDefaults instantiates a new Reminder object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMethod

`func (o *Reminder) GetMethod() ReminderMethod`

GetMethod returns the Method field if non-nil, zero value otherwise.

### GetMethodOk

`func (o *Reminder) GetMethodOk() (*ReminderMethod, bool)`

GetMethodOk returns a tuple with the Method field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMethod

`func (o *Reminder) SetMethod(v ReminderMethod)`

SetMethod sets Method field to given value.


### GetMinutes

`func (o *Reminder) GetMinutes() int32`

GetMinutes returns the Minutes field if non-nil, zero value otherwise.

### GetMinutesOk

`func (o *Reminder) GetMinutesOk() (*int32, bool)`

GetMinutesOk returns a tuple with the Minutes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMinutes

`func (o *Reminder) SetMinutes(v int32)`

SetMinutes sets Minutes field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


