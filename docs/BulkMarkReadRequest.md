# BulkMarkReadRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AccountId** | Pointer to **string** |  | [optional] 
**MessageIds** | **[]string** |  | 
**Read** | Pointer to **bool** |  | [optional] [default to true]

## Methods

### NewBulkMarkReadRequest

`func NewBulkMarkReadRequest(messageIds []string, ) *BulkMarkReadRequest`

NewBulkMarkReadRequest instantiates a new BulkMarkReadRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBulkMarkReadRequestWithDefaults

`func NewBulkMarkReadRequestWithDefaults() *BulkMarkReadRequest`

NewBulkMarkReadRequestWithDefaults instantiates a new BulkMarkReadRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAccountId

`func (o *BulkMarkReadRequest) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *BulkMarkReadRequest) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *BulkMarkReadRequest) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *BulkMarkReadRequest) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.

### GetMessageIds

`func (o *BulkMarkReadRequest) GetMessageIds() []string`

GetMessageIds returns the MessageIds field if non-nil, zero value otherwise.

### GetMessageIdsOk

`func (o *BulkMarkReadRequest) GetMessageIdsOk() (*[]string, bool)`

GetMessageIdsOk returns a tuple with the MessageIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageIds

`func (o *BulkMarkReadRequest) SetMessageIds(v []string)`

SetMessageIds sets MessageIds field to given value.


### GetRead

`func (o *BulkMarkReadRequest) GetRead() bool`

GetRead returns the Read field if non-nil, zero value otherwise.

### GetReadOk

`func (o *BulkMarkReadRequest) GetReadOk() (*bool, bool)`

GetReadOk returns a tuple with the Read field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRead

`func (o *BulkMarkReadRequest) SetRead(v bool)`

SetRead sets Read field to given value.

### HasRead

`func (o *BulkMarkReadRequest) HasRead() bool`

HasRead returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


