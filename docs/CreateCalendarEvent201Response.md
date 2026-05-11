# CreateCalendarEvent201Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | **bool** |  | 
**Data** | Pointer to [**SpatioEvent**](SpatioEvent.md) |  | [optional] 
**Errors** | Pointer to [**[]CalendarAccountError**](CalendarAccountError.md) |  | [optional] 
**Metadata** | Pointer to **map[string]interface{}** |  | [optional] 

## Methods

### NewCreateCalendarEvent201Response

`func NewCreateCalendarEvent201Response(success bool, ) *CreateCalendarEvent201Response`

NewCreateCalendarEvent201Response instantiates a new CreateCalendarEvent201Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateCalendarEvent201ResponseWithDefaults

`func NewCreateCalendarEvent201ResponseWithDefaults() *CreateCalendarEvent201Response`

NewCreateCalendarEvent201ResponseWithDefaults instantiates a new CreateCalendarEvent201Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *CreateCalendarEvent201Response) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *CreateCalendarEvent201Response) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *CreateCalendarEvent201Response) SetSuccess(v bool)`

SetSuccess sets Success field to given value.


### GetData

`func (o *CreateCalendarEvent201Response) GetData() SpatioEvent`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *CreateCalendarEvent201Response) GetDataOk() (*SpatioEvent, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *CreateCalendarEvent201Response) SetData(v SpatioEvent)`

SetData sets Data field to given value.

### HasData

`func (o *CreateCalendarEvent201Response) HasData() bool`

HasData returns a boolean if a field has been set.

### GetErrors

`func (o *CreateCalendarEvent201Response) GetErrors() []CalendarAccountError`

GetErrors returns the Errors field if non-nil, zero value otherwise.

### GetErrorsOk

`func (o *CreateCalendarEvent201Response) GetErrorsOk() (*[]CalendarAccountError, bool)`

GetErrorsOk returns a tuple with the Errors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrors

`func (o *CreateCalendarEvent201Response) SetErrors(v []CalendarAccountError)`

SetErrors sets Errors field to given value.

### HasErrors

`func (o *CreateCalendarEvent201Response) HasErrors() bool`

HasErrors returns a boolean if a field has been set.

### GetMetadata

`func (o *CreateCalendarEvent201Response) GetMetadata() map[string]interface{}`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *CreateCalendarEvent201Response) GetMetadataOk() (*map[string]interface{}, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *CreateCalendarEvent201Response) SetMetadata(v map[string]interface{})`

SetMetadata sets Metadata field to given value.

### HasMetadata

`func (o *CreateCalendarEvent201Response) HasMetadata() bool`

HasMetadata returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


