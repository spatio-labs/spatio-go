# ExportPDFRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**RasterizedSlides** | Pointer to [**[]ExportPDFRequestRasterizedSlidesInner**](ExportPDFRequestRasterizedSlidesInner.md) |  | [optional] 
**Theme** | Pointer to **map[string]interface{}** | Optional palette override. Schemaless — the export sidecar accepts a free-form palette object. Treat as opaque.  | [optional] 

## Methods

### NewExportPDFRequest

`func NewExportPDFRequest() *ExportPDFRequest`

NewExportPDFRequest instantiates a new ExportPDFRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewExportPDFRequestWithDefaults

`func NewExportPDFRequestWithDefaults() *ExportPDFRequest`

NewExportPDFRequestWithDefaults instantiates a new ExportPDFRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRasterizedSlides

`func (o *ExportPDFRequest) GetRasterizedSlides() []ExportPDFRequestRasterizedSlidesInner`

GetRasterizedSlides returns the RasterizedSlides field if non-nil, zero value otherwise.

### GetRasterizedSlidesOk

`func (o *ExportPDFRequest) GetRasterizedSlidesOk() (*[]ExportPDFRequestRasterizedSlidesInner, bool)`

GetRasterizedSlidesOk returns a tuple with the RasterizedSlides field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRasterizedSlides

`func (o *ExportPDFRequest) SetRasterizedSlides(v []ExportPDFRequestRasterizedSlidesInner)`

SetRasterizedSlides sets RasterizedSlides field to given value.

### HasRasterizedSlides

`func (o *ExportPDFRequest) HasRasterizedSlides() bool`

HasRasterizedSlides returns a boolean if a field has been set.

### GetTheme

`func (o *ExportPDFRequest) GetTheme() map[string]interface{}`

GetTheme returns the Theme field if non-nil, zero value otherwise.

### GetThemeOk

`func (o *ExportPDFRequest) GetThemeOk() (*map[string]interface{}, bool)`

GetThemeOk returns a tuple with the Theme field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTheme

`func (o *ExportPDFRequest) SetTheme(v map[string]interface{})`

SetTheme sets Theme field to given value.

### HasTheme

`func (o *ExportPDFRequest) HasTheme() bool`

HasTheme returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


