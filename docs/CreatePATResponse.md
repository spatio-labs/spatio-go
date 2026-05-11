# CreatePATResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Token** | **string** |  | 
**Pat** | Pointer to [**PersonalAccessToken**](PersonalAccessToken.md) |  | [optional] 

## Methods

### NewCreatePATResponse

`func NewCreatePATResponse(token string, ) *CreatePATResponse`

NewCreatePATResponse instantiates a new CreatePATResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreatePATResponseWithDefaults

`func NewCreatePATResponseWithDefaults() *CreatePATResponse`

NewCreatePATResponseWithDefaults instantiates a new CreatePATResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetToken

`func (o *CreatePATResponse) GetToken() string`

GetToken returns the Token field if non-nil, zero value otherwise.

### GetTokenOk

`func (o *CreatePATResponse) GetTokenOk() (*string, bool)`

GetTokenOk returns a tuple with the Token field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetToken

`func (o *CreatePATResponse) SetToken(v string)`

SetToken sets Token field to given value.


### GetPat

`func (o *CreatePATResponse) GetPat() PersonalAccessToken`

GetPat returns the Pat field if non-nil, zero value otherwise.

### GetPatOk

`func (o *CreatePATResponse) GetPatOk() (*PersonalAccessToken, bool)`

GetPatOk returns a tuple with the Pat field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPat

`func (o *CreatePATResponse) SetPat(v PersonalAccessToken)`

SetPat sets Pat field to given value.

### HasPat

`func (o *CreatePATResponse) HasPat() bool`

HasPat returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


