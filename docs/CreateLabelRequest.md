# CreateLabelRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AccountId** | Pointer to **string** |  | [optional] 
**Name** | **string** |  | 
**MessageListVisibility** | Pointer to **string** |  | [optional] 
**LabelListVisibility** | Pointer to **string** |  | [optional] 
**Color** | Pointer to [**LabelColor**](LabelColor.md) |  | [optional] 

## Methods

### NewCreateLabelRequest

`func NewCreateLabelRequest(name string, ) *CreateLabelRequest`

NewCreateLabelRequest instantiates a new CreateLabelRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateLabelRequestWithDefaults

`func NewCreateLabelRequestWithDefaults() *CreateLabelRequest`

NewCreateLabelRequestWithDefaults instantiates a new CreateLabelRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAccountId

`func (o *CreateLabelRequest) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *CreateLabelRequest) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *CreateLabelRequest) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *CreateLabelRequest) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.

### GetName

`func (o *CreateLabelRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateLabelRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateLabelRequest) SetName(v string)`

SetName sets Name field to given value.


### GetMessageListVisibility

`func (o *CreateLabelRequest) GetMessageListVisibility() string`

GetMessageListVisibility returns the MessageListVisibility field if non-nil, zero value otherwise.

### GetMessageListVisibilityOk

`func (o *CreateLabelRequest) GetMessageListVisibilityOk() (*string, bool)`

GetMessageListVisibilityOk returns a tuple with the MessageListVisibility field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageListVisibility

`func (o *CreateLabelRequest) SetMessageListVisibility(v string)`

SetMessageListVisibility sets MessageListVisibility field to given value.

### HasMessageListVisibility

`func (o *CreateLabelRequest) HasMessageListVisibility() bool`

HasMessageListVisibility returns a boolean if a field has been set.

### GetLabelListVisibility

`func (o *CreateLabelRequest) GetLabelListVisibility() string`

GetLabelListVisibility returns the LabelListVisibility field if non-nil, zero value otherwise.

### GetLabelListVisibilityOk

`func (o *CreateLabelRequest) GetLabelListVisibilityOk() (*string, bool)`

GetLabelListVisibilityOk returns a tuple with the LabelListVisibility field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabelListVisibility

`func (o *CreateLabelRequest) SetLabelListVisibility(v string)`

SetLabelListVisibility sets LabelListVisibility field to given value.

### HasLabelListVisibility

`func (o *CreateLabelRequest) HasLabelListVisibility() bool`

HasLabelListVisibility returns a boolean if a field has been set.

### GetColor

`func (o *CreateLabelRequest) GetColor() LabelColor`

GetColor returns the Color field if non-nil, zero value otherwise.

### GetColorOk

`func (o *CreateLabelRequest) GetColorOk() (*LabelColor, bool)`

GetColorOk returns a tuple with the Color field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetColor

`func (o *CreateLabelRequest) SetColor(v LabelColor)`

SetColor sets Color field to given value.

### HasColor

`func (o *CreateLabelRequest) HasColor() bool`

HasColor returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


