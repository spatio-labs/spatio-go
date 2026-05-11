# SlideElement

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**SlideId** | **string** |  | 
**ElementType** | **string** | Free-form type id (&#x60;text&#x60;, &#x60;image&#x60;, &#x60;shape&#x60;, etc.). | 
**Content** | **map[string]interface{}** |  | 
**X** | **float64** |  | 
**Y** | **float64** |  | 
**Width** | **float64** |  | 
**Height** | **float64** |  | 
**Rotation** | **float64** | Degrees. | 
**ZIndex** | **int32** |  | 
**CreatedAt** | **time.Time** |  | 
**UpdatedAt** | **time.Time** |  | 

## Methods

### NewSlideElement

`func NewSlideElement(id string, slideId string, elementType string, content map[string]interface{}, x float64, y float64, width float64, height float64, rotation float64, zIndex int32, createdAt time.Time, updatedAt time.Time, ) *SlideElement`

NewSlideElement instantiates a new SlideElement object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSlideElementWithDefaults

`func NewSlideElementWithDefaults() *SlideElement`

NewSlideElementWithDefaults instantiates a new SlideElement object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *SlideElement) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *SlideElement) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *SlideElement) SetId(v string)`

SetId sets Id field to given value.


### GetSlideId

`func (o *SlideElement) GetSlideId() string`

GetSlideId returns the SlideId field if non-nil, zero value otherwise.

### GetSlideIdOk

`func (o *SlideElement) GetSlideIdOk() (*string, bool)`

GetSlideIdOk returns a tuple with the SlideId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlideId

`func (o *SlideElement) SetSlideId(v string)`

SetSlideId sets SlideId field to given value.


### GetElementType

`func (o *SlideElement) GetElementType() string`

GetElementType returns the ElementType field if non-nil, zero value otherwise.

### GetElementTypeOk

`func (o *SlideElement) GetElementTypeOk() (*string, bool)`

GetElementTypeOk returns a tuple with the ElementType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetElementType

`func (o *SlideElement) SetElementType(v string)`

SetElementType sets ElementType field to given value.


### GetContent

`func (o *SlideElement) GetContent() map[string]interface{}`

GetContent returns the Content field if non-nil, zero value otherwise.

### GetContentOk

`func (o *SlideElement) GetContentOk() (*map[string]interface{}, bool)`

GetContentOk returns a tuple with the Content field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContent

`func (o *SlideElement) SetContent(v map[string]interface{})`

SetContent sets Content field to given value.


### GetX

`func (o *SlideElement) GetX() float64`

GetX returns the X field if non-nil, zero value otherwise.

### GetXOk

`func (o *SlideElement) GetXOk() (*float64, bool)`

GetXOk returns a tuple with the X field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetX

`func (o *SlideElement) SetX(v float64)`

SetX sets X field to given value.


### GetY

`func (o *SlideElement) GetY() float64`

GetY returns the Y field if non-nil, zero value otherwise.

### GetYOk

`func (o *SlideElement) GetYOk() (*float64, bool)`

GetYOk returns a tuple with the Y field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetY

`func (o *SlideElement) SetY(v float64)`

SetY sets Y field to given value.


### GetWidth

`func (o *SlideElement) GetWidth() float64`

GetWidth returns the Width field if non-nil, zero value otherwise.

### GetWidthOk

`func (o *SlideElement) GetWidthOk() (*float64, bool)`

GetWidthOk returns a tuple with the Width field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWidth

`func (o *SlideElement) SetWidth(v float64)`

SetWidth sets Width field to given value.


### GetHeight

`func (o *SlideElement) GetHeight() float64`

GetHeight returns the Height field if non-nil, zero value otherwise.

### GetHeightOk

`func (o *SlideElement) GetHeightOk() (*float64, bool)`

GetHeightOk returns a tuple with the Height field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHeight

`func (o *SlideElement) SetHeight(v float64)`

SetHeight sets Height field to given value.


### GetRotation

`func (o *SlideElement) GetRotation() float64`

GetRotation returns the Rotation field if non-nil, zero value otherwise.

### GetRotationOk

`func (o *SlideElement) GetRotationOk() (*float64, bool)`

GetRotationOk returns a tuple with the Rotation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRotation

`func (o *SlideElement) SetRotation(v float64)`

SetRotation sets Rotation field to given value.


### GetZIndex

`func (o *SlideElement) GetZIndex() int32`

GetZIndex returns the ZIndex field if non-nil, zero value otherwise.

### GetZIndexOk

`func (o *SlideElement) GetZIndexOk() (*int32, bool)`

GetZIndexOk returns a tuple with the ZIndex field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetZIndex

`func (o *SlideElement) SetZIndex(v int32)`

SetZIndex sets ZIndex field to given value.


### GetCreatedAt

`func (o *SlideElement) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *SlideElement) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *SlideElement) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *SlideElement) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *SlideElement) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *SlideElement) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


