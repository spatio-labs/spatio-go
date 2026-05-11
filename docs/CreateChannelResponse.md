# CreateChannelResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Channel** | [**Channel**](Channel.md) |  | 
**Provider** | **string** |  | 

## Methods

### NewCreateChannelResponse

`func NewCreateChannelResponse(channel Channel, provider string, ) *CreateChannelResponse`

NewCreateChannelResponse instantiates a new CreateChannelResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateChannelResponseWithDefaults

`func NewCreateChannelResponseWithDefaults() *CreateChannelResponse`

NewCreateChannelResponseWithDefaults instantiates a new CreateChannelResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetChannel

`func (o *CreateChannelResponse) GetChannel() Channel`

GetChannel returns the Channel field if non-nil, zero value otherwise.

### GetChannelOk

`func (o *CreateChannelResponse) GetChannelOk() (*Channel, bool)`

GetChannelOk returns a tuple with the Channel field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChannel

`func (o *CreateChannelResponse) SetChannel(v Channel)`

SetChannel sets Channel field to given value.


### GetProvider

`func (o *CreateChannelResponse) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *CreateChannelResponse) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *CreateChannelResponse) SetProvider(v string)`

SetProvider sets Provider field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


