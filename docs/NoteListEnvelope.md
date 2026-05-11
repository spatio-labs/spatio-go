# NoteListEnvelope

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Items** | [**[]Note**](Note.md) |  | 
**Accounts** | [**[]AccountStatus**](AccountStatus.md) |  | 

## Methods

### NewNoteListEnvelope

`func NewNoteListEnvelope(items []Note, accounts []AccountStatus, ) *NoteListEnvelope`

NewNoteListEnvelope instantiates a new NoteListEnvelope object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewNoteListEnvelopeWithDefaults

`func NewNoteListEnvelopeWithDefaults() *NoteListEnvelope`

NewNoteListEnvelopeWithDefaults instantiates a new NoteListEnvelope object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetItems

`func (o *NoteListEnvelope) GetItems() []Note`

GetItems returns the Items field if non-nil, zero value otherwise.

### GetItemsOk

`func (o *NoteListEnvelope) GetItemsOk() (*[]Note, bool)`

GetItemsOk returns a tuple with the Items field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItems

`func (o *NoteListEnvelope) SetItems(v []Note)`

SetItems sets Items field to given value.


### GetAccounts

`func (o *NoteListEnvelope) GetAccounts() []AccountStatus`

GetAccounts returns the Accounts field if non-nil, zero value otherwise.

### GetAccountsOk

`func (o *NoteListEnvelope) GetAccountsOk() (*[]AccountStatus, bool)`

GetAccountsOk returns a tuple with the Accounts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccounts

`func (o *NoteListEnvelope) SetAccounts(v []AccountStatus)`

SetAccounts sets Accounts field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


