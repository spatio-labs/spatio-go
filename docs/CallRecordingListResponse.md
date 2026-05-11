# CallRecordingListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Recordings** | [**[]CallRecording**](CallRecording.md) |  | 

## Methods

### NewCallRecordingListResponse

`func NewCallRecordingListResponse(recordings []CallRecording, ) *CallRecordingListResponse`

NewCallRecordingListResponse instantiates a new CallRecordingListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCallRecordingListResponseWithDefaults

`func NewCallRecordingListResponseWithDefaults() *CallRecordingListResponse`

NewCallRecordingListResponseWithDefaults instantiates a new CallRecordingListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRecordings

`func (o *CallRecordingListResponse) GetRecordings() []CallRecording`

GetRecordings returns the Recordings field if non-nil, zero value otherwise.

### GetRecordingsOk

`func (o *CallRecordingListResponse) GetRecordingsOk() (*[]CallRecording, bool)`

GetRecordingsOk returns a tuple with the Recordings field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRecordings

`func (o *CallRecordingListResponse) SetRecordings(v []CallRecording)`

SetRecordings sets Recordings field to given value.


### SetRecordingsNil

`func (o *CallRecordingListResponse) SetRecordingsNil(b bool)`

 SetRecordingsNil sets the value for Recordings to be an explicit nil

### UnsetRecordings
`func (o *CallRecordingListResponse) UnsetRecordings()`

UnsetRecordings ensures that no value is present for Recordings, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


