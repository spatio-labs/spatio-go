# ContactCategoryListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Categories** | [**[]ContactCategory**](ContactCategory.md) |  | 

## Methods

### NewContactCategoryListResponse

`func NewContactCategoryListResponse(categories []ContactCategory, ) *ContactCategoryListResponse`

NewContactCategoryListResponse instantiates a new ContactCategoryListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewContactCategoryListResponseWithDefaults

`func NewContactCategoryListResponseWithDefaults() *ContactCategoryListResponse`

NewContactCategoryListResponseWithDefaults instantiates a new ContactCategoryListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCategories

`func (o *ContactCategoryListResponse) GetCategories() []ContactCategory`

GetCategories returns the Categories field if non-nil, zero value otherwise.

### GetCategoriesOk

`func (o *ContactCategoryListResponse) GetCategoriesOk() (*[]ContactCategory, bool)`

GetCategoriesOk returns a tuple with the Categories field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCategories

`func (o *ContactCategoryListResponse) SetCategories(v []ContactCategory)`

SetCategories sets Categories field to given value.


### SetCategoriesNil

`func (o *ContactCategoryListResponse) SetCategoriesNil(b bool)`

 SetCategoriesNil sets the value for Categories to be an explicit nil

### UnsetCategories
`func (o *ContactCategoryListResponse) UnsetCategories()`

UnsetCategories ensures that no value is present for Categories, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


