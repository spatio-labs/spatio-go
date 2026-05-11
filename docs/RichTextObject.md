# RichTextObject

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | **string** |  | 
**Text** | Pointer to **string** |  | [optional] 
**Annotations** | Pointer to [**TextAnnotations**](TextAnnotations.md) |  | [optional] 
**Href** | Pointer to **string** | External URL (&#x60;https://…&#x60;) or internal note anchor (&#x60;#blockId&#x60;, &#x60;#heading-slug&#x60;). Internal anchors resolve to the matching block in the same note.  | [optional] 

## Methods

### NewRichTextObject

`func NewRichTextObject(type_ string, ) *RichTextObject`

NewRichTextObject instantiates a new RichTextObject object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRichTextObjectWithDefaults

`func NewRichTextObjectWithDefaults() *RichTextObject`

NewRichTextObjectWithDefaults instantiates a new RichTextObject object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *RichTextObject) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *RichTextObject) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *RichTextObject) SetType(v string)`

SetType sets Type field to given value.


### GetText

`func (o *RichTextObject) GetText() string`

GetText returns the Text field if non-nil, zero value otherwise.

### GetTextOk

`func (o *RichTextObject) GetTextOk() (*string, bool)`

GetTextOk returns a tuple with the Text field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetText

`func (o *RichTextObject) SetText(v string)`

SetText sets Text field to given value.

### HasText

`func (o *RichTextObject) HasText() bool`

HasText returns a boolean if a field has been set.

### GetAnnotations

`func (o *RichTextObject) GetAnnotations() TextAnnotations`

GetAnnotations returns the Annotations field if non-nil, zero value otherwise.

### GetAnnotationsOk

`func (o *RichTextObject) GetAnnotationsOk() (*TextAnnotations, bool)`

GetAnnotationsOk returns a tuple with the Annotations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAnnotations

`func (o *RichTextObject) SetAnnotations(v TextAnnotations)`

SetAnnotations sets Annotations field to given value.

### HasAnnotations

`func (o *RichTextObject) HasAnnotations() bool`

HasAnnotations returns a boolean if a field has been set.

### GetHref

`func (o *RichTextObject) GetHref() string`

GetHref returns the Href field if non-nil, zero value otherwise.

### GetHrefOk

`func (o *RichTextObject) GetHrefOk() (*string, bool)`

GetHrefOk returns a tuple with the Href field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHref

`func (o *RichTextObject) SetHref(v string)`

SetHref sets Href field to given value.

### HasHref

`func (o *RichTextObject) HasHref() bool`

HasHref returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


