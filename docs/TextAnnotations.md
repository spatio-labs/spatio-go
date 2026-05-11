# TextAnnotations

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Bold** | **bool** |  | 
**Italic** | **bool** |  | 
**Strikethrough** | **bool** |  | 
**Underline** | **bool** |  | 
**Code** | **bool** |  | 
**Color** | Pointer to **string** |  | [optional] 

## Methods

### NewTextAnnotations

`func NewTextAnnotations(bold bool, italic bool, strikethrough bool, underline bool, code bool, ) *TextAnnotations`

NewTextAnnotations instantiates a new TextAnnotations object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTextAnnotationsWithDefaults

`func NewTextAnnotationsWithDefaults() *TextAnnotations`

NewTextAnnotationsWithDefaults instantiates a new TextAnnotations object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBold

`func (o *TextAnnotations) GetBold() bool`

GetBold returns the Bold field if non-nil, zero value otherwise.

### GetBoldOk

`func (o *TextAnnotations) GetBoldOk() (*bool, bool)`

GetBoldOk returns a tuple with the Bold field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBold

`func (o *TextAnnotations) SetBold(v bool)`

SetBold sets Bold field to given value.


### GetItalic

`func (o *TextAnnotations) GetItalic() bool`

GetItalic returns the Italic field if non-nil, zero value otherwise.

### GetItalicOk

`func (o *TextAnnotations) GetItalicOk() (*bool, bool)`

GetItalicOk returns a tuple with the Italic field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItalic

`func (o *TextAnnotations) SetItalic(v bool)`

SetItalic sets Italic field to given value.


### GetStrikethrough

`func (o *TextAnnotations) GetStrikethrough() bool`

GetStrikethrough returns the Strikethrough field if non-nil, zero value otherwise.

### GetStrikethroughOk

`func (o *TextAnnotations) GetStrikethroughOk() (*bool, bool)`

GetStrikethroughOk returns a tuple with the Strikethrough field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStrikethrough

`func (o *TextAnnotations) SetStrikethrough(v bool)`

SetStrikethrough sets Strikethrough field to given value.


### GetUnderline

`func (o *TextAnnotations) GetUnderline() bool`

GetUnderline returns the Underline field if non-nil, zero value otherwise.

### GetUnderlineOk

`func (o *TextAnnotations) GetUnderlineOk() (*bool, bool)`

GetUnderlineOk returns a tuple with the Underline field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnderline

`func (o *TextAnnotations) SetUnderline(v bool)`

SetUnderline sets Underline field to given value.


### GetCode

`func (o *TextAnnotations) GetCode() bool`

GetCode returns the Code field if non-nil, zero value otherwise.

### GetCodeOk

`func (o *TextAnnotations) GetCodeOk() (*bool, bool)`

GetCodeOk returns a tuple with the Code field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCode

`func (o *TextAnnotations) SetCode(v bool)`

SetCode sets Code field to given value.


### GetColor

`func (o *TextAnnotations) GetColor() string`

GetColor returns the Color field if non-nil, zero value otherwise.

### GetColorOk

`func (o *TextAnnotations) GetColorOk() (*string, bool)`

GetColorOk returns a tuple with the Color field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetColor

`func (o *TextAnnotations) SetColor(v string)`

SetColor sets Color field to given value.

### HasColor

`func (o *TextAnnotations) HasColor() bool`

HasColor returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


