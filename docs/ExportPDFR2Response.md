# ExportPDFR2Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Storage** | **string** |  | 
**Url** | **string** | 24-hour signed URL. | 
**ExpiresAt** | **time.Time** |  | 
**Size** | **int32** | PDF size in bytes. | 

## Methods

### NewExportPDFR2Response

`func NewExportPDFR2Response(storage string, url string, expiresAt time.Time, size int32, ) *ExportPDFR2Response`

NewExportPDFR2Response instantiates a new ExportPDFR2Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewExportPDFR2ResponseWithDefaults

`func NewExportPDFR2ResponseWithDefaults() *ExportPDFR2Response`

NewExportPDFR2ResponseWithDefaults instantiates a new ExportPDFR2Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetStorage

`func (o *ExportPDFR2Response) GetStorage() string`

GetStorage returns the Storage field if non-nil, zero value otherwise.

### GetStorageOk

`func (o *ExportPDFR2Response) GetStorageOk() (*string, bool)`

GetStorageOk returns a tuple with the Storage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStorage

`func (o *ExportPDFR2Response) SetStorage(v string)`

SetStorage sets Storage field to given value.


### GetUrl

`func (o *ExportPDFR2Response) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *ExportPDFR2Response) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *ExportPDFR2Response) SetUrl(v string)`

SetUrl sets Url field to given value.


### GetExpiresAt

`func (o *ExportPDFR2Response) GetExpiresAt() time.Time`

GetExpiresAt returns the ExpiresAt field if non-nil, zero value otherwise.

### GetExpiresAtOk

`func (o *ExportPDFR2Response) GetExpiresAtOk() (*time.Time, bool)`

GetExpiresAtOk returns a tuple with the ExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresAt

`func (o *ExportPDFR2Response) SetExpiresAt(v time.Time)`

SetExpiresAt sets ExpiresAt field to given value.


### GetSize

`func (o *ExportPDFR2Response) GetSize() int32`

GetSize returns the Size field if non-nil, zero value otherwise.

### GetSizeOk

`func (o *ExportPDFR2Response) GetSizeOk() (*int32, bool)`

GetSizeOk returns a tuple with the Size field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSize

`func (o *ExportPDFR2Response) SetSize(v int32)`

SetSize sets Size field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


