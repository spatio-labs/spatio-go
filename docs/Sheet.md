# Sheet

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Provider** | Pointer to **string** | Registered provider id (e.g. &#x60;native-sheets&#x60;). | [optional] 
**AccountId** | Pointer to **string** | Connected-account row this sheet belongs to. | [optional] 
**OwnerUserId** | Pointer to **string** | User id of the sheet owner; non-native providers leave empty. | [optional] 
**Name** | **string** |  | 
**Description** | Pointer to **NullableString** |  | [optional] 
**Data** | Pointer to **map[string]interface{}** | Free-form provider blob. Treat as opaque. | [optional] 
**RowCount** | **int32** |  | 
**ColumnCount** | **int32** |  | 
**SheetCount** | **int32** | Tab count when the file contains multiple sheets. | 
**IsPublic** | **bool** |  | 
**IsReadOnly** | **bool** |  | 
**FileSize** | Pointer to **NullableInt32** |  | [optional] 
**LastAccessedAt** | Pointer to **NullableTime** |  | [optional] 
**CreatedAt** | **time.Time** |  | 
**UpdatedAt** | **time.Time** |  | 

## Methods

### NewSheet

`func NewSheet(id string, name string, rowCount int32, columnCount int32, sheetCount int32, isPublic bool, isReadOnly bool, createdAt time.Time, updatedAt time.Time, ) *Sheet`

NewSheet instantiates a new Sheet object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSheetWithDefaults

`func NewSheetWithDefaults() *Sheet`

NewSheetWithDefaults instantiates a new Sheet object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Sheet) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Sheet) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Sheet) SetId(v string)`

SetId sets Id field to given value.


### GetProvider

`func (o *Sheet) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *Sheet) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *Sheet) SetProvider(v string)`

SetProvider sets Provider field to given value.

### HasProvider

`func (o *Sheet) HasProvider() bool`

HasProvider returns a boolean if a field has been set.

### GetAccountId

`func (o *Sheet) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *Sheet) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *Sheet) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *Sheet) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.

### GetOwnerUserId

`func (o *Sheet) GetOwnerUserId() string`

GetOwnerUserId returns the OwnerUserId field if non-nil, zero value otherwise.

### GetOwnerUserIdOk

`func (o *Sheet) GetOwnerUserIdOk() (*string, bool)`

GetOwnerUserIdOk returns a tuple with the OwnerUserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOwnerUserId

`func (o *Sheet) SetOwnerUserId(v string)`

SetOwnerUserId sets OwnerUserId field to given value.

### HasOwnerUserId

`func (o *Sheet) HasOwnerUserId() bool`

HasOwnerUserId returns a boolean if a field has been set.

### GetName

`func (o *Sheet) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Sheet) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Sheet) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *Sheet) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *Sheet) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *Sheet) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *Sheet) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *Sheet) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *Sheet) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetData

`func (o *Sheet) GetData() map[string]interface{}`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *Sheet) GetDataOk() (*map[string]interface{}, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *Sheet) SetData(v map[string]interface{})`

SetData sets Data field to given value.

### HasData

`func (o *Sheet) HasData() bool`

HasData returns a boolean if a field has been set.

### GetRowCount

`func (o *Sheet) GetRowCount() int32`

GetRowCount returns the RowCount field if non-nil, zero value otherwise.

### GetRowCountOk

`func (o *Sheet) GetRowCountOk() (*int32, bool)`

GetRowCountOk returns a tuple with the RowCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRowCount

`func (o *Sheet) SetRowCount(v int32)`

SetRowCount sets RowCount field to given value.


### GetColumnCount

`func (o *Sheet) GetColumnCount() int32`

GetColumnCount returns the ColumnCount field if non-nil, zero value otherwise.

### GetColumnCountOk

`func (o *Sheet) GetColumnCountOk() (*int32, bool)`

GetColumnCountOk returns a tuple with the ColumnCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetColumnCount

`func (o *Sheet) SetColumnCount(v int32)`

SetColumnCount sets ColumnCount field to given value.


### GetSheetCount

`func (o *Sheet) GetSheetCount() int32`

GetSheetCount returns the SheetCount field if non-nil, zero value otherwise.

### GetSheetCountOk

`func (o *Sheet) GetSheetCountOk() (*int32, bool)`

GetSheetCountOk returns a tuple with the SheetCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSheetCount

`func (o *Sheet) SetSheetCount(v int32)`

SetSheetCount sets SheetCount field to given value.


### GetIsPublic

`func (o *Sheet) GetIsPublic() bool`

GetIsPublic returns the IsPublic field if non-nil, zero value otherwise.

### GetIsPublicOk

`func (o *Sheet) GetIsPublicOk() (*bool, bool)`

GetIsPublicOk returns a tuple with the IsPublic field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsPublic

`func (o *Sheet) SetIsPublic(v bool)`

SetIsPublic sets IsPublic field to given value.


### GetIsReadOnly

`func (o *Sheet) GetIsReadOnly() bool`

GetIsReadOnly returns the IsReadOnly field if non-nil, zero value otherwise.

### GetIsReadOnlyOk

`func (o *Sheet) GetIsReadOnlyOk() (*bool, bool)`

GetIsReadOnlyOk returns a tuple with the IsReadOnly field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsReadOnly

`func (o *Sheet) SetIsReadOnly(v bool)`

SetIsReadOnly sets IsReadOnly field to given value.


### GetFileSize

`func (o *Sheet) GetFileSize() int32`

GetFileSize returns the FileSize field if non-nil, zero value otherwise.

### GetFileSizeOk

`func (o *Sheet) GetFileSizeOk() (*int32, bool)`

GetFileSizeOk returns a tuple with the FileSize field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileSize

`func (o *Sheet) SetFileSize(v int32)`

SetFileSize sets FileSize field to given value.

### HasFileSize

`func (o *Sheet) HasFileSize() bool`

HasFileSize returns a boolean if a field has been set.

### SetFileSizeNil

`func (o *Sheet) SetFileSizeNil(b bool)`

 SetFileSizeNil sets the value for FileSize to be an explicit nil

### UnsetFileSize
`func (o *Sheet) UnsetFileSize()`

UnsetFileSize ensures that no value is present for FileSize, not even an explicit nil
### GetLastAccessedAt

`func (o *Sheet) GetLastAccessedAt() time.Time`

GetLastAccessedAt returns the LastAccessedAt field if non-nil, zero value otherwise.

### GetLastAccessedAtOk

`func (o *Sheet) GetLastAccessedAtOk() (*time.Time, bool)`

GetLastAccessedAtOk returns a tuple with the LastAccessedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastAccessedAt

`func (o *Sheet) SetLastAccessedAt(v time.Time)`

SetLastAccessedAt sets LastAccessedAt field to given value.

### HasLastAccessedAt

`func (o *Sheet) HasLastAccessedAt() bool`

HasLastAccessedAt returns a boolean if a field has been set.

### SetLastAccessedAtNil

`func (o *Sheet) SetLastAccessedAtNil(b bool)`

 SetLastAccessedAtNil sets the value for LastAccessedAt to be an explicit nil

### UnsetLastAccessedAt
`func (o *Sheet) UnsetLastAccessedAt()`

UnsetLastAccessedAt ensures that no value is present for LastAccessedAt, not even an explicit nil
### GetCreatedAt

`func (o *Sheet) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Sheet) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Sheet) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *Sheet) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *Sheet) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *Sheet) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


