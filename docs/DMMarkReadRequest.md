# DMMarkReadRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**MessageId** | **string** |  | 
**AccountId** | Pointer to **string** |  | [optional] 

## Methods

### NewDMMarkReadRequest

`func NewDMMarkReadRequest(messageId string, ) *DMMarkReadRequest`

NewDMMarkReadRequest instantiates a new DMMarkReadRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDMMarkReadRequestWithDefaults

`func NewDMMarkReadRequestWithDefaults() *DMMarkReadRequest`

NewDMMarkReadRequestWithDefaults instantiates a new DMMarkReadRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMessageId

`func (o *DMMarkReadRequest) GetMessageId() string`

GetMessageId returns the MessageId field if non-nil, zero value otherwise.

### GetMessageIdOk

`func (o *DMMarkReadRequest) GetMessageIdOk() (*string, bool)`

GetMessageIdOk returns a tuple with the MessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageId

`func (o *DMMarkReadRequest) SetMessageId(v string)`

SetMessageId sets MessageId field to given value.


### GetAccountId

`func (o *DMMarkReadRequest) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *DMMarkReadRequest) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *DMMarkReadRequest) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *DMMarkReadRequest) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


