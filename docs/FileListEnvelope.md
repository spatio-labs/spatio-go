# FileListEnvelope

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Items** | [**[]SpatioFile**](SpatioFile.md) |  | 
**Accounts** | [**[]AccountStatus**](AccountStatus.md) |  | 

## Methods

### NewFileListEnvelope

`func NewFileListEnvelope(items []SpatioFile, accounts []AccountStatus, ) *FileListEnvelope`

NewFileListEnvelope instantiates a new FileListEnvelope object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewFileListEnvelopeWithDefaults

`func NewFileListEnvelopeWithDefaults() *FileListEnvelope`

NewFileListEnvelopeWithDefaults instantiates a new FileListEnvelope object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetItems

`func (o *FileListEnvelope) GetItems() []SpatioFile`

GetItems returns the Items field if non-nil, zero value otherwise.

### GetItemsOk

`func (o *FileListEnvelope) GetItemsOk() (*[]SpatioFile, bool)`

GetItemsOk returns a tuple with the Items field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItems

`func (o *FileListEnvelope) SetItems(v []SpatioFile)`

SetItems sets Items field to given value.


### SetItemsNil

`func (o *FileListEnvelope) SetItemsNil(b bool)`

 SetItemsNil sets the value for Items to be an explicit nil

### UnsetItems
`func (o *FileListEnvelope) UnsetItems()`

UnsetItems ensures that no value is present for Items, not even an explicit nil
### GetAccounts

`func (o *FileListEnvelope) GetAccounts() []AccountStatus`

GetAccounts returns the Accounts field if non-nil, zero value otherwise.

### GetAccountsOk

`func (o *FileListEnvelope) GetAccountsOk() (*[]AccountStatus, bool)`

GetAccountsOk returns a tuple with the Accounts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccounts

`func (o *FileListEnvelope) SetAccounts(v []AccountStatus)`

SetAccounts sets Accounts field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


