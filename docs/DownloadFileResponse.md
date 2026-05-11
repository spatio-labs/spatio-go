# DownloadFileResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**SignedUrl** | **string** | Pre-signed direct-download URL pointing at the backing storage (R2, Drive, etc.). Time-limited per provider. Clients follow the URL — the platform does not proxy bytes.  | 
**File** | [**SpatioFile**](SpatioFile.md) |  | 

## Methods

### NewDownloadFileResponse

`func NewDownloadFileResponse(signedUrl string, file SpatioFile, ) *DownloadFileResponse`

NewDownloadFileResponse instantiates a new DownloadFileResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDownloadFileResponseWithDefaults

`func NewDownloadFileResponseWithDefaults() *DownloadFileResponse`

NewDownloadFileResponseWithDefaults instantiates a new DownloadFileResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSignedUrl

`func (o *DownloadFileResponse) GetSignedUrl() string`

GetSignedUrl returns the SignedUrl field if non-nil, zero value otherwise.

### GetSignedUrlOk

`func (o *DownloadFileResponse) GetSignedUrlOk() (*string, bool)`

GetSignedUrlOk returns a tuple with the SignedUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSignedUrl

`func (o *DownloadFileResponse) SetSignedUrl(v string)`

SetSignedUrl sets SignedUrl field to given value.


### GetFile

`func (o *DownloadFileResponse) GetFile() SpatioFile`

GetFile returns the File field if non-nil, zero value otherwise.

### GetFileOk

`func (o *DownloadFileResponse) GetFileOk() (*SpatioFile, bool)`

GetFileOk returns a tuple with the File field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFile

`func (o *DownloadFileResponse) SetFile(v SpatioFile)`

SetFile sets File field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


