# \MovieWatchlistApi

All URIs are relative to *https://d01aws001.fts.d-3.de/microservicetemplate*

Method | HTTP request | Description
------------- | ------------- | -------------
[**MoviesGet**](MovieWatchlistApi.md#MoviesGet) | **Get** /movies | Return all movies
[**MoviesIdDelete**](MovieWatchlistApi.md#MoviesIdDelete) | **Delete** /movies/{id} | Delete an movie by ID
[**MoviesIdGet**](MovieWatchlistApi.md#MoviesIdGet) | **Get** /movies/{id} | Returns an movie by ID
[**MoviesIdPut**](MovieWatchlistApi.md#MoviesIdPut) | **Put** /movies/{id} | Update an movie by ID
[**MoviesPost**](MovieWatchlistApi.md#MoviesPost) | **Post** /movies | Create a new movie



## MoviesGet

> []Movie MoviesGet(ctx).Execute()

Return all movies

### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    openapiclient "./openapi"
)

func main() {

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.MovieWatchlistApi.MoviesGet(context.Background()).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `MovieWatchlistApi.MoviesGet``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `MoviesGet`: []Movie
    fmt.Fprintf(os.Stdout, "Response from `MovieWatchlistApi.MoviesGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiMoviesGetRequest struct via the builder pattern


### Return type

[**[]Movie**](Movie.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MoviesIdDelete

> MoviesIdDelete(ctx, id).Execute()

Delete an movie by ID

### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    openapiclient "./openapi"
)

func main() {
    id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | ID of movie

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.MovieWatchlistApi.MoviesIdDelete(context.Background(), id).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `MovieWatchlistApi.MoviesIdDelete``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | ID of movie | 

### Other Parameters

Other parameters are passed through a pointer to a apiMoviesIdDeleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MoviesIdGet

> Movie MoviesIdGet(ctx, id).Execute()

Returns an movie by ID

### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    openapiclient "./openapi"
)

func main() {
    id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | ID of movie

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.MovieWatchlistApi.MoviesIdGet(context.Background(), id).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `MovieWatchlistApi.MoviesIdGet``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `MoviesIdGet`: Movie
    fmt.Fprintf(os.Stdout, "Response from `MovieWatchlistApi.MoviesIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | ID of movie | 

### Other Parameters

Other parameters are passed through a pointer to a apiMoviesIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**Movie**](Movie.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MoviesIdPut

> Movie MoviesIdPut(ctx, id).Movie(movie).Execute()

Update an movie by ID

### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    openapiclient "./openapi"
)

func main() {
    id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | ID of movie
    movie := *openapiclient.NewMovie("Id_example", "Name_example", "Genre_example", "Director_example", []string{"Actors_example"}, "Description_example", "Type_example") // Movie | Updated movie

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.MovieWatchlistApi.MoviesIdPut(context.Background(), id).Movie(movie).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `MovieWatchlistApi.MoviesIdPut``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `MoviesIdPut`: Movie
    fmt.Fprintf(os.Stdout, "Response from `MovieWatchlistApi.MoviesIdPut`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | ID of movie | 

### Other Parameters

Other parameters are passed through a pointer to a apiMoviesIdPutRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **movie** | [**Movie**](Movie.md) | Updated movie | 

### Return type

[**Movie**](Movie.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MoviesPost

> Movie MoviesPost(ctx).Movie(movie).Execute()

Create a new movie

### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    openapiclient "./openapi"
)

func main() {
    movie := *openapiclient.NewMovie("Id_example", "Name_example", "Genre_example", "Director_example", []string{"Actors_example"}, "Description_example", "Type_example") // Movie | Movie to storage

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.MovieWatchlistApi.MoviesPost(context.Background()).Movie(movie).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `MovieWatchlistApi.MoviesPost``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `MoviesPost`: Movie
    fmt.Fprintf(os.Stdout, "Response from `MovieWatchlistApi.MoviesPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiMoviesPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **movie** | [**Movie**](Movie.md) | Movie to storage | 

### Return type

[**Movie**](Movie.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

