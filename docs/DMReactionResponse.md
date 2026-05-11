# DMReactionResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Reactions** | Pointer to **interface{}** | Updated reaction list for the message. | [optional] 

## Methods

### NewDMReactionResponse

`func NewDMReactionResponse() *DMReactionResponse`

NewDMReactionResponse instantiates a new DMReactionResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDMReactionResponseWithDefaults

`func NewDMReactionResponseWithDefaults() *DMReactionResponse`

NewDMReactionResponseWithDefaults instantiates a new DMReactionResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetReactions

`func (o *DMReactionResponse) GetReactions() interface{}`

GetReactions returns the Reactions field if non-nil, zero value otherwise.

### GetReactionsOk

`func (o *DMReactionResponse) GetReactionsOk() (*interface{}, bool)`

GetReactionsOk returns a tuple with the Reactions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReactions

`func (o *DMReactionResponse) SetReactions(v interface{})`

SetReactions sets Reactions field to given value.

### HasReactions

`func (o *DMReactionResponse) HasReactions() bool`

HasReactions returns a boolean if a field has been set.

### SetReactionsNil

`func (o *DMReactionResponse) SetReactionsNil(b bool)`

 SetReactionsNil sets the value for Reactions to be an explicit nil

### UnsetReactions
`func (o *DMReactionResponse) UnsetReactions()`

UnsetReactions ensures that no value is present for Reactions, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


