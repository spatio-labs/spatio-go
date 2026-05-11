# CreateConversationRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Title** | Pointer to **string** |  | [optional] 
**Context** | Pointer to **string** |  | [optional] 
**Cwd** | Pointer to **string** |  | [optional] 
**SessionId** | Pointer to **string** |  | [optional] 
**Metadata** | Pointer to **map[string]interface{}** |  | [optional] 

## Methods

### NewCreateConversationRequest

`func NewCreateConversationRequest() *CreateConversationRequest`

NewCreateConversationRequest instantiates a new CreateConversationRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateConversationRequestWithDefaults

`func NewCreateConversationRequestWithDefaults() *CreateConversationRequest`

NewCreateConversationRequestWithDefaults instantiates a new CreateConversationRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTitle

`func (o *CreateConversationRequest) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *CreateConversationRequest) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *CreateConversationRequest) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *CreateConversationRequest) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### GetContext

`func (o *CreateConversationRequest) GetContext() string`

GetContext returns the Context field if non-nil, zero value otherwise.

### GetContextOk

`func (o *CreateConversationRequest) GetContextOk() (*string, bool)`

GetContextOk returns a tuple with the Context field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContext

`func (o *CreateConversationRequest) SetContext(v string)`

SetContext sets Context field to given value.

### HasContext

`func (o *CreateConversationRequest) HasContext() bool`

HasContext returns a boolean if a field has been set.

### GetCwd

`func (o *CreateConversationRequest) GetCwd() string`

GetCwd returns the Cwd field if non-nil, zero value otherwise.

### GetCwdOk

`func (o *CreateConversationRequest) GetCwdOk() (*string, bool)`

GetCwdOk returns a tuple with the Cwd field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCwd

`func (o *CreateConversationRequest) SetCwd(v string)`

SetCwd sets Cwd field to given value.

### HasCwd

`func (o *CreateConversationRequest) HasCwd() bool`

HasCwd returns a boolean if a field has been set.

### GetSessionId

`func (o *CreateConversationRequest) GetSessionId() string`

GetSessionId returns the SessionId field if non-nil, zero value otherwise.

### GetSessionIdOk

`func (o *CreateConversationRequest) GetSessionIdOk() (*string, bool)`

GetSessionIdOk returns a tuple with the SessionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSessionId

`func (o *CreateConversationRequest) SetSessionId(v string)`

SetSessionId sets SessionId field to given value.

### HasSessionId

`func (o *CreateConversationRequest) HasSessionId() bool`

HasSessionId returns a boolean if a field has been set.

### GetMetadata

`func (o *CreateConversationRequest) GetMetadata() map[string]interface{}`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *CreateConversationRequest) GetMetadataOk() (*map[string]interface{}, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *CreateConversationRequest) SetMetadata(v map[string]interface{})`

SetMetadata sets Metadata field to given value.

### HasMetadata

`func (o *CreateConversationRequest) HasMetadata() bool`

HasMetadata returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


