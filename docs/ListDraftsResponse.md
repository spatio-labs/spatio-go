# ListDraftsResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Drafts** | [**[]Draft**](Draft.md) |  | 
**Total** | **int32** |  | 
**NextPageToken** | Pointer to **string** |  | [optional] 
**Provider** | **string** |  | 

## Methods

### NewListDraftsResponse

`func NewListDraftsResponse(drafts []Draft, total int32, provider string, ) *ListDraftsResponse`

NewListDraftsResponse instantiates a new ListDraftsResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewListDraftsResponseWithDefaults

`func NewListDraftsResponseWithDefaults() *ListDraftsResponse`

NewListDraftsResponseWithDefaults instantiates a new ListDraftsResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDrafts

`func (o *ListDraftsResponse) GetDrafts() []Draft`

GetDrafts returns the Drafts field if non-nil, zero value otherwise.

### GetDraftsOk

`func (o *ListDraftsResponse) GetDraftsOk() (*[]Draft, bool)`

GetDraftsOk returns a tuple with the Drafts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDrafts

`func (o *ListDraftsResponse) SetDrafts(v []Draft)`

SetDrafts sets Drafts field to given value.


### GetTotal

`func (o *ListDraftsResponse) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *ListDraftsResponse) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *ListDraftsResponse) SetTotal(v int32)`

SetTotal sets Total field to given value.


### GetNextPageToken

`func (o *ListDraftsResponse) GetNextPageToken() string`

GetNextPageToken returns the NextPageToken field if non-nil, zero value otherwise.

### GetNextPageTokenOk

`func (o *ListDraftsResponse) GetNextPageTokenOk() (*string, bool)`

GetNextPageTokenOk returns a tuple with the NextPageToken field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextPageToken

`func (o *ListDraftsResponse) SetNextPageToken(v string)`

SetNextPageToken sets NextPageToken field to given value.

### HasNextPageToken

`func (o *ListDraftsResponse) HasNextPageToken() bool`

HasNextPageToken returns a boolean if a field has been set.

### GetProvider

`func (o *ListDraftsResponse) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *ListDraftsResponse) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *ListDraftsResponse) SetProvider(v string)`

SetProvider sets Provider field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


