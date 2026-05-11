# ListLabelsResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Labels** | [**[]Label**](Label.md) |  | 
**Provider** | **string** |  | 

## Methods

### NewListLabelsResponse

`func NewListLabelsResponse(labels []Label, provider string, ) *ListLabelsResponse`

NewListLabelsResponse instantiates a new ListLabelsResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewListLabelsResponseWithDefaults

`func NewListLabelsResponseWithDefaults() *ListLabelsResponse`

NewListLabelsResponseWithDefaults instantiates a new ListLabelsResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLabels

`func (o *ListLabelsResponse) GetLabels() []Label`

GetLabels returns the Labels field if non-nil, zero value otherwise.

### GetLabelsOk

`func (o *ListLabelsResponse) GetLabelsOk() (*[]Label, bool)`

GetLabelsOk returns a tuple with the Labels field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabels

`func (o *ListLabelsResponse) SetLabels(v []Label)`

SetLabels sets Labels field to given value.


### GetProvider

`func (o *ListLabelsResponse) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *ListLabelsResponse) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *ListLabelsResponse) SetProvider(v string)`

SetProvider sets Provider field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


