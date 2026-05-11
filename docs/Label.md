# Label

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Name** | **string** |  | 
**Type** | **string** | Provider-specific label type. Common values: &#x60;system&#x60;, &#x60;user&#x60;. Not enumerated to avoid forcing a breaking change every time a provider adds one.  | 
**MessageListVisibility** | Pointer to **string** |  | [optional] 
**LabelListVisibility** | Pointer to **string** |  | [optional] 
**Color** | Pointer to [**LabelColor**](LabelColor.md) |  | [optional] 

## Methods

### NewLabel

`func NewLabel(id string, name string, type_ string, ) *Label`

NewLabel instantiates a new Label object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewLabelWithDefaults

`func NewLabelWithDefaults() *Label`

NewLabelWithDefaults instantiates a new Label object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Label) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Label) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Label) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *Label) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Label) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Label) SetName(v string)`

SetName sets Name field to given value.


### GetType

`func (o *Label) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *Label) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *Label) SetType(v string)`

SetType sets Type field to given value.


### GetMessageListVisibility

`func (o *Label) GetMessageListVisibility() string`

GetMessageListVisibility returns the MessageListVisibility field if non-nil, zero value otherwise.

### GetMessageListVisibilityOk

`func (o *Label) GetMessageListVisibilityOk() (*string, bool)`

GetMessageListVisibilityOk returns a tuple with the MessageListVisibility field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageListVisibility

`func (o *Label) SetMessageListVisibility(v string)`

SetMessageListVisibility sets MessageListVisibility field to given value.

### HasMessageListVisibility

`func (o *Label) HasMessageListVisibility() bool`

HasMessageListVisibility returns a boolean if a field has been set.

### GetLabelListVisibility

`func (o *Label) GetLabelListVisibility() string`

GetLabelListVisibility returns the LabelListVisibility field if non-nil, zero value otherwise.

### GetLabelListVisibilityOk

`func (o *Label) GetLabelListVisibilityOk() (*string, bool)`

GetLabelListVisibilityOk returns a tuple with the LabelListVisibility field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabelListVisibility

`func (o *Label) SetLabelListVisibility(v string)`

SetLabelListVisibility sets LabelListVisibility field to given value.

### HasLabelListVisibility

`func (o *Label) HasLabelListVisibility() bool`

HasLabelListVisibility returns a boolean if a field has been set.

### GetColor

`func (o *Label) GetColor() LabelColor`

GetColor returns the Color field if non-nil, zero value otherwise.

### GetColorOk

`func (o *Label) GetColorOk() (*LabelColor, bool)`

GetColorOk returns a tuple with the Color field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetColor

`func (o *Label) SetColor(v LabelColor)`

SetColor sets Color field to given value.

### HasColor

`func (o *Label) HasColor() bool`

HasColor returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


