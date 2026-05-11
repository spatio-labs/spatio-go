# ProposeRecommendationRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**WorkspaceId** | Pointer to **string** |  | [optional] 
**Kind** | **string** |  | 
**Title** | Pointer to **string** |  | [optional] 
**Body** | Pointer to **string** |  | [optional] 
**Payload** | Pointer to **map[string]interface{}** |  | [optional] 
**ExpiresAt** | Pointer to **time.Time** |  | [optional] 

## Methods

### NewProposeRecommendationRequest

`func NewProposeRecommendationRequest(kind string, ) *ProposeRecommendationRequest`

NewProposeRecommendationRequest instantiates a new ProposeRecommendationRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewProposeRecommendationRequestWithDefaults

`func NewProposeRecommendationRequestWithDefaults() *ProposeRecommendationRequest`

NewProposeRecommendationRequestWithDefaults instantiates a new ProposeRecommendationRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetWorkspaceId

`func (o *ProposeRecommendationRequest) GetWorkspaceId() string`

GetWorkspaceId returns the WorkspaceId field if non-nil, zero value otherwise.

### GetWorkspaceIdOk

`func (o *ProposeRecommendationRequest) GetWorkspaceIdOk() (*string, bool)`

GetWorkspaceIdOk returns a tuple with the WorkspaceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWorkspaceId

`func (o *ProposeRecommendationRequest) SetWorkspaceId(v string)`

SetWorkspaceId sets WorkspaceId field to given value.

### HasWorkspaceId

`func (o *ProposeRecommendationRequest) HasWorkspaceId() bool`

HasWorkspaceId returns a boolean if a field has been set.

### GetKind

`func (o *ProposeRecommendationRequest) GetKind() string`

GetKind returns the Kind field if non-nil, zero value otherwise.

### GetKindOk

`func (o *ProposeRecommendationRequest) GetKindOk() (*string, bool)`

GetKindOk returns a tuple with the Kind field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKind

`func (o *ProposeRecommendationRequest) SetKind(v string)`

SetKind sets Kind field to given value.


### GetTitle

`func (o *ProposeRecommendationRequest) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *ProposeRecommendationRequest) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *ProposeRecommendationRequest) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *ProposeRecommendationRequest) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### GetBody

`func (o *ProposeRecommendationRequest) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *ProposeRecommendationRequest) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *ProposeRecommendationRequest) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *ProposeRecommendationRequest) HasBody() bool`

HasBody returns a boolean if a field has been set.

### GetPayload

`func (o *ProposeRecommendationRequest) GetPayload() map[string]interface{}`

GetPayload returns the Payload field if non-nil, zero value otherwise.

### GetPayloadOk

`func (o *ProposeRecommendationRequest) GetPayloadOk() (*map[string]interface{}, bool)`

GetPayloadOk returns a tuple with the Payload field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPayload

`func (o *ProposeRecommendationRequest) SetPayload(v map[string]interface{})`

SetPayload sets Payload field to given value.

### HasPayload

`func (o *ProposeRecommendationRequest) HasPayload() bool`

HasPayload returns a boolean if a field has been set.

### GetExpiresAt

`func (o *ProposeRecommendationRequest) GetExpiresAt() time.Time`

GetExpiresAt returns the ExpiresAt field if non-nil, zero value otherwise.

### GetExpiresAtOk

`func (o *ProposeRecommendationRequest) GetExpiresAtOk() (*time.Time, bool)`

GetExpiresAtOk returns a tuple with the ExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresAt

`func (o *ProposeRecommendationRequest) SetExpiresAt(v time.Time)`

SetExpiresAt sets ExpiresAt field to given value.

### HasExpiresAt

`func (o *ProposeRecommendationRequest) HasExpiresAt() bool`

HasExpiresAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


