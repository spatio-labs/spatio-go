# DMMessageEnvelope

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Message** | [**ChatMessage**](ChatMessage.md) |  | 

## Methods

### NewDMMessageEnvelope

`func NewDMMessageEnvelope(message ChatMessage, ) *DMMessageEnvelope`

NewDMMessageEnvelope instantiates a new DMMessageEnvelope object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDMMessageEnvelopeWithDefaults

`func NewDMMessageEnvelopeWithDefaults() *DMMessageEnvelope`

NewDMMessageEnvelopeWithDefaults instantiates a new DMMessageEnvelope object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMessage

`func (o *DMMessageEnvelope) GetMessage() ChatMessage`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *DMMessageEnvelope) GetMessageOk() (*ChatMessage, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *DMMessageEnvelope) SetMessage(v ChatMessage)`

SetMessage sets Message field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


