# ShareSettings

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**IsPublic** | **bool** |  | 
**HasPassword** | **bool** |  | 
**ShareToken** | Pointer to **string** | Opaque token embedded in the public URL. Empty when &#x60;isPublic&#x60; is false.  | [optional] 
**ShareUrl** | Pointer to **string** | Fully-qualified public viewer URL. Computed server-side from &#x60;PUBLIC_VIEWER_BASE&#x60; (defaults to &#x60;https://spatio.app&#x60;) and the share token. Empty when the note is private.  | [optional] 
**PasswordSetAt** | Pointer to **time.Time** | When the current password was set, if any. | [optional] 

## Methods

### NewShareSettings

`func NewShareSettings(isPublic bool, hasPassword bool, ) *ShareSettings`

NewShareSettings instantiates a new ShareSettings object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewShareSettingsWithDefaults

`func NewShareSettingsWithDefaults() *ShareSettings`

NewShareSettingsWithDefaults instantiates a new ShareSettings object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetIsPublic

`func (o *ShareSettings) GetIsPublic() bool`

GetIsPublic returns the IsPublic field if non-nil, zero value otherwise.

### GetIsPublicOk

`func (o *ShareSettings) GetIsPublicOk() (*bool, bool)`

GetIsPublicOk returns a tuple with the IsPublic field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsPublic

`func (o *ShareSettings) SetIsPublic(v bool)`

SetIsPublic sets IsPublic field to given value.


### GetHasPassword

`func (o *ShareSettings) GetHasPassword() bool`

GetHasPassword returns the HasPassword field if non-nil, zero value otherwise.

### GetHasPasswordOk

`func (o *ShareSettings) GetHasPasswordOk() (*bool, bool)`

GetHasPasswordOk returns a tuple with the HasPassword field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasPassword

`func (o *ShareSettings) SetHasPassword(v bool)`

SetHasPassword sets HasPassword field to given value.


### GetShareToken

`func (o *ShareSettings) GetShareToken() string`

GetShareToken returns the ShareToken field if non-nil, zero value otherwise.

### GetShareTokenOk

`func (o *ShareSettings) GetShareTokenOk() (*string, bool)`

GetShareTokenOk returns a tuple with the ShareToken field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShareToken

`func (o *ShareSettings) SetShareToken(v string)`

SetShareToken sets ShareToken field to given value.

### HasShareToken

`func (o *ShareSettings) HasShareToken() bool`

HasShareToken returns a boolean if a field has been set.

### GetShareUrl

`func (o *ShareSettings) GetShareUrl() string`

GetShareUrl returns the ShareUrl field if non-nil, zero value otherwise.

### GetShareUrlOk

`func (o *ShareSettings) GetShareUrlOk() (*string, bool)`

GetShareUrlOk returns a tuple with the ShareUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShareUrl

`func (o *ShareSettings) SetShareUrl(v string)`

SetShareUrl sets ShareUrl field to given value.

### HasShareUrl

`func (o *ShareSettings) HasShareUrl() bool`

HasShareUrl returns a boolean if a field has been set.

### GetPasswordSetAt

`func (o *ShareSettings) GetPasswordSetAt() time.Time`

GetPasswordSetAt returns the PasswordSetAt field if non-nil, zero value otherwise.

### GetPasswordSetAtOk

`func (o *ShareSettings) GetPasswordSetAtOk() (*time.Time, bool)`

GetPasswordSetAtOk returns a tuple with the PasswordSetAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPasswordSetAt

`func (o *ShareSettings) SetPasswordSetAt(v time.Time)`

SetPasswordSetAt sets PasswordSetAt field to given value.

### HasPasswordSetAt

`func (o *ShareSettings) HasPasswordSetAt() bool`

HasPasswordSetAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


