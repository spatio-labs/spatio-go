# ExtractTextResult

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Text** | **string** |  | 
**PageCount** | **int32** |  | 
**Pages** | Pointer to **[]map[string]interface{}** |  | [optional] 
**Truncated** | Pointer to **bool** | &#x60;true&#x60; when &#x60;maxChars&#x60; was hit before the end. | [optional] 

## Methods

### NewExtractTextResult

`func NewExtractTextResult(text string, pageCount int32, ) *ExtractTextResult`

NewExtractTextResult instantiates a new ExtractTextResult object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewExtractTextResultWithDefaults

`func NewExtractTextResultWithDefaults() *ExtractTextResult`

NewExtractTextResultWithDefaults instantiates a new ExtractTextResult object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetText

`func (o *ExtractTextResult) GetText() string`

GetText returns the Text field if non-nil, zero value otherwise.

### GetTextOk

`func (o *ExtractTextResult) GetTextOk() (*string, bool)`

GetTextOk returns a tuple with the Text field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetText

`func (o *ExtractTextResult) SetText(v string)`

SetText sets Text field to given value.


### GetPageCount

`func (o *ExtractTextResult) GetPageCount() int32`

GetPageCount returns the PageCount field if non-nil, zero value otherwise.

### GetPageCountOk

`func (o *ExtractTextResult) GetPageCountOk() (*int32, bool)`

GetPageCountOk returns a tuple with the PageCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPageCount

`func (o *ExtractTextResult) SetPageCount(v int32)`

SetPageCount sets PageCount field to given value.


### GetPages

`func (o *ExtractTextResult) GetPages() []map[string]interface{}`

GetPages returns the Pages field if non-nil, zero value otherwise.

### GetPagesOk

`func (o *ExtractTextResult) GetPagesOk() (*[]map[string]interface{}, bool)`

GetPagesOk returns a tuple with the Pages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPages

`func (o *ExtractTextResult) SetPages(v []map[string]interface{})`

SetPages sets Pages field to given value.

### HasPages

`func (o *ExtractTextResult) HasPages() bool`

HasPages returns a boolean if a field has been set.

### GetTruncated

`func (o *ExtractTextResult) GetTruncated() bool`

GetTruncated returns the Truncated field if non-nil, zero value otherwise.

### GetTruncatedOk

`func (o *ExtractTextResult) GetTruncatedOk() (*bool, bool)`

GetTruncatedOk returns a tuple with the Truncated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTruncated

`func (o *ExtractTextResult) SetTruncated(v bool)`

SetTruncated sets Truncated field to given value.

### HasTruncated

`func (o *ExtractTextResult) HasTruncated() bool`

HasTruncated returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


