# FederatedSearchRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Query** | **string** |  | 
**Platforms** | Pointer to **[]string** | Subset to fan out to. Empty means all available platforms. | [optional] 
**Limit** | Pointer to **int32** |  | [optional] [default to 25]
**PageTokens** | Pointer to **map[string]string** | Per-platform cursor for pagination. | [optional] 
**WorkspaceId** | Pointer to **string** |  | [optional] 
**OrganizationId** | Pointer to **string** |  | [optional] 
**IncludeShared** | Pointer to **bool** |  | [optional] 
**IncludeArchived** | Pointer to **bool** |  | [optional] 

## Methods

### NewFederatedSearchRequest

`func NewFederatedSearchRequest(query string, ) *FederatedSearchRequest`

NewFederatedSearchRequest instantiates a new FederatedSearchRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewFederatedSearchRequestWithDefaults

`func NewFederatedSearchRequestWithDefaults() *FederatedSearchRequest`

NewFederatedSearchRequestWithDefaults instantiates a new FederatedSearchRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetQuery

`func (o *FederatedSearchRequest) GetQuery() string`

GetQuery returns the Query field if non-nil, zero value otherwise.

### GetQueryOk

`func (o *FederatedSearchRequest) GetQueryOk() (*string, bool)`

GetQueryOk returns a tuple with the Query field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuery

`func (o *FederatedSearchRequest) SetQuery(v string)`

SetQuery sets Query field to given value.


### GetPlatforms

`func (o *FederatedSearchRequest) GetPlatforms() []string`

GetPlatforms returns the Platforms field if non-nil, zero value otherwise.

### GetPlatformsOk

`func (o *FederatedSearchRequest) GetPlatformsOk() (*[]string, bool)`

GetPlatformsOk returns a tuple with the Platforms field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPlatforms

`func (o *FederatedSearchRequest) SetPlatforms(v []string)`

SetPlatforms sets Platforms field to given value.

### HasPlatforms

`func (o *FederatedSearchRequest) HasPlatforms() bool`

HasPlatforms returns a boolean if a field has been set.

### GetLimit

`func (o *FederatedSearchRequest) GetLimit() int32`

GetLimit returns the Limit field if non-nil, zero value otherwise.

### GetLimitOk

`func (o *FederatedSearchRequest) GetLimitOk() (*int32, bool)`

GetLimitOk returns a tuple with the Limit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLimit

`func (o *FederatedSearchRequest) SetLimit(v int32)`

SetLimit sets Limit field to given value.

### HasLimit

`func (o *FederatedSearchRequest) HasLimit() bool`

HasLimit returns a boolean if a field has been set.

### GetPageTokens

`func (o *FederatedSearchRequest) GetPageTokens() map[string]string`

GetPageTokens returns the PageTokens field if non-nil, zero value otherwise.

### GetPageTokensOk

`func (o *FederatedSearchRequest) GetPageTokensOk() (*map[string]string, bool)`

GetPageTokensOk returns a tuple with the PageTokens field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPageTokens

`func (o *FederatedSearchRequest) SetPageTokens(v map[string]string)`

SetPageTokens sets PageTokens field to given value.

### HasPageTokens

`func (o *FederatedSearchRequest) HasPageTokens() bool`

HasPageTokens returns a boolean if a field has been set.

### GetWorkspaceId

`func (o *FederatedSearchRequest) GetWorkspaceId() string`

GetWorkspaceId returns the WorkspaceId field if non-nil, zero value otherwise.

### GetWorkspaceIdOk

`func (o *FederatedSearchRequest) GetWorkspaceIdOk() (*string, bool)`

GetWorkspaceIdOk returns a tuple with the WorkspaceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWorkspaceId

`func (o *FederatedSearchRequest) SetWorkspaceId(v string)`

SetWorkspaceId sets WorkspaceId field to given value.

### HasWorkspaceId

`func (o *FederatedSearchRequest) HasWorkspaceId() bool`

HasWorkspaceId returns a boolean if a field has been set.

### GetOrganizationId

`func (o *FederatedSearchRequest) GetOrganizationId() string`

GetOrganizationId returns the OrganizationId field if non-nil, zero value otherwise.

### GetOrganizationIdOk

`func (o *FederatedSearchRequest) GetOrganizationIdOk() (*string, bool)`

GetOrganizationIdOk returns a tuple with the OrganizationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrganizationId

`func (o *FederatedSearchRequest) SetOrganizationId(v string)`

SetOrganizationId sets OrganizationId field to given value.

### HasOrganizationId

`func (o *FederatedSearchRequest) HasOrganizationId() bool`

HasOrganizationId returns a boolean if a field has been set.

### GetIncludeShared

`func (o *FederatedSearchRequest) GetIncludeShared() bool`

GetIncludeShared returns the IncludeShared field if non-nil, zero value otherwise.

### GetIncludeSharedOk

`func (o *FederatedSearchRequest) GetIncludeSharedOk() (*bool, bool)`

GetIncludeSharedOk returns a tuple with the IncludeShared field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIncludeShared

`func (o *FederatedSearchRequest) SetIncludeShared(v bool)`

SetIncludeShared sets IncludeShared field to given value.

### HasIncludeShared

`func (o *FederatedSearchRequest) HasIncludeShared() bool`

HasIncludeShared returns a boolean if a field has been set.

### GetIncludeArchived

`func (o *FederatedSearchRequest) GetIncludeArchived() bool`

GetIncludeArchived returns the IncludeArchived field if non-nil, zero value otherwise.

### GetIncludeArchivedOk

`func (o *FederatedSearchRequest) GetIncludeArchivedOk() (*bool, bool)`

GetIncludeArchivedOk returns a tuple with the IncludeArchived field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIncludeArchived

`func (o *FederatedSearchRequest) SetIncludeArchived(v bool)`

SetIncludeArchived sets IncludeArchived field to given value.

### HasIncludeArchived

`func (o *FederatedSearchRequest) HasIncludeArchived() bool`

HasIncludeArchived returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


