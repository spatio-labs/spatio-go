# SendEmailResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Success** | **bool** |  | 
**MessageId** | **string** |  | 
**ThreadId** | Pointer to **string** |  | [optional] 
**Provider** | **string** |  | 
**Error** | Pointer to **string** |  | [optional] 

## Methods

### NewSendEmailResponse

`func NewSendEmailResponse(success bool, messageId string, provider string, ) *SendEmailResponse`

NewSendEmailResponse instantiates a new SendEmailResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSendEmailResponseWithDefaults

`func NewSendEmailResponseWithDefaults() *SendEmailResponse`

NewSendEmailResponseWithDefaults instantiates a new SendEmailResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSuccess

`func (o *SendEmailResponse) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *SendEmailResponse) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *SendEmailResponse) SetSuccess(v bool)`

SetSuccess sets Success field to given value.


### GetMessageId

`func (o *SendEmailResponse) GetMessageId() string`

GetMessageId returns the MessageId field if non-nil, zero value otherwise.

### GetMessageIdOk

`func (o *SendEmailResponse) GetMessageIdOk() (*string, bool)`

GetMessageIdOk returns a tuple with the MessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageId

`func (o *SendEmailResponse) SetMessageId(v string)`

SetMessageId sets MessageId field to given value.


### GetThreadId

`func (o *SendEmailResponse) GetThreadId() string`

GetThreadId returns the ThreadId field if non-nil, zero value otherwise.

### GetThreadIdOk

`func (o *SendEmailResponse) GetThreadIdOk() (*string, bool)`

GetThreadIdOk returns a tuple with the ThreadId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetThreadId

`func (o *SendEmailResponse) SetThreadId(v string)`

SetThreadId sets ThreadId field to given value.

### HasThreadId

`func (o *SendEmailResponse) HasThreadId() bool`

HasThreadId returns a boolean if a field has been set.

### GetProvider

`func (o *SendEmailResponse) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *SendEmailResponse) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *SendEmailResponse) SetProvider(v string)`

SetProvider sets Provider field to given value.


### GetError

`func (o *SendEmailResponse) GetError() string`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *SendEmailResponse) GetErrorOk() (*string, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *SendEmailResponse) SetError(v string)`

SetError sets Error field to given value.

### HasError

`func (o *SendEmailResponse) HasError() bool`

HasError returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


