# AccountTierDetails

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Tier** | **string** |  | 
**DailyApiCalls** | Pointer to **int32** |  | [optional] 
**MaxConnectedAccounts** | Pointer to **int32** |  | [optional] 
**MaxEmailSendsPerDay** | Pointer to **int32** |  | [optional] 
**MaxNotes** | Pointer to **int32** |  | [optional] 
**MaxSheets** | Pointer to **int32** |  | [optional] 
**MaxSlides** | Pointer to **int32** |  | [optional] 
**MaxFiles** | Pointer to **int32** |  | [optional] 
**MaxTasks** | Pointer to **int32** |  | [optional] 
**MaxTeamMembers** | Pointer to **int32** |  | [optional] 
**MaxWorkspaces** | Pointer to **int32** |  | [optional] 
**StorageGb** | Pointer to **int32** |  | [optional] 
**HasAutomations** | Pointer to **bool** |  | [optional] 
**HasAdvancedAutomations** | Pointer to **bool** |  | [optional] 
**HasFullApiAccess** | Pointer to **bool** |  | [optional] 

## Methods

### NewAccountTierDetails

`func NewAccountTierDetails(tier string, ) *AccountTierDetails`

NewAccountTierDetails instantiates a new AccountTierDetails object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAccountTierDetailsWithDefaults

`func NewAccountTierDetailsWithDefaults() *AccountTierDetails`

NewAccountTierDetailsWithDefaults instantiates a new AccountTierDetails object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTier

`func (o *AccountTierDetails) GetTier() string`

GetTier returns the Tier field if non-nil, zero value otherwise.

### GetTierOk

`func (o *AccountTierDetails) GetTierOk() (*string, bool)`

GetTierOk returns a tuple with the Tier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTier

`func (o *AccountTierDetails) SetTier(v string)`

SetTier sets Tier field to given value.


### GetDailyApiCalls

`func (o *AccountTierDetails) GetDailyApiCalls() int32`

GetDailyApiCalls returns the DailyApiCalls field if non-nil, zero value otherwise.

### GetDailyApiCallsOk

`func (o *AccountTierDetails) GetDailyApiCallsOk() (*int32, bool)`

GetDailyApiCallsOk returns a tuple with the DailyApiCalls field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDailyApiCalls

`func (o *AccountTierDetails) SetDailyApiCalls(v int32)`

SetDailyApiCalls sets DailyApiCalls field to given value.

### HasDailyApiCalls

`func (o *AccountTierDetails) HasDailyApiCalls() bool`

HasDailyApiCalls returns a boolean if a field has been set.

### GetMaxConnectedAccounts

`func (o *AccountTierDetails) GetMaxConnectedAccounts() int32`

GetMaxConnectedAccounts returns the MaxConnectedAccounts field if non-nil, zero value otherwise.

### GetMaxConnectedAccountsOk

`func (o *AccountTierDetails) GetMaxConnectedAccountsOk() (*int32, bool)`

GetMaxConnectedAccountsOk returns a tuple with the MaxConnectedAccounts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxConnectedAccounts

`func (o *AccountTierDetails) SetMaxConnectedAccounts(v int32)`

SetMaxConnectedAccounts sets MaxConnectedAccounts field to given value.

### HasMaxConnectedAccounts

`func (o *AccountTierDetails) HasMaxConnectedAccounts() bool`

HasMaxConnectedAccounts returns a boolean if a field has been set.

### GetMaxEmailSendsPerDay

`func (o *AccountTierDetails) GetMaxEmailSendsPerDay() int32`

GetMaxEmailSendsPerDay returns the MaxEmailSendsPerDay field if non-nil, zero value otherwise.

### GetMaxEmailSendsPerDayOk

`func (o *AccountTierDetails) GetMaxEmailSendsPerDayOk() (*int32, bool)`

GetMaxEmailSendsPerDayOk returns a tuple with the MaxEmailSendsPerDay field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxEmailSendsPerDay

`func (o *AccountTierDetails) SetMaxEmailSendsPerDay(v int32)`

SetMaxEmailSendsPerDay sets MaxEmailSendsPerDay field to given value.

### HasMaxEmailSendsPerDay

`func (o *AccountTierDetails) HasMaxEmailSendsPerDay() bool`

HasMaxEmailSendsPerDay returns a boolean if a field has been set.

### GetMaxNotes

`func (o *AccountTierDetails) GetMaxNotes() int32`

GetMaxNotes returns the MaxNotes field if non-nil, zero value otherwise.

### GetMaxNotesOk

`func (o *AccountTierDetails) GetMaxNotesOk() (*int32, bool)`

GetMaxNotesOk returns a tuple with the MaxNotes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxNotes

`func (o *AccountTierDetails) SetMaxNotes(v int32)`

SetMaxNotes sets MaxNotes field to given value.

### HasMaxNotes

`func (o *AccountTierDetails) HasMaxNotes() bool`

HasMaxNotes returns a boolean if a field has been set.

### GetMaxSheets

`func (o *AccountTierDetails) GetMaxSheets() int32`

GetMaxSheets returns the MaxSheets field if non-nil, zero value otherwise.

### GetMaxSheetsOk

`func (o *AccountTierDetails) GetMaxSheetsOk() (*int32, bool)`

GetMaxSheetsOk returns a tuple with the MaxSheets field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxSheets

`func (o *AccountTierDetails) SetMaxSheets(v int32)`

SetMaxSheets sets MaxSheets field to given value.

### HasMaxSheets

`func (o *AccountTierDetails) HasMaxSheets() bool`

HasMaxSheets returns a boolean if a field has been set.

### GetMaxSlides

`func (o *AccountTierDetails) GetMaxSlides() int32`

GetMaxSlides returns the MaxSlides field if non-nil, zero value otherwise.

### GetMaxSlidesOk

`func (o *AccountTierDetails) GetMaxSlidesOk() (*int32, bool)`

GetMaxSlidesOk returns a tuple with the MaxSlides field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxSlides

`func (o *AccountTierDetails) SetMaxSlides(v int32)`

SetMaxSlides sets MaxSlides field to given value.

### HasMaxSlides

`func (o *AccountTierDetails) HasMaxSlides() bool`

HasMaxSlides returns a boolean if a field has been set.

### GetMaxFiles

`func (o *AccountTierDetails) GetMaxFiles() int32`

GetMaxFiles returns the MaxFiles field if non-nil, zero value otherwise.

### GetMaxFilesOk

`func (o *AccountTierDetails) GetMaxFilesOk() (*int32, bool)`

GetMaxFilesOk returns a tuple with the MaxFiles field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxFiles

`func (o *AccountTierDetails) SetMaxFiles(v int32)`

SetMaxFiles sets MaxFiles field to given value.

### HasMaxFiles

`func (o *AccountTierDetails) HasMaxFiles() bool`

HasMaxFiles returns a boolean if a field has been set.

### GetMaxTasks

`func (o *AccountTierDetails) GetMaxTasks() int32`

GetMaxTasks returns the MaxTasks field if non-nil, zero value otherwise.

### GetMaxTasksOk

`func (o *AccountTierDetails) GetMaxTasksOk() (*int32, bool)`

GetMaxTasksOk returns a tuple with the MaxTasks field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxTasks

`func (o *AccountTierDetails) SetMaxTasks(v int32)`

SetMaxTasks sets MaxTasks field to given value.

### HasMaxTasks

`func (o *AccountTierDetails) HasMaxTasks() bool`

HasMaxTasks returns a boolean if a field has been set.

### GetMaxTeamMembers

`func (o *AccountTierDetails) GetMaxTeamMembers() int32`

GetMaxTeamMembers returns the MaxTeamMembers field if non-nil, zero value otherwise.

### GetMaxTeamMembersOk

`func (o *AccountTierDetails) GetMaxTeamMembersOk() (*int32, bool)`

GetMaxTeamMembersOk returns a tuple with the MaxTeamMembers field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxTeamMembers

`func (o *AccountTierDetails) SetMaxTeamMembers(v int32)`

SetMaxTeamMembers sets MaxTeamMembers field to given value.

### HasMaxTeamMembers

`func (o *AccountTierDetails) HasMaxTeamMembers() bool`

HasMaxTeamMembers returns a boolean if a field has been set.

### GetMaxWorkspaces

`func (o *AccountTierDetails) GetMaxWorkspaces() int32`

GetMaxWorkspaces returns the MaxWorkspaces field if non-nil, zero value otherwise.

### GetMaxWorkspacesOk

`func (o *AccountTierDetails) GetMaxWorkspacesOk() (*int32, bool)`

GetMaxWorkspacesOk returns a tuple with the MaxWorkspaces field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxWorkspaces

`func (o *AccountTierDetails) SetMaxWorkspaces(v int32)`

SetMaxWorkspaces sets MaxWorkspaces field to given value.

### HasMaxWorkspaces

`func (o *AccountTierDetails) HasMaxWorkspaces() bool`

HasMaxWorkspaces returns a boolean if a field has been set.

### GetStorageGb

`func (o *AccountTierDetails) GetStorageGb() int32`

GetStorageGb returns the StorageGb field if non-nil, zero value otherwise.

### GetStorageGbOk

`func (o *AccountTierDetails) GetStorageGbOk() (*int32, bool)`

GetStorageGbOk returns a tuple with the StorageGb field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStorageGb

`func (o *AccountTierDetails) SetStorageGb(v int32)`

SetStorageGb sets StorageGb field to given value.

### HasStorageGb

`func (o *AccountTierDetails) HasStorageGb() bool`

HasStorageGb returns a boolean if a field has been set.

### GetHasAutomations

`func (o *AccountTierDetails) GetHasAutomations() bool`

GetHasAutomations returns the HasAutomations field if non-nil, zero value otherwise.

### GetHasAutomationsOk

`func (o *AccountTierDetails) GetHasAutomationsOk() (*bool, bool)`

GetHasAutomationsOk returns a tuple with the HasAutomations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasAutomations

`func (o *AccountTierDetails) SetHasAutomations(v bool)`

SetHasAutomations sets HasAutomations field to given value.

### HasHasAutomations

`func (o *AccountTierDetails) HasHasAutomations() bool`

HasHasAutomations returns a boolean if a field has been set.

### GetHasAdvancedAutomations

`func (o *AccountTierDetails) GetHasAdvancedAutomations() bool`

GetHasAdvancedAutomations returns the HasAdvancedAutomations field if non-nil, zero value otherwise.

### GetHasAdvancedAutomationsOk

`func (o *AccountTierDetails) GetHasAdvancedAutomationsOk() (*bool, bool)`

GetHasAdvancedAutomationsOk returns a tuple with the HasAdvancedAutomations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasAdvancedAutomations

`func (o *AccountTierDetails) SetHasAdvancedAutomations(v bool)`

SetHasAdvancedAutomations sets HasAdvancedAutomations field to given value.

### HasHasAdvancedAutomations

`func (o *AccountTierDetails) HasHasAdvancedAutomations() bool`

HasHasAdvancedAutomations returns a boolean if a field has been set.

### GetHasFullApiAccess

`func (o *AccountTierDetails) GetHasFullApiAccess() bool`

GetHasFullApiAccess returns the HasFullApiAccess field if non-nil, zero value otherwise.

### GetHasFullApiAccessOk

`func (o *AccountTierDetails) GetHasFullApiAccessOk() (*bool, bool)`

GetHasFullApiAccessOk returns a tuple with the HasFullApiAccess field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasFullApiAccess

`func (o *AccountTierDetails) SetHasFullApiAccess(v bool)`

SetHasFullApiAccess sets HasFullApiAccess field to given value.

### HasHasFullApiAccess

`func (o *AccountTierDetails) HasHasFullApiAccess() bool`

HasHasFullApiAccess returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


