# BulkDeleteEmailsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AccountId** | Pointer to **string** |  | [optional] 
**MessageIds** | **[]string** |  | 
**Permanent** | Pointer to **bool** |  | [optional] 

## Methods

### NewBulkDeleteEmailsRequest

`func NewBulkDeleteEmailsRequest(messageIds []string, ) *BulkDeleteEmailsRequest`

NewBulkDeleteEmailsRequest instantiates a new BulkDeleteEmailsRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBulkDeleteEmailsRequestWithDefaults

`func NewBulkDeleteEmailsRequestWithDefaults() *BulkDeleteEmailsRequest`

NewBulkDeleteEmailsRequestWithDefaults instantiates a new BulkDeleteEmailsRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAccountId

`func (o *BulkDeleteEmailsRequest) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *BulkDeleteEmailsRequest) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *BulkDeleteEmailsRequest) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *BulkDeleteEmailsRequest) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.

### GetMessageIds

`func (o *BulkDeleteEmailsRequest) GetMessageIds() []string`

GetMessageIds returns the MessageIds field if non-nil, zero value otherwise.

### GetMessageIdsOk

`func (o *BulkDeleteEmailsRequest) GetMessageIdsOk() (*[]string, bool)`

GetMessageIdsOk returns a tuple with the MessageIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageIds

`func (o *BulkDeleteEmailsRequest) SetMessageIds(v []string)`

SetMessageIds sets MessageIds field to given value.


### GetPermanent

`func (o *BulkDeleteEmailsRequest) GetPermanent() bool`

GetPermanent returns the Permanent field if non-nil, zero value otherwise.

### GetPermanentOk

`func (o *BulkDeleteEmailsRequest) GetPermanentOk() (*bool, bool)`

GetPermanentOk returns a tuple with the Permanent field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPermanent

`func (o *BulkDeleteEmailsRequest) SetPermanent(v bool)`

SetPermanent sets Permanent field to given value.

### HasPermanent

`func (o *BulkDeleteEmailsRequest) HasPermanent() bool`

HasPermanent returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


