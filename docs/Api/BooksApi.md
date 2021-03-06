# Bookstore\Client\BooksApi

All URIs are relative to *http://192.168.100.10:8080/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addBook**](BooksApi.md#addBook) | **POST** /books | Creates a new book
[**deleteBook**](BooksApi.md#deleteBook) | **DELETE** /books/{id} | 
[**findBook**](BooksApi.md#findBook) | **GET** /books/{id} | get book by id
[**listBook**](BooksApi.md#listBook) | **GET** /books | List of books
[**updateBook**](BooksApi.md#updateBook) | **PUT** /books/{id} | 


# **addBook**
> addBook($newbook)

Creates a new book

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Bookstore\Client\Api\BooksApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$newbook = new \Bookstore\Client\Model\Newbook(); // \Bookstore\Client\Model\Newbook | Book to add to the store

try {
    $apiInstance->addBook($newbook);
} catch (Exception $e) {
    echo 'Exception when calling BooksApi->addBook: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **newbook** | [**\Bookstore\Client\Model\Newbook**](../Model/Newbook.md)| Book to add to the store |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteBook**
> deleteBook($id)



Updates a book

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Bookstore\Client\Api\BooksApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id = 56; // int | ID of book to update

try {
    $apiInstance->deleteBook($id);
} catch (Exception $e) {
    echo 'Exception when calling BooksApi->deleteBook: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ID of book to update |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **findBook**
> \Bookstore\Client\Model\Bookresponse findBook($id)

get book by id

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Bookstore\Client\Api\BooksApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id = 56; // int | ID of book to fetch

try {
    $result = $apiInstance->findBook($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BooksApi->findBook: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ID of book to fetch |

### Return type

[**\Bookstore\Client\Model\Bookresponse**](../Model/Bookresponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listBook**
> \Bookstore\Client\Model\Bookresponse[] listBook()

List of books

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Bookstore\Client\Api\BooksApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->listBook();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BooksApi->listBook: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Bookstore\Client\Model\Bookresponse[]**](../Model/Bookresponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateBook**
> updateBook($id, $newbook)



Updates a book

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Bookstore\Client\Api\BooksApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id = 56; // int | ID of book to update
$newbook = new \Bookstore\Client\Model\Newbook(); // \Bookstore\Client\Model\Newbook | Book to update

try {
    $apiInstance->updateBook($id, $newbook);
} catch (Exception $e) {
    echo 'Exception when calling BooksApi->updateBook: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ID of book to update |
 **newbook** | [**\Bookstore\Client\Model\Newbook**](../Model/Newbook.md)| Book to update |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

