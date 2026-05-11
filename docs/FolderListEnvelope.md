# FolderListEnvelope

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Items** | [**[]Folder**](Folder.md) |  | 
**Accounts** | [**[]AccountStatus**](AccountStatus.md) |  | 

## Methods

### NewFolderListEnvelope

`func NewFolderListEnvelope(items []Folder, accounts []AccountStatus, ) *FolderListEnvelope`

NewFolderListEnvelope instantiates a new FolderListEnvelope object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewFolderListEnvelopeWithDefaults

`func NewFolderListEnvelopeWithDefaults() *FolderListEnvelope`

NewFolderListEnvelopeWithDefaults instantiates a new FolderListEnvelope object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetItems

`func (o *FolderListEnvelope) GetItems() []Folder`

GetItems returns the Items field if non-nil, zero value otherwise.

### GetItemsOk

`func (o *FolderListEnvelope) GetItemsOk() (*[]Folder, bool)`

GetItemsOk returns a tuple with the Items field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItems

`func (o *FolderListEnvelope) SetItems(v []Folder)`

SetItems sets Items field to given value.


### SetItemsNil

`func (o *FolderListEnvelope) SetItemsNil(b bool)`

 SetItemsNil sets the value for Items to be an explicit nil

### UnsetItems
`func (o *FolderListEnvelope) UnsetItems()`

UnsetItems ensures that no value is present for Items, not even an explicit nil
### GetAccounts

`func (o *FolderListEnvelope) GetAccounts() []AccountStatus`

GetAccounts returns the Accounts field if non-nil, zero value otherwise.

### GetAccountsOk

`func (o *FolderListEnvelope) GetAccountsOk() (*[]AccountStatus, bool)`

GetAccountsOk returns a tuple with the Accounts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccounts

`func (o *FolderListEnvelope) SetAccounts(v []AccountStatus)`

SetAccounts sets Accounts field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


