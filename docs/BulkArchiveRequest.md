# BulkArchiveRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AccountId** | Pointer to **string** |  | [optional] 
**MessageIds** | **[]string** |  | 

## Methods

### NewBulkArchiveRequest

`func NewBulkArchiveRequest(messageIds []string, ) *BulkArchiveRequest`

NewBulkArchiveRequest instantiates a new BulkArchiveRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBulkArchiveRequestWithDefaults

`func NewBulkArchiveRequestWithDefaults() *BulkArchiveRequest`

NewBulkArchiveRequestWithDefaults instantiates a new BulkArchiveRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAccountId

`func (o *BulkArchiveRequest) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *BulkArchiveRequest) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *BulkArchiveRequest) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *BulkArchiveRequest) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.

### GetMessageIds

`func (o *BulkArchiveRequest) GetMessageIds() []string`

GetMessageIds returns the MessageIds field if non-nil, zero value otherwise.

### GetMessageIdsOk

`func (o *BulkArchiveRequest) GetMessageIdsOk() (*[]string, bool)`

GetMessageIdsOk returns a tuple with the MessageIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageIds

`func (o *BulkArchiveRequest) SetMessageIds(v []string)`

SetMessageIds sets MessageIds field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


