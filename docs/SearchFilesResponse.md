# SearchFilesResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Files** | Pointer to [**[]SpatioFile**](SpatioFile.md) |  | [optional] 
**Total** | **int32** |  | 
**HasMore** | **bool** |  | 
**Query** | **string** |  | 

## Methods

### NewSearchFilesResponse

`func NewSearchFilesResponse(total int32, hasMore bool, query string, ) *SearchFilesResponse`

NewSearchFilesResponse instantiates a new SearchFilesResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSearchFilesResponseWithDefaults

`func NewSearchFilesResponseWithDefaults() *SearchFilesResponse`

NewSearchFilesResponseWithDefaults instantiates a new SearchFilesResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFiles

`func (o *SearchFilesResponse) GetFiles() []SpatioFile`

GetFiles returns the Files field if non-nil, zero value otherwise.

### GetFilesOk

`func (o *SearchFilesResponse) GetFilesOk() (*[]SpatioFile, bool)`

GetFilesOk returns a tuple with the Files field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFiles

`func (o *SearchFilesResponse) SetFiles(v []SpatioFile)`

SetFiles sets Files field to given value.

### HasFiles

`func (o *SearchFilesResponse) HasFiles() bool`

HasFiles returns a boolean if a field has been set.

### SetFilesNil

`func (o *SearchFilesResponse) SetFilesNil(b bool)`

 SetFilesNil sets the value for Files to be an explicit nil

### UnsetFiles
`func (o *SearchFilesResponse) UnsetFiles()`

UnsetFiles ensures that no value is present for Files, not even an explicit nil
### GetTotal

`func (o *SearchFilesResponse) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *SearchFilesResponse) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *SearchFilesResponse) SetTotal(v int32)`

SetTotal sets Total field to given value.


### GetHasMore

`func (o *SearchFilesResponse) GetHasMore() bool`

GetHasMore returns the HasMore field if non-nil, zero value otherwise.

### GetHasMoreOk

`func (o *SearchFilesResponse) GetHasMoreOk() (*bool, bool)`

GetHasMoreOk returns a tuple with the HasMore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasMore

`func (o *SearchFilesResponse) SetHasMore(v bool)`

SetHasMore sets HasMore field to given value.


### GetQuery

`func (o *SearchFilesResponse) GetQuery() string`

GetQuery returns the Query field if non-nil, zero value otherwise.

### GetQueryOk

`func (o *SearchFilesResponse) GetQueryOk() (*string, bool)`

GetQueryOk returns a tuple with the Query field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuery

`func (o *SearchFilesResponse) SetQuery(v string)`

SetQuery sets Query field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


