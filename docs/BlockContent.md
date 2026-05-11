# BlockContent

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**RichText** | Pointer to [**[]RichTextObject**](RichTextObject.md) |  | [optional] 
**Language** | Pointer to **string** | Programming language for &#x60;code&#x60; blocks. | [optional] 
**Checked** | Pointer to **bool** | Toggle state for &#x60;to_do&#x60; blocks. | [optional] 
**Icon** | Pointer to **string** | Emoji or short string for &#x60;callout&#x60; blocks. | [optional] 
**Color** | Pointer to **string** | Theme color for &#x60;callout&#x60; blocks. | [optional] 
**Url** | Pointer to **string** | Source URL for &#x60;image&#x60;, &#x60;video&#x60;, &#x60;file&#x60; blocks. | [optional] 
**Caption** | Pointer to **string** | Visible caption for media blocks. | [optional] 
**AltText** | Pointer to **string** | Screen-reader description for media blocks. Distinct from &#x60;caption&#x60; (visible to readers) — required for accessible notes when the image conveys meaning.  | [optional] 
**EmbedUrl** | Pointer to **string** | Source URL for &#x60;embed&#x60; blocks. | [optional] 
**Cells** | Pointer to [**[][]RichTextObject**]([]RichTextObject.md) | 2D rich-text grid for &#x60;table&#x60; and &#x60;table_row&#x60; blocks. | [optional] 
**Expression** | Pointer to **string** | TeX/MathJax expression for &#x60;equation&#x60; blocks. | [optional] 

## Methods

### NewBlockContent

`func NewBlockContent() *BlockContent`

NewBlockContent instantiates a new BlockContent object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBlockContentWithDefaults

`func NewBlockContentWithDefaults() *BlockContent`

NewBlockContentWithDefaults instantiates a new BlockContent object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRichText

`func (o *BlockContent) GetRichText() []RichTextObject`

GetRichText returns the RichText field if non-nil, zero value otherwise.

### GetRichTextOk

`func (o *BlockContent) GetRichTextOk() (*[]RichTextObject, bool)`

GetRichTextOk returns a tuple with the RichText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRichText

`func (o *BlockContent) SetRichText(v []RichTextObject)`

SetRichText sets RichText field to given value.

### HasRichText

`func (o *BlockContent) HasRichText() bool`

HasRichText returns a boolean if a field has been set.

### GetLanguage

`func (o *BlockContent) GetLanguage() string`

GetLanguage returns the Language field if non-nil, zero value otherwise.

### GetLanguageOk

`func (o *BlockContent) GetLanguageOk() (*string, bool)`

GetLanguageOk returns a tuple with the Language field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLanguage

`func (o *BlockContent) SetLanguage(v string)`

SetLanguage sets Language field to given value.

### HasLanguage

`func (o *BlockContent) HasLanguage() bool`

HasLanguage returns a boolean if a field has been set.

### GetChecked

`func (o *BlockContent) GetChecked() bool`

GetChecked returns the Checked field if non-nil, zero value otherwise.

### GetCheckedOk

`func (o *BlockContent) GetCheckedOk() (*bool, bool)`

GetCheckedOk returns a tuple with the Checked field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChecked

`func (o *BlockContent) SetChecked(v bool)`

SetChecked sets Checked field to given value.

### HasChecked

`func (o *BlockContent) HasChecked() bool`

HasChecked returns a boolean if a field has been set.

### GetIcon

`func (o *BlockContent) GetIcon() string`

GetIcon returns the Icon field if non-nil, zero value otherwise.

### GetIconOk

`func (o *BlockContent) GetIconOk() (*string, bool)`

GetIconOk returns a tuple with the Icon field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIcon

`func (o *BlockContent) SetIcon(v string)`

SetIcon sets Icon field to given value.

### HasIcon

`func (o *BlockContent) HasIcon() bool`

HasIcon returns a boolean if a field has been set.

### GetColor

`func (o *BlockContent) GetColor() string`

GetColor returns the Color field if non-nil, zero value otherwise.

### GetColorOk

`func (o *BlockContent) GetColorOk() (*string, bool)`

GetColorOk returns a tuple with the Color field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetColor

`func (o *BlockContent) SetColor(v string)`

SetColor sets Color field to given value.

### HasColor

`func (o *BlockContent) HasColor() bool`

HasColor returns a boolean if a field has been set.

### GetUrl

`func (o *BlockContent) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *BlockContent) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *BlockContent) SetUrl(v string)`

SetUrl sets Url field to given value.

### HasUrl

`func (o *BlockContent) HasUrl() bool`

HasUrl returns a boolean if a field has been set.

### GetCaption

`func (o *BlockContent) GetCaption() string`

GetCaption returns the Caption field if non-nil, zero value otherwise.

### GetCaptionOk

`func (o *BlockContent) GetCaptionOk() (*string, bool)`

GetCaptionOk returns a tuple with the Caption field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCaption

`func (o *BlockContent) SetCaption(v string)`

SetCaption sets Caption field to given value.

### HasCaption

`func (o *BlockContent) HasCaption() bool`

HasCaption returns a boolean if a field has been set.

### GetAltText

`func (o *BlockContent) GetAltText() string`

GetAltText returns the AltText field if non-nil, zero value otherwise.

### GetAltTextOk

`func (o *BlockContent) GetAltTextOk() (*string, bool)`

GetAltTextOk returns a tuple with the AltText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAltText

`func (o *BlockContent) SetAltText(v string)`

SetAltText sets AltText field to given value.

### HasAltText

`func (o *BlockContent) HasAltText() bool`

HasAltText returns a boolean if a field has been set.

### GetEmbedUrl

`func (o *BlockContent) GetEmbedUrl() string`

GetEmbedUrl returns the EmbedUrl field if non-nil, zero value otherwise.

### GetEmbedUrlOk

`func (o *BlockContent) GetEmbedUrlOk() (*string, bool)`

GetEmbedUrlOk returns a tuple with the EmbedUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmbedUrl

`func (o *BlockContent) SetEmbedUrl(v string)`

SetEmbedUrl sets EmbedUrl field to given value.

### HasEmbedUrl

`func (o *BlockContent) HasEmbedUrl() bool`

HasEmbedUrl returns a boolean if a field has been set.

### GetCells

`func (o *BlockContent) GetCells() [][]RichTextObject`

GetCells returns the Cells field if non-nil, zero value otherwise.

### GetCellsOk

`func (o *BlockContent) GetCellsOk() (*[][]RichTextObject, bool)`

GetCellsOk returns a tuple with the Cells field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCells

`func (o *BlockContent) SetCells(v [][]RichTextObject)`

SetCells sets Cells field to given value.

### HasCells

`func (o *BlockContent) HasCells() bool`

HasCells returns a boolean if a field has been set.

### GetExpression

`func (o *BlockContent) GetExpression() string`

GetExpression returns the Expression field if non-nil, zero value otherwise.

### GetExpressionOk

`func (o *BlockContent) GetExpressionOk() (*string, bool)`

GetExpressionOk returns a tuple with the Expression field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpression

`func (o *BlockContent) SetExpression(v string)`

SetExpression sets Expression field to given value.

### HasExpression

`func (o *BlockContent) HasExpression() bool`

HasExpression returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


