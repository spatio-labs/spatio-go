# SpatioEvent

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Title** | **string** |  | 
**Description** | Pointer to **string** |  | [optional] 
**StartTime** | **time.Time** |  | 
**EndTime** | **time.Time** |  | 
**AllDay** | **bool** |  | 
**Location** | Pointer to **string** |  | [optional] 
**LocationDetails** | Pointer to **map[string]string** | Free-form key/value (lat, lng, room, etc.). | [optional] 
**Organizer** | Pointer to **string** | Organizer email. | [optional] 
**Attendees** | Pointer to [**[]Attendee**](Attendee.md) |  | [optional] 
**RecurrenceRule** | Pointer to **string** | RFC 5545 RRULE. | [optional] 
**RecurrenceId** | Pointer to **string** | Set on instances of a recurring series. | [optional] 
**OriginalStart** | Pointer to **time.Time** | Original start of a moved recurring instance. | [optional] 
**Status** | **string** | Provider-mapped event status. Free-form string — common values are &#x60;confirmed&#x60;, &#x60;tentative&#x60;, &#x60;cancelled&#x60;, &#x60;needs_action&#x60;, and the empty string when the provider doesn&#39;t populate it. Not enumerated strictly because providers add custom values and the platform passes them through verbatim.  | 
**Visibility** | **string** | Free-form visibility string. Common values: &#x60;public&#x60;, &#x60;private&#x60;, &#x60;confidential&#x60;, plus empty when unset.  | 
**Busy** | **bool** | Whether this event marks the time as busy or free. | 
**Reminders** | Pointer to [**[]Reminder**](Reminder.md) |  | [optional] 
**TravelTimeMinutes** | Pointer to **NullableInt32** | Apple Calendar&#39;s local-only travel buffer. Stored on the cached row but not synced to providers that don&#39;t model it.  | [optional] 
**Categories** | Pointer to **[]string** |  | [optional] 
**Color** | Pointer to **string** |  | [optional] 
**UserId** | Pointer to **string** |  | [optional] 
**AccountId** | **string** |  | 
**Provider** | Pointer to **string** | Standardized provider id (e.g. &#x60;google-calendar&#x60;, &#x60;native-calendar&#x60;). Mirrors &#x60;provider_id&#x60; — both are populated on writes; clients should prefer &#x60;provider&#x60;.  | [optional] 
**ProviderId** | **string** | Legacy alias of &#x60;provider&#x60;. | 
**ProviderData** | Pointer to **map[string]interface{}** | Provider-specific extras. | [optional] 
**CreatedAt** | **time.Time** |  | 
**UpdatedAt** | **time.Time** |  | 
**DeletedAt** | Pointer to **NullableTime** |  | [optional] 
**SyncedAt** | Pointer to **time.Time** |  | [optional] 
**ConferenceData** | Pointer to [**ConferenceData**](ConferenceData.md) |  | [optional] 
**Attachments** | Pointer to [**[]Attachment**](Attachment.md) |  | [optional] 
**Url** | Pointer to **string** |  | [optional] 
**Etag** | Pointer to **string** |  | [optional] 
**Sequence** | Pointer to **int32** |  | [optional] 
**CustomData** | Pointer to **map[string]string** |  | [optional] 

## Methods

### NewSpatioEvent

`func NewSpatioEvent(id string, title string, startTime time.Time, endTime time.Time, allDay bool, status string, visibility string, busy bool, accountId string, providerId string, createdAt time.Time, updatedAt time.Time, ) *SpatioEvent`

NewSpatioEvent instantiates a new SpatioEvent object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSpatioEventWithDefaults

`func NewSpatioEventWithDefaults() *SpatioEvent`

NewSpatioEventWithDefaults instantiates a new SpatioEvent object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *SpatioEvent) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *SpatioEvent) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *SpatioEvent) SetId(v string)`

SetId sets Id field to given value.


### GetTitle

`func (o *SpatioEvent) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *SpatioEvent) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *SpatioEvent) SetTitle(v string)`

SetTitle sets Title field to given value.


### GetDescription

`func (o *SpatioEvent) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *SpatioEvent) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *SpatioEvent) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *SpatioEvent) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetStartTime

`func (o *SpatioEvent) GetStartTime() time.Time`

GetStartTime returns the StartTime field if non-nil, zero value otherwise.

### GetStartTimeOk

`func (o *SpatioEvent) GetStartTimeOk() (*time.Time, bool)`

GetStartTimeOk returns a tuple with the StartTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStartTime

`func (o *SpatioEvent) SetStartTime(v time.Time)`

SetStartTime sets StartTime field to given value.


### GetEndTime

`func (o *SpatioEvent) GetEndTime() time.Time`

GetEndTime returns the EndTime field if non-nil, zero value otherwise.

### GetEndTimeOk

`func (o *SpatioEvent) GetEndTimeOk() (*time.Time, bool)`

GetEndTimeOk returns a tuple with the EndTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndTime

`func (o *SpatioEvent) SetEndTime(v time.Time)`

SetEndTime sets EndTime field to given value.


### GetAllDay

`func (o *SpatioEvent) GetAllDay() bool`

GetAllDay returns the AllDay field if non-nil, zero value otherwise.

### GetAllDayOk

`func (o *SpatioEvent) GetAllDayOk() (*bool, bool)`

GetAllDayOk returns a tuple with the AllDay field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAllDay

`func (o *SpatioEvent) SetAllDay(v bool)`

SetAllDay sets AllDay field to given value.


### GetLocation

`func (o *SpatioEvent) GetLocation() string`

GetLocation returns the Location field if non-nil, zero value otherwise.

### GetLocationOk

`func (o *SpatioEvent) GetLocationOk() (*string, bool)`

GetLocationOk returns a tuple with the Location field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLocation

`func (o *SpatioEvent) SetLocation(v string)`

SetLocation sets Location field to given value.

### HasLocation

`func (o *SpatioEvent) HasLocation() bool`

HasLocation returns a boolean if a field has been set.

### GetLocationDetails

`func (o *SpatioEvent) GetLocationDetails() map[string]string`

GetLocationDetails returns the LocationDetails field if non-nil, zero value otherwise.

### GetLocationDetailsOk

`func (o *SpatioEvent) GetLocationDetailsOk() (*map[string]string, bool)`

GetLocationDetailsOk returns a tuple with the LocationDetails field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLocationDetails

`func (o *SpatioEvent) SetLocationDetails(v map[string]string)`

SetLocationDetails sets LocationDetails field to given value.

### HasLocationDetails

`func (o *SpatioEvent) HasLocationDetails() bool`

HasLocationDetails returns a boolean if a field has been set.

### GetOrganizer

`func (o *SpatioEvent) GetOrganizer() string`

GetOrganizer returns the Organizer field if non-nil, zero value otherwise.

### GetOrganizerOk

`func (o *SpatioEvent) GetOrganizerOk() (*string, bool)`

GetOrganizerOk returns a tuple with the Organizer field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrganizer

`func (o *SpatioEvent) SetOrganizer(v string)`

SetOrganizer sets Organizer field to given value.

### HasOrganizer

`func (o *SpatioEvent) HasOrganizer() bool`

HasOrganizer returns a boolean if a field has been set.

### GetAttendees

`func (o *SpatioEvent) GetAttendees() []Attendee`

GetAttendees returns the Attendees field if non-nil, zero value otherwise.

### GetAttendeesOk

`func (o *SpatioEvent) GetAttendeesOk() (*[]Attendee, bool)`

GetAttendeesOk returns a tuple with the Attendees field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttendees

`func (o *SpatioEvent) SetAttendees(v []Attendee)`

SetAttendees sets Attendees field to given value.

### HasAttendees

`func (o *SpatioEvent) HasAttendees() bool`

HasAttendees returns a boolean if a field has been set.

### GetRecurrenceRule

`func (o *SpatioEvent) GetRecurrenceRule() string`

GetRecurrenceRule returns the RecurrenceRule field if non-nil, zero value otherwise.

### GetRecurrenceRuleOk

`func (o *SpatioEvent) GetRecurrenceRuleOk() (*string, bool)`

GetRecurrenceRuleOk returns a tuple with the RecurrenceRule field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRecurrenceRule

`func (o *SpatioEvent) SetRecurrenceRule(v string)`

SetRecurrenceRule sets RecurrenceRule field to given value.

### HasRecurrenceRule

`func (o *SpatioEvent) HasRecurrenceRule() bool`

HasRecurrenceRule returns a boolean if a field has been set.

### GetRecurrenceId

`func (o *SpatioEvent) GetRecurrenceId() string`

GetRecurrenceId returns the RecurrenceId field if non-nil, zero value otherwise.

### GetRecurrenceIdOk

`func (o *SpatioEvent) GetRecurrenceIdOk() (*string, bool)`

GetRecurrenceIdOk returns a tuple with the RecurrenceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRecurrenceId

`func (o *SpatioEvent) SetRecurrenceId(v string)`

SetRecurrenceId sets RecurrenceId field to given value.

### HasRecurrenceId

`func (o *SpatioEvent) HasRecurrenceId() bool`

HasRecurrenceId returns a boolean if a field has been set.

### GetOriginalStart

`func (o *SpatioEvent) GetOriginalStart() time.Time`

GetOriginalStart returns the OriginalStart field if non-nil, zero value otherwise.

### GetOriginalStartOk

`func (o *SpatioEvent) GetOriginalStartOk() (*time.Time, bool)`

GetOriginalStartOk returns a tuple with the OriginalStart field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOriginalStart

`func (o *SpatioEvent) SetOriginalStart(v time.Time)`

SetOriginalStart sets OriginalStart field to given value.

### HasOriginalStart

`func (o *SpatioEvent) HasOriginalStart() bool`

HasOriginalStart returns a boolean if a field has been set.

### GetStatus

`func (o *SpatioEvent) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *SpatioEvent) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *SpatioEvent) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetVisibility

`func (o *SpatioEvent) GetVisibility() string`

GetVisibility returns the Visibility field if non-nil, zero value otherwise.

### GetVisibilityOk

`func (o *SpatioEvent) GetVisibilityOk() (*string, bool)`

GetVisibilityOk returns a tuple with the Visibility field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVisibility

`func (o *SpatioEvent) SetVisibility(v string)`

SetVisibility sets Visibility field to given value.


### GetBusy

`func (o *SpatioEvent) GetBusy() bool`

GetBusy returns the Busy field if non-nil, zero value otherwise.

### GetBusyOk

`func (o *SpatioEvent) GetBusyOk() (*bool, bool)`

GetBusyOk returns a tuple with the Busy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBusy

`func (o *SpatioEvent) SetBusy(v bool)`

SetBusy sets Busy field to given value.


### GetReminders

`func (o *SpatioEvent) GetReminders() []Reminder`

GetReminders returns the Reminders field if non-nil, zero value otherwise.

### GetRemindersOk

`func (o *SpatioEvent) GetRemindersOk() (*[]Reminder, bool)`

GetRemindersOk returns a tuple with the Reminders field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReminders

`func (o *SpatioEvent) SetReminders(v []Reminder)`

SetReminders sets Reminders field to given value.

### HasReminders

`func (o *SpatioEvent) HasReminders() bool`

HasReminders returns a boolean if a field has been set.

### GetTravelTimeMinutes

`func (o *SpatioEvent) GetTravelTimeMinutes() int32`

GetTravelTimeMinutes returns the TravelTimeMinutes field if non-nil, zero value otherwise.

### GetTravelTimeMinutesOk

`func (o *SpatioEvent) GetTravelTimeMinutesOk() (*int32, bool)`

GetTravelTimeMinutesOk returns a tuple with the TravelTimeMinutes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTravelTimeMinutes

`func (o *SpatioEvent) SetTravelTimeMinutes(v int32)`

SetTravelTimeMinutes sets TravelTimeMinutes field to given value.

### HasTravelTimeMinutes

`func (o *SpatioEvent) HasTravelTimeMinutes() bool`

HasTravelTimeMinutes returns a boolean if a field has been set.

### SetTravelTimeMinutesNil

`func (o *SpatioEvent) SetTravelTimeMinutesNil(b bool)`

 SetTravelTimeMinutesNil sets the value for TravelTimeMinutes to be an explicit nil

### UnsetTravelTimeMinutes
`func (o *SpatioEvent) UnsetTravelTimeMinutes()`

UnsetTravelTimeMinutes ensures that no value is present for TravelTimeMinutes, not even an explicit nil
### GetCategories

`func (o *SpatioEvent) GetCategories() []string`

GetCategories returns the Categories field if non-nil, zero value otherwise.

### GetCategoriesOk

`func (o *SpatioEvent) GetCategoriesOk() (*[]string, bool)`

GetCategoriesOk returns a tuple with the Categories field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCategories

`func (o *SpatioEvent) SetCategories(v []string)`

SetCategories sets Categories field to given value.

### HasCategories

`func (o *SpatioEvent) HasCategories() bool`

HasCategories returns a boolean if a field has been set.

### GetColor

`func (o *SpatioEvent) GetColor() string`

GetColor returns the Color field if non-nil, zero value otherwise.

### GetColorOk

`func (o *SpatioEvent) GetColorOk() (*string, bool)`

GetColorOk returns a tuple with the Color field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetColor

`func (o *SpatioEvent) SetColor(v string)`

SetColor sets Color field to given value.

### HasColor

`func (o *SpatioEvent) HasColor() bool`

HasColor returns a boolean if a field has been set.

### GetUserId

`func (o *SpatioEvent) GetUserId() string`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *SpatioEvent) GetUserIdOk() (*string, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *SpatioEvent) SetUserId(v string)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *SpatioEvent) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetAccountId

`func (o *SpatioEvent) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *SpatioEvent) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *SpatioEvent) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.


### GetProvider

`func (o *SpatioEvent) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *SpatioEvent) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *SpatioEvent) SetProvider(v string)`

SetProvider sets Provider field to given value.

### HasProvider

`func (o *SpatioEvent) HasProvider() bool`

HasProvider returns a boolean if a field has been set.

### GetProviderId

`func (o *SpatioEvent) GetProviderId() string`

GetProviderId returns the ProviderId field if non-nil, zero value otherwise.

### GetProviderIdOk

`func (o *SpatioEvent) GetProviderIdOk() (*string, bool)`

GetProviderIdOk returns a tuple with the ProviderId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProviderId

`func (o *SpatioEvent) SetProviderId(v string)`

SetProviderId sets ProviderId field to given value.


### GetProviderData

`func (o *SpatioEvent) GetProviderData() map[string]interface{}`

GetProviderData returns the ProviderData field if non-nil, zero value otherwise.

### GetProviderDataOk

`func (o *SpatioEvent) GetProviderDataOk() (*map[string]interface{}, bool)`

GetProviderDataOk returns a tuple with the ProviderData field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProviderData

`func (o *SpatioEvent) SetProviderData(v map[string]interface{})`

SetProviderData sets ProviderData field to given value.

### HasProviderData

`func (o *SpatioEvent) HasProviderData() bool`

HasProviderData returns a boolean if a field has been set.

### GetCreatedAt

`func (o *SpatioEvent) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *SpatioEvent) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *SpatioEvent) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *SpatioEvent) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *SpatioEvent) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *SpatioEvent) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.


### GetDeletedAt

`func (o *SpatioEvent) GetDeletedAt() time.Time`

GetDeletedAt returns the DeletedAt field if non-nil, zero value otherwise.

### GetDeletedAtOk

`func (o *SpatioEvent) GetDeletedAtOk() (*time.Time, bool)`

GetDeletedAtOk returns a tuple with the DeletedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeletedAt

`func (o *SpatioEvent) SetDeletedAt(v time.Time)`

SetDeletedAt sets DeletedAt field to given value.

### HasDeletedAt

`func (o *SpatioEvent) HasDeletedAt() bool`

HasDeletedAt returns a boolean if a field has been set.

### SetDeletedAtNil

`func (o *SpatioEvent) SetDeletedAtNil(b bool)`

 SetDeletedAtNil sets the value for DeletedAt to be an explicit nil

### UnsetDeletedAt
`func (o *SpatioEvent) UnsetDeletedAt()`

UnsetDeletedAt ensures that no value is present for DeletedAt, not even an explicit nil
### GetSyncedAt

`func (o *SpatioEvent) GetSyncedAt() time.Time`

GetSyncedAt returns the SyncedAt field if non-nil, zero value otherwise.

### GetSyncedAtOk

`func (o *SpatioEvent) GetSyncedAtOk() (*time.Time, bool)`

GetSyncedAtOk returns a tuple with the SyncedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSyncedAt

`func (o *SpatioEvent) SetSyncedAt(v time.Time)`

SetSyncedAt sets SyncedAt field to given value.

### HasSyncedAt

`func (o *SpatioEvent) HasSyncedAt() bool`

HasSyncedAt returns a boolean if a field has been set.

### GetConferenceData

`func (o *SpatioEvent) GetConferenceData() ConferenceData`

GetConferenceData returns the ConferenceData field if non-nil, zero value otherwise.

### GetConferenceDataOk

`func (o *SpatioEvent) GetConferenceDataOk() (*ConferenceData, bool)`

GetConferenceDataOk returns a tuple with the ConferenceData field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConferenceData

`func (o *SpatioEvent) SetConferenceData(v ConferenceData)`

SetConferenceData sets ConferenceData field to given value.

### HasConferenceData

`func (o *SpatioEvent) HasConferenceData() bool`

HasConferenceData returns a boolean if a field has been set.

### GetAttachments

`func (o *SpatioEvent) GetAttachments() []Attachment`

GetAttachments returns the Attachments field if non-nil, zero value otherwise.

### GetAttachmentsOk

`func (o *SpatioEvent) GetAttachmentsOk() (*[]Attachment, bool)`

GetAttachmentsOk returns a tuple with the Attachments field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttachments

`func (o *SpatioEvent) SetAttachments(v []Attachment)`

SetAttachments sets Attachments field to given value.

### HasAttachments

`func (o *SpatioEvent) HasAttachments() bool`

HasAttachments returns a boolean if a field has been set.

### GetUrl

`func (o *SpatioEvent) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *SpatioEvent) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *SpatioEvent) SetUrl(v string)`

SetUrl sets Url field to given value.

### HasUrl

`func (o *SpatioEvent) HasUrl() bool`

HasUrl returns a boolean if a field has been set.

### GetEtag

`func (o *SpatioEvent) GetEtag() string`

GetEtag returns the Etag field if non-nil, zero value otherwise.

### GetEtagOk

`func (o *SpatioEvent) GetEtagOk() (*string, bool)`

GetEtagOk returns a tuple with the Etag field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEtag

`func (o *SpatioEvent) SetEtag(v string)`

SetEtag sets Etag field to given value.

### HasEtag

`func (o *SpatioEvent) HasEtag() bool`

HasEtag returns a boolean if a field has been set.

### GetSequence

`func (o *SpatioEvent) GetSequence() int32`

GetSequence returns the Sequence field if non-nil, zero value otherwise.

### GetSequenceOk

`func (o *SpatioEvent) GetSequenceOk() (*int32, bool)`

GetSequenceOk returns a tuple with the Sequence field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSequence

`func (o *SpatioEvent) SetSequence(v int32)`

SetSequence sets Sequence field to given value.

### HasSequence

`func (o *SpatioEvent) HasSequence() bool`

HasSequence returns a boolean if a field has been set.

### GetCustomData

`func (o *SpatioEvent) GetCustomData() map[string]string`

GetCustomData returns the CustomData field if non-nil, zero value otherwise.

### GetCustomDataOk

`func (o *SpatioEvent) GetCustomDataOk() (*map[string]string, bool)`

GetCustomDataOk returns a tuple with the CustomData field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomData

`func (o *SpatioEvent) SetCustomData(v map[string]string)`

SetCustomData sets CustomData field to given value.

### HasCustomData

`func (o *SpatioEvent) HasCustomData() bool`

HasCustomData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


