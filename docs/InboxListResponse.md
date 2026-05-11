# InboxListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Items** | [**[]InboxItem**](InboxItem.md) |  | 
**TotalCount** | **int32** |  | 
**HasMore** | **bool** |  | 

## Methods

### NewInboxListResponse

`func NewInboxListResponse(items []InboxItem, totalCount int32, hasMore bool, ) *InboxListResponse`

NewInboxListResponse instantiates a new InboxListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInboxListResponseWithDefaults

`func NewInboxListResponseWithDefaults() *InboxListResponse`

NewInboxListResponseWithDefaults instantiates a new InboxListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetItems

`func (o *InboxListResponse) GetItems() []InboxItem`

GetItems returns the Items field if non-nil, zero value otherwise.

### GetItemsOk

`func (o *InboxListResponse) GetItemsOk() (*[]InboxItem, bool)`

GetItemsOk returns a tuple with the Items field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItems

`func (o *InboxListResponse) SetItems(v []InboxItem)`

SetItems sets Items field to given value.


### GetTotalCount

`func (o *InboxListResponse) GetTotalCount() int32`

GetTotalCount returns the TotalCount field if non-nil, zero value otherwise.

### GetTotalCountOk

`func (o *InboxListResponse) GetTotalCountOk() (*int32, bool)`

GetTotalCountOk returns a tuple with the TotalCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalCount

`func (o *InboxListResponse) SetTotalCount(v int32)`

SetTotalCount sets TotalCount field to given value.


### GetHasMore

`func (o *InboxListResponse) GetHasMore() bool`

GetHasMore returns the HasMore field if non-nil, zero value otherwise.

### GetHasMoreOk

`func (o *InboxListResponse) GetHasMoreOk() (*bool, bool)`

GetHasMoreOk returns a tuple with the HasMore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasMore

`func (o *InboxListResponse) SetHasMore(v bool)`

SetHasMore sets HasMore field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


