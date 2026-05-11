# DMReactionRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Emoji** | **string** |  | 
**AccountId** | Pointer to **string** |  | [optional] 

## Methods

### NewDMReactionRequest

`func NewDMReactionRequest(emoji string, ) *DMReactionRequest`

NewDMReactionRequest instantiates a new DMReactionRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDMReactionRequestWithDefaults

`func NewDMReactionRequestWithDefaults() *DMReactionRequest`

NewDMReactionRequestWithDefaults instantiates a new DMReactionRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEmoji

`func (o *DMReactionRequest) GetEmoji() string`

GetEmoji returns the Emoji field if non-nil, zero value otherwise.

### GetEmojiOk

`func (o *DMReactionRequest) GetEmojiOk() (*string, bool)`

GetEmojiOk returns a tuple with the Emoji field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmoji

`func (o *DMReactionRequest) SetEmoji(v string)`

SetEmoji sets Emoji field to given value.


### GetAccountId

`func (o *DMReactionRequest) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *DMReactionRequest) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *DMReactionRequest) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *DMReactionRequest) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


