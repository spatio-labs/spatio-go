# JWK

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Kty** | **string** |  | 
**Use** | **string** |  | 
**Alg** | **string** |  | 
**Kid** | **string** |  | 
**N** | **string** | Base64url-encoded RSA modulus. | 
**E** | **string** | Base64url-encoded RSA exponent. Almost always \&quot;AQAB\&quot;. | 

## Methods

### NewJWK

`func NewJWK(kty string, use string, alg string, kid string, n string, e string, ) *JWK`

NewJWK instantiates a new JWK object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewJWKWithDefaults

`func NewJWKWithDefaults() *JWK`

NewJWKWithDefaults instantiates a new JWK object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetKty

`func (o *JWK) GetKty() string`

GetKty returns the Kty field if non-nil, zero value otherwise.

### GetKtyOk

`func (o *JWK) GetKtyOk() (*string, bool)`

GetKtyOk returns a tuple with the Kty field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKty

`func (o *JWK) SetKty(v string)`

SetKty sets Kty field to given value.


### GetUse

`func (o *JWK) GetUse() string`

GetUse returns the Use field if non-nil, zero value otherwise.

### GetUseOk

`func (o *JWK) GetUseOk() (*string, bool)`

GetUseOk returns a tuple with the Use field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUse

`func (o *JWK) SetUse(v string)`

SetUse sets Use field to given value.


### GetAlg

`func (o *JWK) GetAlg() string`

GetAlg returns the Alg field if non-nil, zero value otherwise.

### GetAlgOk

`func (o *JWK) GetAlgOk() (*string, bool)`

GetAlgOk returns a tuple with the Alg field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAlg

`func (o *JWK) SetAlg(v string)`

SetAlg sets Alg field to given value.


### GetKid

`func (o *JWK) GetKid() string`

GetKid returns the Kid field if non-nil, zero value otherwise.

### GetKidOk

`func (o *JWK) GetKidOk() (*string, bool)`

GetKidOk returns a tuple with the Kid field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKid

`func (o *JWK) SetKid(v string)`

SetKid sets Kid field to given value.


### GetN

`func (o *JWK) GetN() string`

GetN returns the N field if non-nil, zero value otherwise.

### GetNOk

`func (o *JWK) GetNOk() (*string, bool)`

GetNOk returns a tuple with the N field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetN

`func (o *JWK) SetN(v string)`

SetN sets N field to given value.


### GetE

`func (o *JWK) GetE() string`

GetE returns the E field if non-nil, zero value otherwise.

### GetEOk

`func (o *JWK) GetEOk() (*string, bool)`

GetEOk returns a tuple with the E field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetE

`func (o *JWK) SetE(v string)`

SetE sets E field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


