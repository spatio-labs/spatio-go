# Slide

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Provider** | Pointer to **string** |  | [optional] 
**AccountId** | Pointer to **string** |  | [optional] 
**PresentationId** | **string** |  | 
**Title** | **string** |  | 
**Notes** | Pointer to **string** | Speaker notes. | [optional] 
**Layout** | Pointer to **string** | Free-form layout id. Provider-specific (&#x60;title&#x60;, &#x60;two-column&#x60;, &#x60;image-left&#x60;, custom). Not enumerated to avoid forcing a breaking change every time a provider adds one.  | [optional] 
**BackgroundColor** | Pointer to **string** |  | [optional] 
**BackgroundImageUrl** | Pointer to **string** |  | [optional] 
**TextColor** | Pointer to **string** |  | [optional] 
**Transition** | Pointer to **string** | Free-form transition id. | [optional] 
**Position** | **int32** | Zero-based position within the presentation. | 
**CreatedAt** | **time.Time** |  | 
**UpdatedAt** | **time.Time** |  | 

## Methods

### NewSlide

`func NewSlide(id string, presentationId string, title string, position int32, createdAt time.Time, updatedAt time.Time, ) *Slide`

NewSlide instantiates a new Slide object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSlideWithDefaults

`func NewSlideWithDefaults() *Slide`

NewSlideWithDefaults instantiates a new Slide object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Slide) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Slide) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Slide) SetId(v string)`

SetId sets Id field to given value.


### GetProvider

`func (o *Slide) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *Slide) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *Slide) SetProvider(v string)`

SetProvider sets Provider field to given value.

### HasProvider

`func (o *Slide) HasProvider() bool`

HasProvider returns a boolean if a field has been set.

### GetAccountId

`func (o *Slide) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *Slide) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *Slide) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *Slide) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.

### GetPresentationId

`func (o *Slide) GetPresentationId() string`

GetPresentationId returns the PresentationId field if non-nil, zero value otherwise.

### GetPresentationIdOk

`func (o *Slide) GetPresentationIdOk() (*string, bool)`

GetPresentationIdOk returns a tuple with the PresentationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPresentationId

`func (o *Slide) SetPresentationId(v string)`

SetPresentationId sets PresentationId field to given value.


### GetTitle

`func (o *Slide) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *Slide) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *Slide) SetTitle(v string)`

SetTitle sets Title field to given value.


### GetNotes

`func (o *Slide) GetNotes() string`

GetNotes returns the Notes field if non-nil, zero value otherwise.

### GetNotesOk

`func (o *Slide) GetNotesOk() (*string, bool)`

GetNotesOk returns a tuple with the Notes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNotes

`func (o *Slide) SetNotes(v string)`

SetNotes sets Notes field to given value.

### HasNotes

`func (o *Slide) HasNotes() bool`

HasNotes returns a boolean if a field has been set.

### GetLayout

`func (o *Slide) GetLayout() string`

GetLayout returns the Layout field if non-nil, zero value otherwise.

### GetLayoutOk

`func (o *Slide) GetLayoutOk() (*string, bool)`

GetLayoutOk returns a tuple with the Layout field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLayout

`func (o *Slide) SetLayout(v string)`

SetLayout sets Layout field to given value.

### HasLayout

`func (o *Slide) HasLayout() bool`

HasLayout returns a boolean if a field has been set.

### GetBackgroundColor

`func (o *Slide) GetBackgroundColor() string`

GetBackgroundColor returns the BackgroundColor field if non-nil, zero value otherwise.

### GetBackgroundColorOk

`func (o *Slide) GetBackgroundColorOk() (*string, bool)`

GetBackgroundColorOk returns a tuple with the BackgroundColor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBackgroundColor

`func (o *Slide) SetBackgroundColor(v string)`

SetBackgroundColor sets BackgroundColor field to given value.

### HasBackgroundColor

`func (o *Slide) HasBackgroundColor() bool`

HasBackgroundColor returns a boolean if a field has been set.

### GetBackgroundImageUrl

`func (o *Slide) GetBackgroundImageUrl() string`

GetBackgroundImageUrl returns the BackgroundImageUrl field if non-nil, zero value otherwise.

### GetBackgroundImageUrlOk

`func (o *Slide) GetBackgroundImageUrlOk() (*string, bool)`

GetBackgroundImageUrlOk returns a tuple with the BackgroundImageUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBackgroundImageUrl

`func (o *Slide) SetBackgroundImageUrl(v string)`

SetBackgroundImageUrl sets BackgroundImageUrl field to given value.

### HasBackgroundImageUrl

`func (o *Slide) HasBackgroundImageUrl() bool`

HasBackgroundImageUrl returns a boolean if a field has been set.

### GetTextColor

`func (o *Slide) GetTextColor() string`

GetTextColor returns the TextColor field if non-nil, zero value otherwise.

### GetTextColorOk

`func (o *Slide) GetTextColorOk() (*string, bool)`

GetTextColorOk returns a tuple with the TextColor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTextColor

`func (o *Slide) SetTextColor(v string)`

SetTextColor sets TextColor field to given value.

### HasTextColor

`func (o *Slide) HasTextColor() bool`

HasTextColor returns a boolean if a field has been set.

### GetTransition

`func (o *Slide) GetTransition() string`

GetTransition returns the Transition field if non-nil, zero value otherwise.

### GetTransitionOk

`func (o *Slide) GetTransitionOk() (*string, bool)`

GetTransitionOk returns a tuple with the Transition field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTransition

`func (o *Slide) SetTransition(v string)`

SetTransition sets Transition field to given value.

### HasTransition

`func (o *Slide) HasTransition() bool`

HasTransition returns a boolean if a field has been set.

### GetPosition

`func (o *Slide) GetPosition() int32`

GetPosition returns the Position field if non-nil, zero value otherwise.

### GetPositionOk

`func (o *Slide) GetPositionOk() (*int32, bool)`

GetPositionOk returns a tuple with the Position field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPosition

`func (o *Slide) SetPosition(v int32)`

SetPosition sets Position field to given value.


### GetCreatedAt

`func (o *Slide) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Slide) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Slide) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *Slide) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *Slide) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *Slide) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


