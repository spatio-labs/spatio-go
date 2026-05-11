# AccountPlan

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Tier** | **string** |  | 
**DisplayName** | **string** |  | 
**SubscriptionStatus** | **string** | Stripe subscription state: &#x60;ACTIVE&#x60;, &#x60;TRIALING&#x60;, &#x60;PAST_DUE&#x60;, &#x60;CANCELED&#x60;, etc. | 
**TrialEndsAt** | Pointer to **NullableTime** |  | [optional] 

## Methods

### NewAccountPlan

`func NewAccountPlan(tier string, displayName string, subscriptionStatus string, ) *AccountPlan`

NewAccountPlan instantiates a new AccountPlan object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAccountPlanWithDefaults

`func NewAccountPlanWithDefaults() *AccountPlan`

NewAccountPlanWithDefaults instantiates a new AccountPlan object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTier

`func (o *AccountPlan) GetTier() string`

GetTier returns the Tier field if non-nil, zero value otherwise.

### GetTierOk

`func (o *AccountPlan) GetTierOk() (*string, bool)`

GetTierOk returns a tuple with the Tier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTier

`func (o *AccountPlan) SetTier(v string)`

SetTier sets Tier field to given value.


### GetDisplayName

`func (o *AccountPlan) GetDisplayName() string`

GetDisplayName returns the DisplayName field if non-nil, zero value otherwise.

### GetDisplayNameOk

`func (o *AccountPlan) GetDisplayNameOk() (*string, bool)`

GetDisplayNameOk returns a tuple with the DisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayName

`func (o *AccountPlan) SetDisplayName(v string)`

SetDisplayName sets DisplayName field to given value.


### GetSubscriptionStatus

`func (o *AccountPlan) GetSubscriptionStatus() string`

GetSubscriptionStatus returns the SubscriptionStatus field if non-nil, zero value otherwise.

### GetSubscriptionStatusOk

`func (o *AccountPlan) GetSubscriptionStatusOk() (*string, bool)`

GetSubscriptionStatusOk returns a tuple with the SubscriptionStatus field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubscriptionStatus

`func (o *AccountPlan) SetSubscriptionStatus(v string)`

SetSubscriptionStatus sets SubscriptionStatus field to given value.


### GetTrialEndsAt

`func (o *AccountPlan) GetTrialEndsAt() time.Time`

GetTrialEndsAt returns the TrialEndsAt field if non-nil, zero value otherwise.

### GetTrialEndsAtOk

`func (o *AccountPlan) GetTrialEndsAtOk() (*time.Time, bool)`

GetTrialEndsAtOk returns a tuple with the TrialEndsAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTrialEndsAt

`func (o *AccountPlan) SetTrialEndsAt(v time.Time)`

SetTrialEndsAt sets TrialEndsAt field to given value.

### HasTrialEndsAt

`func (o *AccountPlan) HasTrialEndsAt() bool`

HasTrialEndsAt returns a boolean if a field has been set.

### SetTrialEndsAtNil

`func (o *AccountPlan) SetTrialEndsAtNil(b bool)`

 SetTrialEndsAtNil sets the value for TrialEndsAt to be an explicit nil

### UnsetTrialEndsAt
`func (o *AccountPlan) UnsetTrialEndsAt()`

UnsetTrialEndsAt ensures that no value is present for TrialEndsAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


