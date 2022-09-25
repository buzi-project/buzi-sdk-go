# \SmsApi

All URIs are relative to *https://petstore3.swagger.io*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CancelMessage**](SmsApi.md#CancelMessage) | **Post** /v1/sms/messages/{messageId}/cancel | Cancel a message
[**CreateMessage**](SmsApi.md#CreateMessage) | **Post** /v1/sms/messages | Create Message
[**CreatePricing**](SmsApi.md#CreatePricing) | **Put** /v1/sms/networks/{networkId}/pricing | Create network price
[**DeleteMessage**](SmsApi.md#DeleteMessage) | **Delete** /v1/sms/messages/{messageId} | Deletes a message
[**GetMessage**](SmsApi.md#GetMessage) | **Get** /v1/sms/messages/{messageId} | Get message
[**GetNetwork**](SmsApi.md#GetNetwork) | **Get** /v1/sms/networks/{networkId} | Get network
[**GetPricing**](SmsApi.md#GetPricing) | **Get** /v1/sms/networks/{networkId}/pricing | List network rates
[**ListMessages**](SmsApi.md#ListMessages) | **Get** /v1/sms/messages | List messages
[**ListNetworks**](SmsApi.md#ListNetworks) | **Get** /v1/sms/networks | List networks
[**SendMessage**](SmsApi.md#SendMessage) | **Post** /v1/sms/messages/{messageId}/send | Sends a message



## CancelMessage

> Message CancelMessage(context.Background(), messageId).Execute()

Cancel a message



### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
"./buzi"
)

func main() {
    messageId := int64(789) // int64 | ID of pet to return

    configuration := buzi.NewConfiguration(
        buzi.WithBaseURL("example.com"),
    )
    apiClient := buzi.New(configuration)
    resp, err := apiClient.SmsApi.CancelMessage(context.Background(), messageId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `SmsApi.CancelMessage``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `CancelMessage`: Message
    fmt.Fprintf(os.Stdout, "Response from `SmsApi.CancelMessage`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**messageId** | **int64** | ID of pet to return | 

### Other Parameters

Other parameters are passed through a pointer to a apiCancelMessageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**Message**](Message.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateMessage

> Message CreateMessage(context.Background(), createMessageInput).Execute()

Create Message



### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
"./buzi"
)

func main() {
    createMessageInput = buzi.CreateMessageInput{}

    configuration := buzi.NewConfiguration(
        buzi.WithBaseURL("example.com"),
    )
    apiClient := buzi.New(configuration)
    resp, err := apiClient.SmsApi.CreateMessage(context.Background(), createMessageInput).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `SmsApi.CreateMessage``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `CreateMessage`: Message
    fmt.Fprintf(os.Stdout, "Response from `SmsApi.CreateMessage`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateMessageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createMessageInput** | [**CreateMessageInput**](CreateMessageInput.md) | Update an existent pet in the store | 

### Return type

[**Message**](Message.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreatePricing

> Message CreatePricing(context.Background(), networkId).Execute()

Create network price



### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
"./buzi"
)

func main() {
    networkId := int32(56) // int32 | 

    configuration := buzi.NewConfiguration(
        buzi.WithBaseURL("example.com"),
    )
    apiClient := buzi.New(configuration)
    resp, err := apiClient.SmsApi.CreatePricing(context.Background(), networkId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `SmsApi.CreatePricing``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `CreatePricing`: Message
    fmt.Fprintf(os.Stdout, "Response from `SmsApi.CreatePricing`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**networkId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreatePricingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**Message**](Message.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteMessage

> Error DeleteMessage(context.Background(), messageId).Execute()

Deletes a message



### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
"./buzi"
)

func main() {
    messageId := int64(789) // int64 | Pet id to delete

    configuration := buzi.NewConfiguration(
        buzi.WithBaseURL("example.com"),
    )
    apiClient := buzi.New(configuration)
    resp, err := apiClient.SmsApi.DeleteMessage(context.Background(), messageId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `SmsApi.DeleteMessage``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `DeleteMessage`: Error
    fmt.Fprintf(os.Stdout, "Response from `SmsApi.DeleteMessage`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**messageId** | **int64** | Pet id to delete | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteMessageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **apiKey** | **string** |  | 

### Return type

[**Error**](Error.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetMessage

> Message GetMessage(context.Background(), messageId).Execute()

Get message



### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
"./buzi"
)

func main() {
    messageId := int64(789) // int64 | ID of pet to return

    configuration := buzi.NewConfiguration(
        buzi.WithBaseURL("example.com"),
    )
    apiClient := buzi.New(configuration)
    resp, err := apiClient.SmsApi.GetMessage(context.Background(), messageId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `SmsApi.GetMessage``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetMessage`: Message
    fmt.Fprintf(os.Stdout, "Response from `SmsApi.GetMessage`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**messageId** | **int64** | ID of pet to return | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetMessageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**Message**](Message.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetNetwork

> Network GetNetwork(context.Background(), networkId).Execute()

Get network



### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
"./buzi"
)

func main() {
    networkId := int32(56) // int32 | 
    opt := buzi.GetNetworkOptions{}

    configuration := buzi.NewConfiguration(
        buzi.WithBaseURL("example.com"),
    )
    apiClient := buzi.New(configuration)
    resp, err := apiClient.SmsApi.GetNetwork(context.Background(), networkId, &opt).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `SmsApi.GetNetwork``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetNetwork`: Network
    fmt.Fprintf(os.Stdout, "Response from `SmsApi.GetNetwork`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**networkId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetNetworkRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **countryCode** | **int64** | ID of pet to return | 

### Return type

[**Network**](Network.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetPricing

> []Pricing GetPricing(context.Background(), networkId).Execute()

List network rates



### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
"./buzi"
)

func main() {
    networkId := int32(56) // int32 | 

    configuration := buzi.NewConfiguration(
        buzi.WithBaseURL("example.com"),
    )
    apiClient := buzi.New(configuration)
    resp, err := apiClient.SmsApi.GetPricing(context.Background(), networkId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `SmsApi.GetPricing``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetPricing`: []Pricing
    fmt.Fprintf(os.Stdout, "Response from `SmsApi.GetPricing`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**networkId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetPricingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**[]Pricing**](Pricing.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListMessages

> []Message ListMessages(context.Background()).Execute()

List messages



### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
"./buzi"
)

func main() {
    opt := buzi.ListMessagesOptions{}

    configuration := buzi.NewConfiguration(
        buzi.WithBaseURL("example.com"),
    )
    apiClient := buzi.New(configuration)
    resp, err := apiClient.SmsApi.ListMessages(context.Background(), &opt).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `SmsApi.ListMessages``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `ListMessages`: []Message
    fmt.Fprintf(os.Stdout, "Response from `SmsApi.ListMessages`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListMessagesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inbox** | **string** |  | 
 **status** | **string** |  | 

### Return type

[**[]Message**](Message.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListNetworks

> []Network ListNetworks(context.Background()).Execute()

List networks



### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
"./buzi"
)

func main() {
    opt := buzi.ListNetworksOptions{}

    configuration := buzi.NewConfiguration(
        buzi.WithBaseURL("example.com"),
    )
    apiClient := buzi.New(configuration)
    resp, err := apiClient.SmsApi.ListNetworks(context.Background(), &opt).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `SmsApi.ListNetworks``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `ListNetworks`: []Network
    fmt.Fprintf(os.Stdout, "Response from `SmsApi.ListNetworks`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListNetworksRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **countryCode** | **string** | ID of pet to return | 

### Return type

[**[]Network**](Network.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SendMessage

> Message SendMessage(context.Background(), messageId).Execute()

Sends a message



### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
"./buzi"
)

func main() {
    messageId := int64(789) // int64 | ID of pet to return

    configuration := buzi.NewConfiguration(
        buzi.WithBaseURL("example.com"),
    )
    apiClient := buzi.New(configuration)
    resp, err := apiClient.SmsApi.SendMessage(context.Background(), messageId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `SmsApi.SendMessage``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `SendMessage`: Message
    fmt.Fprintf(os.Stdout, "Response from `SmsApi.SendMessage`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**messageId** | **int64** | ID of pet to return | 

### Other Parameters

Other parameters are passed through a pointer to a apiSendMessageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**Message**](Message.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

