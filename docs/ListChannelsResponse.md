# ListChannelsResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Channels** | Pointer to [**[]Channel**](Channel.md) | &#x60;null&#x60; when no results (Go nil-slice serialization). | [optional] 
**Total** | **int32** |  | 
**NextCursor** | Pointer to **string** |  | [optional] 
**Provider** | **string** |  | 

## Methods

### NewListChannelsResponse

`func NewListChannelsResponse(total int32, provider string, ) *ListChannelsResponse`

NewListChannelsResponse instantiates a new ListChannelsResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewListChannelsResponseWithDefaults

`func NewListChannelsResponseWithDefaults() *ListChannelsResponse`

NewListChannelsResponseWithDefaults instantiates a new ListChannelsResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetChannels

`func (o *ListChannelsResponse) GetChannels() []Channel`

GetChannels returns the Channels field if non-nil, zero value otherwise.

### GetChannelsOk

`func (o *ListChannelsResponse) GetChannelsOk() (*[]Channel, bool)`

GetChannelsOk returns a tuple with the Channels field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChannels

`func (o *ListChannelsResponse) SetChannels(v []Channel)`

SetChannels sets Channels field to given value.

### HasChannels

`func (o *ListChannelsResponse) HasChannels() bool`

HasChannels returns a boolean if a field has been set.

### SetChannelsNil

`func (o *ListChannelsResponse) SetChannelsNil(b bool)`

 SetChannelsNil sets the value for Channels to be an explicit nil

### UnsetChannels
`func (o *ListChannelsResponse) UnsetChannels()`

UnsetChannels ensures that no value is present for Channels, not even an explicit nil
### GetTotal

`func (o *ListChannelsResponse) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *ListChannelsResponse) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *ListChannelsResponse) SetTotal(v int32)`

SetTotal sets Total field to given value.


### GetNextCursor

`func (o *ListChannelsResponse) GetNextCursor() string`

GetNextCursor returns the NextCursor field if non-nil, zero value otherwise.

### GetNextCursorOk

`func (o *ListChannelsResponse) GetNextCursorOk() (*string, bool)`

GetNextCursorOk returns a tuple with the NextCursor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextCursor

`func (o *ListChannelsResponse) SetNextCursor(v string)`

SetNextCursor sets NextCursor field to given value.

### HasNextCursor

`func (o *ListChannelsResponse) HasNextCursor() bool`

HasNextCursor returns a boolean if a field has been set.

### GetProvider

`func (o *ListChannelsResponse) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *ListChannelsResponse) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *ListChannelsResponse) SetProvider(v string)`

SetProvider sets Provider field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


