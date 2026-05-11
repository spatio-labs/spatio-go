# \OAuthAPI

All URIs are relative to *https://api.spatio.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetJWKS**](OAuthAPI.md#GetJWKS) | **Get** /.well-known/jwks.json | JSON Web Key Set for id_token verification (RFC 7517).
[**GetOAuthDiscovery**](OAuthAPI.md#GetOAuthDiscovery) | **Get** /.well-known/oauth-authorization-server | OAuth 2.1 authorization server metadata (RFC 8414).
[**GetOpenIDConfiguration**](OAuthAPI.md#GetOpenIDConfiguration) | **Get** /.well-known/openid-configuration | OpenID Connect Discovery 1.0 metadata.
[**GetUserInfo**](OAuthAPI.md#GetUserInfo) | **Get** /oauth2/userinfo | OIDC UserInfo (OpenID Connect Core 1.0 §5.3).
[**OauthAuthorize**](OAuthAPI.md#OauthAuthorize) | **Get** /oauth2/authorize | OAuth 2.1 authorization endpoint (RFC 6749 + 7636 PKCE).
[**OauthIntrospect**](OAuthAPI.md#OauthIntrospect) | **Post** /oauth2/introspect | RFC 7662 token introspection. Accepts both OAuth access tokens and PATs.
[**OauthRevoke**](OAuthAPI.md#OauthRevoke) | **Post** /oauth2/revoke | RFC 7009 token revocation. Idempotent.
[**OauthToken**](OAuthAPI.md#OauthToken) | **Post** /oauth2/token | Exchange authorization code or refresh token for an access token (+ id_token if &#x60;openid&#x60; scope).
[**PostUserInfo**](OAuthAPI.md#PostUserInfo) | **Post** /oauth2/userinfo | Same as GET /oauth2/userinfo. Provided for clients that send the bearer in the body.
[**RegisterOAuthClient**](OAuthAPI.md#RegisterOAuthClient) | **Post** /oauth2/register | Register a new OAuth 2.1 client (RFC 7591 dynamic client registration).



## GetJWKS

> JWKS GetJWKS(ctx).Execute()

JSON Web Key Set for id_token verification (RFC 7517).



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/spatio-labs/spatio-go"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OAuthAPI.GetJWKS(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OAuthAPI.GetJWKS``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetJWKS`: JWKS
	fmt.Fprintf(os.Stdout, "Response from `OAuthAPI.GetJWKS`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetJWKSRequest struct via the builder pattern


### Return type

[**JWKS**](JWKS.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetOAuthDiscovery

> DiscoveryDocument GetOAuthDiscovery(ctx).Execute()

OAuth 2.1 authorization server metadata (RFC 8414).



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/spatio-labs/spatio-go"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OAuthAPI.GetOAuthDiscovery(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OAuthAPI.GetOAuthDiscovery``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetOAuthDiscovery`: DiscoveryDocument
	fmt.Fprintf(os.Stdout, "Response from `OAuthAPI.GetOAuthDiscovery`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetOAuthDiscoveryRequest struct via the builder pattern


### Return type

[**DiscoveryDocument**](DiscoveryDocument.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetOpenIDConfiguration

> DiscoveryDocument GetOpenIDConfiguration(ctx).Execute()

OpenID Connect Discovery 1.0 metadata.



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/spatio-labs/spatio-go"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OAuthAPI.GetOpenIDConfiguration(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OAuthAPI.GetOpenIDConfiguration``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetOpenIDConfiguration`: DiscoveryDocument
	fmt.Fprintf(os.Stdout, "Response from `OAuthAPI.GetOpenIDConfiguration`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetOpenIDConfigurationRequest struct via the builder pattern


### Return type

[**DiscoveryDocument**](DiscoveryDocument.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetUserInfo

> UserInfoResponse GetUserInfo(ctx).Execute()

OIDC UserInfo (OpenID Connect Core 1.0 §5.3).



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/spatio-labs/spatio-go"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OAuthAPI.GetUserInfo(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OAuthAPI.GetUserInfo``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetUserInfo`: UserInfoResponse
	fmt.Fprintf(os.Stdout, "Response from `OAuthAPI.GetUserInfo`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetUserInfoRequest struct via the builder pattern


### Return type

[**UserInfoResponse**](UserInfoResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## OauthAuthorize

> OauthAuthorize(ctx).ClientId(clientId).RedirectUri(redirectUri).ResponseType(responseType).CodeChallenge(codeChallenge).CodeChallengeMethod(codeChallengeMethod).Scope(scope).State(state).Nonce(nonce).Prompt(prompt).MaxAge(maxAge).Execute()

OAuth 2.1 authorization endpoint (RFC 6749 + 7636 PKCE).



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/spatio-labs/spatio-go"
)

func main() {
	clientId := "clientId_example" // string | 
	redirectUri := "redirectUri_example" // string | 
	responseType := "responseType_example" // string | 
	codeChallenge := "codeChallenge_example" // string | 
	codeChallengeMethod := "codeChallengeMethod_example" // string | 
	scope := "scope_example" // string |  (optional)
	state := "state_example" // string |  (optional)
	nonce := "nonce_example" // string |  (optional)
	prompt := "prompt_example" // string |  (optional)
	maxAge := int32(56) // int32 |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.OAuthAPI.OauthAuthorize(context.Background()).ClientId(clientId).RedirectUri(redirectUri).ResponseType(responseType).CodeChallenge(codeChallenge).CodeChallengeMethod(codeChallengeMethod).Scope(scope).State(state).Nonce(nonce).Prompt(prompt).MaxAge(maxAge).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OAuthAPI.OauthAuthorize``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiOauthAuthorizeRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **clientId** | **string** |  | 
 **redirectUri** | **string** |  | 
 **responseType** | **string** |  | 
 **codeChallenge** | **string** |  | 
 **codeChallengeMethod** | **string** |  | 
 **scope** | **string** |  | 
 **state** | **string** |  | 
 **nonce** | **string** |  | 
 **prompt** | **string** |  | 
 **maxAge** | **int32** |  | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## OauthIntrospect

> IntrospectionResponse OauthIntrospect(ctx).Token(token).Execute()

RFC 7662 token introspection. Accepts both OAuth access tokens and PATs.

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/spatio-labs/spatio-go"
)

func main() {
	token := "token_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OAuthAPI.OauthIntrospect(context.Background()).Token(token).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OAuthAPI.OauthIntrospect``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `OauthIntrospect`: IntrospectionResponse
	fmt.Fprintf(os.Stdout, "Response from `OAuthAPI.OauthIntrospect`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiOauthIntrospectRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **string** |  | 

### Return type

[**IntrospectionResponse**](IntrospectionResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/x-www-form-urlencoded
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## OauthRevoke

> OauthRevoke(ctx).Token(token).Execute()

RFC 7009 token revocation. Idempotent.

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/spatio-labs/spatio-go"
)

func main() {
	token := "token_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.OAuthAPI.OauthRevoke(context.Background()).Token(token).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OAuthAPI.OauthRevoke``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiOauthRevokeRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **string** |  | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/x-www-form-urlencoded
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## OauthToken

> TokenResponse OauthToken(ctx).GrantType(grantType).Code(code).CodeVerifier(codeVerifier).RedirectUri(redirectUri).RefreshToken(refreshToken).ClientId(clientId).ClientSecret(clientSecret).Execute()

Exchange authorization code or refresh token for an access token (+ id_token if `openid` scope).

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/spatio-labs/spatio-go"
)

func main() {
	grantType := "grantType_example" // string | 
	code := "code_example" // string | Required for authorization_code grant. (optional)
	codeVerifier := "codeVerifier_example" // string | PKCE verifier — required for authorization_code grant. (optional)
	redirectUri := "redirectUri_example" // string |  (optional)
	refreshToken := "refreshToken_example" // string | Required for refresh_token grant. (optional)
	clientId := "clientId_example" // string |  (optional)
	clientSecret := "clientSecret_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OAuthAPI.OauthToken(context.Background()).GrantType(grantType).Code(code).CodeVerifier(codeVerifier).RedirectUri(redirectUri).RefreshToken(refreshToken).ClientId(clientId).ClientSecret(clientSecret).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OAuthAPI.OauthToken``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `OauthToken`: TokenResponse
	fmt.Fprintf(os.Stdout, "Response from `OAuthAPI.OauthToken`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiOauthTokenRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **grantType** | **string** |  | 
 **code** | **string** | Required for authorization_code grant. | 
 **codeVerifier** | **string** | PKCE verifier — required for authorization_code grant. | 
 **redirectUri** | **string** |  | 
 **refreshToken** | **string** | Required for refresh_token grant. | 
 **clientId** | **string** |  | 
 **clientSecret** | **string** |  | 

### Return type

[**TokenResponse**](TokenResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/x-www-form-urlencoded
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PostUserInfo

> UserInfoResponse PostUserInfo(ctx).Execute()

Same as GET /oauth2/userinfo. Provided for clients that send the bearer in the body.

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/spatio-labs/spatio-go"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OAuthAPI.PostUserInfo(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OAuthAPI.PostUserInfo``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PostUserInfo`: UserInfoResponse
	fmt.Fprintf(os.Stdout, "Response from `OAuthAPI.PostUserInfo`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiPostUserInfoRequest struct via the builder pattern


### Return type

[**UserInfoResponse**](UserInfoResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RegisterOAuthClient

> ClientRegistrationResponse RegisterOAuthClient(ctx).ClientRegistrationRequest(clientRegistrationRequest).Execute()

Register a new OAuth 2.1 client (RFC 7591 dynamic client registration).



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/spatio-labs/spatio-go"
)

func main() {
	clientRegistrationRequest := *openapiclient.NewClientRegistrationRequest("ClientName_example", []string{"RedirectUris_example"}) // ClientRegistrationRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OAuthAPI.RegisterOAuthClient(context.Background()).ClientRegistrationRequest(clientRegistrationRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OAuthAPI.RegisterOAuthClient``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RegisterOAuthClient`: ClientRegistrationResponse
	fmt.Fprintf(os.Stdout, "Response from `OAuthAPI.RegisterOAuthClient`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRegisterOAuthClientRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **clientRegistrationRequest** | [**ClientRegistrationRequest**](ClientRegistrationRequest.md) |  | 

### Return type

[**ClientRegistrationResponse**](ClientRegistrationResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

