# CreateLabelResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Label** | [**Label**](Label.md) |  | 
**Provider** | **string** |  | 

## Methods

### NewCreateLabelResponse

`func NewCreateLabelResponse(label Label, provider string, ) *CreateLabelResponse`

NewCreateLabelResponse instantiates a new CreateLabelResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateLabelResponseWithDefaults

`func NewCreateLabelResponseWithDefaults() *CreateLabelResponse`

NewCreateLabelResponseWithDefaults instantiates a new CreateLabelResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLabel

`func (o *CreateLabelResponse) GetLabel() Label`

GetLabel returns the Label field if non-nil, zero value otherwise.

### GetLabelOk

`func (o *CreateLabelResponse) GetLabelOk() (*Label, bool)`

GetLabelOk returns a tuple with the Label field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabel

`func (o *CreateLabelResponse) SetLabel(v Label)`

SetLabel sets Label field to given value.


### GetProvider

`func (o *CreateLabelResponse) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *CreateLabelResponse) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *CreateLabelResponse) SetProvider(v string)`

SetProvider sets Provider field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


