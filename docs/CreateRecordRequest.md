# CreateRecordRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OrganizationId** | Pointer to **string** |  | [optional] 
**RecordTypeId** | **string** |  | 
**Name** | Pointer to **string** |  | [optional] 
**Attributes** | Pointer to **map[string]interface{}** |  | [optional] 
**Metadata** | Pointer to **map[string]interface{}** |  | [optional] 

## Methods

### NewCreateRecordRequest

`func NewCreateRecordRequest(recordTypeId string, ) *CreateRecordRequest`

NewCreateRecordRequest instantiates a new CreateRecordRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateRecordRequestWithDefaults

`func NewCreateRecordRequestWithDefaults() *CreateRecordRequest`

NewCreateRecordRequestWithDefaults instantiates a new CreateRecordRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetOrganizationId

`func (o *CreateRecordRequest) GetOrganizationId() string`

GetOrganizationId returns the OrganizationId field if non-nil, zero value otherwise.

### GetOrganizationIdOk

`func (o *CreateRecordRequest) GetOrganizationIdOk() (*string, bool)`

GetOrganizationIdOk returns a tuple with the OrganizationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrganizationId

`func (o *CreateRecordRequest) SetOrganizationId(v string)`

SetOrganizationId sets OrganizationId field to given value.

### HasOrganizationId

`func (o *CreateRecordRequest) HasOrganizationId() bool`

HasOrganizationId returns a boolean if a field has been set.

### GetRecordTypeId

`func (o *CreateRecordRequest) GetRecordTypeId() string`

GetRecordTypeId returns the RecordTypeId field if non-nil, zero value otherwise.

### GetRecordTypeIdOk

`func (o *CreateRecordRequest) GetRecordTypeIdOk() (*string, bool)`

GetRecordTypeIdOk returns a tuple with the RecordTypeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRecordTypeId

`func (o *CreateRecordRequest) SetRecordTypeId(v string)`

SetRecordTypeId sets RecordTypeId field to given value.


### GetName

`func (o *CreateRecordRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateRecordRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateRecordRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *CreateRecordRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### GetAttributes

`func (o *CreateRecordRequest) GetAttributes() map[string]interface{}`

GetAttributes returns the Attributes field if non-nil, zero value otherwise.

### GetAttributesOk

`func (o *CreateRecordRequest) GetAttributesOk() (*map[string]interface{}, bool)`

GetAttributesOk returns a tuple with the Attributes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributes

`func (o *CreateRecordRequest) SetAttributes(v map[string]interface{})`

SetAttributes sets Attributes field to given value.

### HasAttributes

`func (o *CreateRecordRequest) HasAttributes() bool`

HasAttributes returns a boolean if a field has been set.

### GetMetadata

`func (o *CreateRecordRequest) GetMetadata() map[string]interface{}`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *CreateRecordRequest) GetMetadataOk() (*map[string]interface{}, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *CreateRecordRequest) SetMetadata(v map[string]interface{})`

SetMetadata sets Metadata field to given value.

### HasMetadata

`func (o *CreateRecordRequest) HasMetadata() bool`

HasMetadata returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


