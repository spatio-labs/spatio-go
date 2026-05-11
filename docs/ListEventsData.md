# ListEventsData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Events** | Pointer to [**[]SpatioEvent**](SpatioEvent.md) | &#x60;null&#x60; when there are no results (Go nil-slice serialization).  | [optional] 
**NextPageToken** | Pointer to **string** |  | [optional] 
**TotalResults** | Pointer to **int32** |  | [optional] 
**UpdatedAt** | **time.Time** |  | 

## Methods

### NewListEventsData

`func NewListEventsData(updatedAt time.Time, ) *ListEventsData`

NewListEventsData instantiates a new ListEventsData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewListEventsDataWithDefaults

`func NewListEventsDataWithDefaults() *ListEventsData`

NewListEventsDataWithDefaults instantiates a new ListEventsData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEvents

`func (o *ListEventsData) GetEvents() []SpatioEvent`

GetEvents returns the Events field if non-nil, zero value otherwise.

### GetEventsOk

`func (o *ListEventsData) GetEventsOk() (*[]SpatioEvent, bool)`

GetEventsOk returns a tuple with the Events field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEvents

`func (o *ListEventsData) SetEvents(v []SpatioEvent)`

SetEvents sets Events field to given value.

### HasEvents

`func (o *ListEventsData) HasEvents() bool`

HasEvents returns a boolean if a field has been set.

### SetEventsNil

`func (o *ListEventsData) SetEventsNil(b bool)`

 SetEventsNil sets the value for Events to be an explicit nil

### UnsetEvents
`func (o *ListEventsData) UnsetEvents()`

UnsetEvents ensures that no value is present for Events, not even an explicit nil
### GetNextPageToken

`func (o *ListEventsData) GetNextPageToken() string`

GetNextPageToken returns the NextPageToken field if non-nil, zero value otherwise.

### GetNextPageTokenOk

`func (o *ListEventsData) GetNextPageTokenOk() (*string, bool)`

GetNextPageTokenOk returns a tuple with the NextPageToken field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextPageToken

`func (o *ListEventsData) SetNextPageToken(v string)`

SetNextPageToken sets NextPageToken field to given value.

### HasNextPageToken

`func (o *ListEventsData) HasNextPageToken() bool`

HasNextPageToken returns a boolean if a field has been set.

### GetTotalResults

`func (o *ListEventsData) GetTotalResults() int32`

GetTotalResults returns the TotalResults field if non-nil, zero value otherwise.

### GetTotalResultsOk

`func (o *ListEventsData) GetTotalResultsOk() (*int32, bool)`

GetTotalResultsOk returns a tuple with the TotalResults field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalResults

`func (o *ListEventsData) SetTotalResults(v int32)`

SetTotalResults sets TotalResults field to given value.

### HasTotalResults

`func (o *ListEventsData) HasTotalResults() bool`

HasTotalResults returns a boolean if a field has been set.

### GetUpdatedAt

`func (o *ListEventsData) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *ListEventsData) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *ListEventsData) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


