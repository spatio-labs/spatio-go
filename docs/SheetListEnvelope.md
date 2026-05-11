# SheetListEnvelope

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Items** | [**[]Sheet**](Sheet.md) |  | 
**Accounts** | [**[]AccountStatus**](AccountStatus.md) |  | 

## Methods

### NewSheetListEnvelope

`func NewSheetListEnvelope(items []Sheet, accounts []AccountStatus, ) *SheetListEnvelope`

NewSheetListEnvelope instantiates a new SheetListEnvelope object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSheetListEnvelopeWithDefaults

`func NewSheetListEnvelopeWithDefaults() *SheetListEnvelope`

NewSheetListEnvelopeWithDefaults instantiates a new SheetListEnvelope object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetItems

`func (o *SheetListEnvelope) GetItems() []Sheet`

GetItems returns the Items field if non-nil, zero value otherwise.

### GetItemsOk

`func (o *SheetListEnvelope) GetItemsOk() (*[]Sheet, bool)`

GetItemsOk returns a tuple with the Items field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItems

`func (o *SheetListEnvelope) SetItems(v []Sheet)`

SetItems sets Items field to given value.


### GetAccounts

`func (o *SheetListEnvelope) GetAccounts() []AccountStatus`

GetAccounts returns the Accounts field if non-nil, zero value otherwise.

### GetAccountsOk

`func (o *SheetListEnvelope) GetAccountsOk() (*[]AccountStatus, bool)`

GetAccountsOk returns a tuple with the Accounts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccounts

`func (o *SheetListEnvelope) SetAccounts(v []AccountStatus)`

SetAccounts sets Accounts field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


