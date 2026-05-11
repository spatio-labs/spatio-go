# ListCalendarEvents200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | **bool** |  | 
**Data** | Pointer to [**ListEventsData**](ListEventsData.md) |  | [optional] 
**Errors** | Pointer to [**[]CalendarAccountError**](CalendarAccountError.md) |  | [optional] 
**Metadata** | Pointer to **map[string]interface{}** |  | [optional] 

## Methods

### NewListCalendarEvents200Response

`func NewListCalendarEvents200Response(success bool, ) *ListCalendarEvents200Response`

NewListCalendarEvents200Response instantiates a new ListCalendarEvents200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewListCalendarEvents200ResponseWithDefaults

`func NewListCalendarEvents200ResponseWithDefaults() *ListCalendarEvents200Response`

NewListCalendarEvents200ResponseWithDefaults instantiates a new ListCalendarEvents200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *ListCalendarEvents200Response) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *ListCalendarEvents200Response) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *ListCalendarEvents200Response) SetSuccess(v bool)`

SetSuccess sets Success field to given value.


### GetData

`func (o *ListCalendarEvents200Response) GetData() ListEventsData`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *ListCalendarEvents200Response) GetDataOk() (*ListEventsData, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *ListCalendarEvents200Response) SetData(v ListEventsData)`

SetData sets Data field to given value.

### HasData

`func (o *ListCalendarEvents200Response) HasData() bool`

HasData returns a boolean if a field has been set.

### GetErrors

`func (o *ListCalendarEvents200Response) GetErrors() []CalendarAccountError`

GetErrors returns the Errors field if non-nil, zero value otherwise.

### GetErrorsOk

`func (o *ListCalendarEvents200Response) GetErrorsOk() (*[]CalendarAccountError, bool)`

GetErrorsOk returns a tuple with the Errors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrors

`func (o *ListCalendarEvents200Response) SetErrors(v []CalendarAccountError)`

SetErrors sets Errors field to given value.

### HasErrors

`func (o *ListCalendarEvents200Response) HasErrors() bool`

HasErrors returns a boolean if a field has been set.

### GetMetadata

`func (o *ListCalendarEvents200Response) GetMetadata() map[string]interface{}`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *ListCalendarEvents200Response) GetMetadataOk() (*map[string]interface{}, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *ListCalendarEvents200Response) SetMetadata(v map[string]interface{})`

SetMetadata sets Metadata field to given value.

### HasMetadata

`func (o *ListCalendarEvents200Response) HasMetadata() bool`

HasMetadata returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


