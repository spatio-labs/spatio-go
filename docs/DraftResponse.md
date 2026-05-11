# DraftResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Draft** | [**Draft**](Draft.md) |  | 
**Provider** | **string** |  | 

## Methods

### NewDraftResponse

`func NewDraftResponse(draft Draft, provider string, ) *DraftResponse`

NewDraftResponse instantiates a new DraftResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDraftResponseWithDefaults

`func NewDraftResponseWithDefaults() *DraftResponse`

NewDraftResponseWithDefaults instantiates a new DraftResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDraft

`func (o *DraftResponse) GetDraft() Draft`

GetDraft returns the Draft field if non-nil, zero value otherwise.

### GetDraftOk

`func (o *DraftResponse) GetDraftOk() (*Draft, bool)`

GetDraftOk returns a tuple with the Draft field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDraft

`func (o *DraftResponse) SetDraft(v Draft)`

SetDraft sets Draft field to given value.


### GetProvider

`func (o *DraftResponse) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *DraftResponse) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *DraftResponse) SetProvider(v string)`

SetProvider sets Provider field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


