# SlideList

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Slides** | [**[]Slide**](Slide.md) |  | 
**Total** | **int32** |  | 

## Methods

### NewSlideList

`func NewSlideList(slides []Slide, total int32, ) *SlideList`

NewSlideList instantiates a new SlideList object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSlideListWithDefaults

`func NewSlideListWithDefaults() *SlideList`

NewSlideListWithDefaults instantiates a new SlideList object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSlides

`func (o *SlideList) GetSlides() []Slide`

GetSlides returns the Slides field if non-nil, zero value otherwise.

### GetSlidesOk

`func (o *SlideList) GetSlidesOk() (*[]Slide, bool)`

GetSlidesOk returns a tuple with the Slides field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlides

`func (o *SlideList) SetSlides(v []Slide)`

SetSlides sets Slides field to given value.


### GetTotal

`func (o *SlideList) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *SlideList) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *SlideList) SetTotal(v int32)`

SetTotal sets Total field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


