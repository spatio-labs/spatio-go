# UserInfoResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Sub** | **string** | User identifier (stable for the lifetime of the user). | 
**Email** | Pointer to **string** |  | [optional] 
**EmailVerified** | Pointer to **bool** |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**GivenName** | Pointer to **string** |  | [optional] 
**FamilyName** | Pointer to **string** |  | [optional] 
**PreferredUsername** | Pointer to **string** |  | [optional] 
**Picture** | Pointer to **string** |  | [optional] 
**UpdatedAt** | Pointer to **int32** |  | [optional] 

## Methods

### NewUserInfoResponse

`func NewUserInfoResponse(sub string, ) *UserInfoResponse`

NewUserInfoResponse instantiates a new UserInfoResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUserInfoResponseWithDefaults

`func NewUserInfoResponseWithDefaults() *UserInfoResponse`

NewUserInfoResponseWithDefaults instantiates a new UserInfoResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSub

`func (o *UserInfoResponse) GetSub() string`

GetSub returns the Sub field if non-nil, zero value otherwise.

### GetSubOk

`func (o *UserInfoResponse) GetSubOk() (*string, bool)`

GetSubOk returns a tuple with the Sub field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSub

`func (o *UserInfoResponse) SetSub(v string)`

SetSub sets Sub field to given value.


### GetEmail

`func (o *UserInfoResponse) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *UserInfoResponse) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *UserInfoResponse) SetEmail(v string)`

SetEmail sets Email field to given value.

### HasEmail

`func (o *UserInfoResponse) HasEmail() bool`

HasEmail returns a boolean if a field has been set.

### GetEmailVerified

`func (o *UserInfoResponse) GetEmailVerified() bool`

GetEmailVerified returns the EmailVerified field if non-nil, zero value otherwise.

### GetEmailVerifiedOk

`func (o *UserInfoResponse) GetEmailVerifiedOk() (*bool, bool)`

GetEmailVerifiedOk returns a tuple with the EmailVerified field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmailVerified

`func (o *UserInfoResponse) SetEmailVerified(v bool)`

SetEmailVerified sets EmailVerified field to given value.

### HasEmailVerified

`func (o *UserInfoResponse) HasEmailVerified() bool`

HasEmailVerified returns a boolean if a field has been set.

### GetName

`func (o *UserInfoResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *UserInfoResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *UserInfoResponse) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *UserInfoResponse) HasName() bool`

HasName returns a boolean if a field has been set.

### GetGivenName

`func (o *UserInfoResponse) GetGivenName() string`

GetGivenName returns the GivenName field if non-nil, zero value otherwise.

### GetGivenNameOk

`func (o *UserInfoResponse) GetGivenNameOk() (*string, bool)`

GetGivenNameOk returns a tuple with the GivenName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGivenName

`func (o *UserInfoResponse) SetGivenName(v string)`

SetGivenName sets GivenName field to given value.

### HasGivenName

`func (o *UserInfoResponse) HasGivenName() bool`

HasGivenName returns a boolean if a field has been set.

### GetFamilyName

`func (o *UserInfoResponse) GetFamilyName() string`

GetFamilyName returns the FamilyName field if non-nil, zero value otherwise.

### GetFamilyNameOk

`func (o *UserInfoResponse) GetFamilyNameOk() (*string, bool)`

GetFamilyNameOk returns a tuple with the FamilyName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFamilyName

`func (o *UserInfoResponse) SetFamilyName(v string)`

SetFamilyName sets FamilyName field to given value.

### HasFamilyName

`func (o *UserInfoResponse) HasFamilyName() bool`

HasFamilyName returns a boolean if a field has been set.

### GetPreferredUsername

`func (o *UserInfoResponse) GetPreferredUsername() string`

GetPreferredUsername returns the PreferredUsername field if non-nil, zero value otherwise.

### GetPreferredUsernameOk

`func (o *UserInfoResponse) GetPreferredUsernameOk() (*string, bool)`

GetPreferredUsernameOk returns a tuple with the PreferredUsername field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPreferredUsername

`func (o *UserInfoResponse) SetPreferredUsername(v string)`

SetPreferredUsername sets PreferredUsername field to given value.

### HasPreferredUsername

`func (o *UserInfoResponse) HasPreferredUsername() bool`

HasPreferredUsername returns a boolean if a field has been set.

### GetPicture

`func (o *UserInfoResponse) GetPicture() string`

GetPicture returns the Picture field if non-nil, zero value otherwise.

### GetPictureOk

`func (o *UserInfoResponse) GetPictureOk() (*string, bool)`

GetPictureOk returns a tuple with the Picture field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPicture

`func (o *UserInfoResponse) SetPicture(v string)`

SetPicture sets Picture field to given value.

### HasPicture

`func (o *UserInfoResponse) HasPicture() bool`

HasPicture returns a boolean if a field has been set.

### GetUpdatedAt

`func (o *UserInfoResponse) GetUpdatedAt() int32`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *UserInfoResponse) GetUpdatedAtOk() (*int32, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *UserInfoResponse) SetUpdatedAt(v int32)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *UserInfoResponse) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


