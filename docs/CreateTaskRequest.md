# CreateTaskRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Title** | **string** |  | 
**Description** | Pointer to **string** |  | [optional] 
**Status** | Pointer to **string** |  | [optional] 
**DueDate** | Pointer to **NullableTime** |  | [optional] 
**Priority** | Pointer to **string** |  | [optional] 
**Labels** | Pointer to **[]string** |  | [optional] 
**Tags** | Pointer to **[]string** |  | [optional] 
**AssigneeId** | Pointer to **string** |  | [optional] 
**ParentTaskId** | Pointer to **NullableString** |  | [optional] 
**Type** | Pointer to **string** |  | [optional] 
**SourcePlatform** | Pointer to **string** |  | [optional] 
**SourceId** | Pointer to **string** |  | [optional] 
**AccountId** | Pointer to **string** | Optional override for the target connected account. May also be passed as &#x60;?accountId&#x3D;&#x60;.  | [optional] 
**Provider** | Pointer to **string** |  | [optional] 

## Methods

### NewCreateTaskRequest

`func NewCreateTaskRequest(title string, ) *CreateTaskRequest`

NewCreateTaskRequest instantiates a new CreateTaskRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateTaskRequestWithDefaults

`func NewCreateTaskRequestWithDefaults() *CreateTaskRequest`

NewCreateTaskRequestWithDefaults instantiates a new CreateTaskRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTitle

`func (o *CreateTaskRequest) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *CreateTaskRequest) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *CreateTaskRequest) SetTitle(v string)`

SetTitle sets Title field to given value.


### GetDescription

`func (o *CreateTaskRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *CreateTaskRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *CreateTaskRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *CreateTaskRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetStatus

`func (o *CreateTaskRequest) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *CreateTaskRequest) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *CreateTaskRequest) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *CreateTaskRequest) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetDueDate

`func (o *CreateTaskRequest) GetDueDate() time.Time`

GetDueDate returns the DueDate field if non-nil, zero value otherwise.

### GetDueDateOk

`func (o *CreateTaskRequest) GetDueDateOk() (*time.Time, bool)`

GetDueDateOk returns a tuple with the DueDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDueDate

`func (o *CreateTaskRequest) SetDueDate(v time.Time)`

SetDueDate sets DueDate field to given value.

### HasDueDate

`func (o *CreateTaskRequest) HasDueDate() bool`

HasDueDate returns a boolean if a field has been set.

### SetDueDateNil

`func (o *CreateTaskRequest) SetDueDateNil(b bool)`

 SetDueDateNil sets the value for DueDate to be an explicit nil

### UnsetDueDate
`func (o *CreateTaskRequest) UnsetDueDate()`

UnsetDueDate ensures that no value is present for DueDate, not even an explicit nil
### GetPriority

`func (o *CreateTaskRequest) GetPriority() string`

GetPriority returns the Priority field if non-nil, zero value otherwise.

### GetPriorityOk

`func (o *CreateTaskRequest) GetPriorityOk() (*string, bool)`

GetPriorityOk returns a tuple with the Priority field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriority

`func (o *CreateTaskRequest) SetPriority(v string)`

SetPriority sets Priority field to given value.

### HasPriority

`func (o *CreateTaskRequest) HasPriority() bool`

HasPriority returns a boolean if a field has been set.

### GetLabels

`func (o *CreateTaskRequest) GetLabels() []string`

GetLabels returns the Labels field if non-nil, zero value otherwise.

### GetLabelsOk

`func (o *CreateTaskRequest) GetLabelsOk() (*[]string, bool)`

GetLabelsOk returns a tuple with the Labels field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabels

`func (o *CreateTaskRequest) SetLabels(v []string)`

SetLabels sets Labels field to given value.

### HasLabels

`func (o *CreateTaskRequest) HasLabels() bool`

HasLabels returns a boolean if a field has been set.

### GetTags

`func (o *CreateTaskRequest) GetTags() []string`

GetTags returns the Tags field if non-nil, zero value otherwise.

### GetTagsOk

`func (o *CreateTaskRequest) GetTagsOk() (*[]string, bool)`

GetTagsOk returns a tuple with the Tags field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTags

`func (o *CreateTaskRequest) SetTags(v []string)`

SetTags sets Tags field to given value.

### HasTags

`func (o *CreateTaskRequest) HasTags() bool`

HasTags returns a boolean if a field has been set.

### GetAssigneeId

`func (o *CreateTaskRequest) GetAssigneeId() string`

GetAssigneeId returns the AssigneeId field if non-nil, zero value otherwise.

### GetAssigneeIdOk

`func (o *CreateTaskRequest) GetAssigneeIdOk() (*string, bool)`

GetAssigneeIdOk returns a tuple with the AssigneeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAssigneeId

`func (o *CreateTaskRequest) SetAssigneeId(v string)`

SetAssigneeId sets AssigneeId field to given value.

### HasAssigneeId

`func (o *CreateTaskRequest) HasAssigneeId() bool`

HasAssigneeId returns a boolean if a field has been set.

### GetParentTaskId

`func (o *CreateTaskRequest) GetParentTaskId() string`

GetParentTaskId returns the ParentTaskId field if non-nil, zero value otherwise.

### GetParentTaskIdOk

`func (o *CreateTaskRequest) GetParentTaskIdOk() (*string, bool)`

GetParentTaskIdOk returns a tuple with the ParentTaskId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetParentTaskId

`func (o *CreateTaskRequest) SetParentTaskId(v string)`

SetParentTaskId sets ParentTaskId field to given value.

### HasParentTaskId

`func (o *CreateTaskRequest) HasParentTaskId() bool`

HasParentTaskId returns a boolean if a field has been set.

### SetParentTaskIdNil

`func (o *CreateTaskRequest) SetParentTaskIdNil(b bool)`

 SetParentTaskIdNil sets the value for ParentTaskId to be an explicit nil

### UnsetParentTaskId
`func (o *CreateTaskRequest) UnsetParentTaskId()`

UnsetParentTaskId ensures that no value is present for ParentTaskId, not even an explicit nil
### GetType

`func (o *CreateTaskRequest) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *CreateTaskRequest) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *CreateTaskRequest) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *CreateTaskRequest) HasType() bool`

HasType returns a boolean if a field has been set.

### GetSourcePlatform

`func (o *CreateTaskRequest) GetSourcePlatform() string`

GetSourcePlatform returns the SourcePlatform field if non-nil, zero value otherwise.

### GetSourcePlatformOk

`func (o *CreateTaskRequest) GetSourcePlatformOk() (*string, bool)`

GetSourcePlatformOk returns a tuple with the SourcePlatform field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourcePlatform

`func (o *CreateTaskRequest) SetSourcePlatform(v string)`

SetSourcePlatform sets SourcePlatform field to given value.

### HasSourcePlatform

`func (o *CreateTaskRequest) HasSourcePlatform() bool`

HasSourcePlatform returns a boolean if a field has been set.

### GetSourceId

`func (o *CreateTaskRequest) GetSourceId() string`

GetSourceId returns the SourceId field if non-nil, zero value otherwise.

### GetSourceIdOk

`func (o *CreateTaskRequest) GetSourceIdOk() (*string, bool)`

GetSourceIdOk returns a tuple with the SourceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceId

`func (o *CreateTaskRequest) SetSourceId(v string)`

SetSourceId sets SourceId field to given value.

### HasSourceId

`func (o *CreateTaskRequest) HasSourceId() bool`

HasSourceId returns a boolean if a field has been set.

### GetAccountId

`func (o *CreateTaskRequest) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *CreateTaskRequest) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *CreateTaskRequest) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *CreateTaskRequest) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.

### GetProvider

`func (o *CreateTaskRequest) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *CreateTaskRequest) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *CreateTaskRequest) SetProvider(v string)`

SetProvider sets Provider field to given value.

### HasProvider

`func (o *CreateTaskRequest) HasProvider() bool`

HasProvider returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


