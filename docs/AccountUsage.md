# AccountUsage

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Date** | **string** | Always &#x60;today&#x60; for the current-day rollup. | 
**ApiCalls** | Pointer to **int32** |  | [optional] 
**EmailSends** | Pointer to **int32** |  | [optional] 
**NotesCount** | Pointer to **int32** |  | [optional] 
**SheetsCount** | Pointer to **int32** |  | [optional] 
**SlidesCount** | Pointer to **int32** |  | [optional] 
**FilesCount** | Pointer to **int32** |  | [optional] 
**TasksCount** | Pointer to **int32** |  | [optional] 

## Methods

### NewAccountUsage

`func NewAccountUsage(date string, ) *AccountUsage`

NewAccountUsage instantiates a new AccountUsage object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAccountUsageWithDefaults

`func NewAccountUsageWithDefaults() *AccountUsage`

NewAccountUsageWithDefaults instantiates a new AccountUsage object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDate

`func (o *AccountUsage) GetDate() string`

GetDate returns the Date field if non-nil, zero value otherwise.

### GetDateOk

`func (o *AccountUsage) GetDateOk() (*string, bool)`

GetDateOk returns a tuple with the Date field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDate

`func (o *AccountUsage) SetDate(v string)`

SetDate sets Date field to given value.


### GetApiCalls

`func (o *AccountUsage) GetApiCalls() int32`

GetApiCalls returns the ApiCalls field if non-nil, zero value otherwise.

### GetApiCallsOk

`func (o *AccountUsage) GetApiCallsOk() (*int32, bool)`

GetApiCallsOk returns a tuple with the ApiCalls field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApiCalls

`func (o *AccountUsage) SetApiCalls(v int32)`

SetApiCalls sets ApiCalls field to given value.

### HasApiCalls

`func (o *AccountUsage) HasApiCalls() bool`

HasApiCalls returns a boolean if a field has been set.

### GetEmailSends

`func (o *AccountUsage) GetEmailSends() int32`

GetEmailSends returns the EmailSends field if non-nil, zero value otherwise.

### GetEmailSendsOk

`func (o *AccountUsage) GetEmailSendsOk() (*int32, bool)`

GetEmailSendsOk returns a tuple with the EmailSends field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmailSends

`func (o *AccountUsage) SetEmailSends(v int32)`

SetEmailSends sets EmailSends field to given value.

### HasEmailSends

`func (o *AccountUsage) HasEmailSends() bool`

HasEmailSends returns a boolean if a field has been set.

### GetNotesCount

`func (o *AccountUsage) GetNotesCount() int32`

GetNotesCount returns the NotesCount field if non-nil, zero value otherwise.

### GetNotesCountOk

`func (o *AccountUsage) GetNotesCountOk() (*int32, bool)`

GetNotesCountOk returns a tuple with the NotesCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNotesCount

`func (o *AccountUsage) SetNotesCount(v int32)`

SetNotesCount sets NotesCount field to given value.

### HasNotesCount

`func (o *AccountUsage) HasNotesCount() bool`

HasNotesCount returns a boolean if a field has been set.

### GetSheetsCount

`func (o *AccountUsage) GetSheetsCount() int32`

GetSheetsCount returns the SheetsCount field if non-nil, zero value otherwise.

### GetSheetsCountOk

`func (o *AccountUsage) GetSheetsCountOk() (*int32, bool)`

GetSheetsCountOk returns a tuple with the SheetsCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSheetsCount

`func (o *AccountUsage) SetSheetsCount(v int32)`

SetSheetsCount sets SheetsCount field to given value.

### HasSheetsCount

`func (o *AccountUsage) HasSheetsCount() bool`

HasSheetsCount returns a boolean if a field has been set.

### GetSlidesCount

`func (o *AccountUsage) GetSlidesCount() int32`

GetSlidesCount returns the SlidesCount field if non-nil, zero value otherwise.

### GetSlidesCountOk

`func (o *AccountUsage) GetSlidesCountOk() (*int32, bool)`

GetSlidesCountOk returns a tuple with the SlidesCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlidesCount

`func (o *AccountUsage) SetSlidesCount(v int32)`

SetSlidesCount sets SlidesCount field to given value.

### HasSlidesCount

`func (o *AccountUsage) HasSlidesCount() bool`

HasSlidesCount returns a boolean if a field has been set.

### GetFilesCount

`func (o *AccountUsage) GetFilesCount() int32`

GetFilesCount returns the FilesCount field if non-nil, zero value otherwise.

### GetFilesCountOk

`func (o *AccountUsage) GetFilesCountOk() (*int32, bool)`

GetFilesCountOk returns a tuple with the FilesCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilesCount

`func (o *AccountUsage) SetFilesCount(v int32)`

SetFilesCount sets FilesCount field to given value.

### HasFilesCount

`func (o *AccountUsage) HasFilesCount() bool`

HasFilesCount returns a boolean if a field has been set.

### GetTasksCount

`func (o *AccountUsage) GetTasksCount() int32`

GetTasksCount returns the TasksCount field if non-nil, zero value otherwise.

### GetTasksCountOk

`func (o *AccountUsage) GetTasksCountOk() (*int32, bool)`

GetTasksCountOk returns a tuple with the TasksCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTasksCount

`func (o *AccountUsage) SetTasksCount(v int32)`

SetTasksCount sets TasksCount field to given value.

### HasTasksCount

`func (o *AccountUsage) HasTasksCount() bool`

HasTasksCount returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


