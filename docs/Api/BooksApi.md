# Bookstore\Client\BooksApi

All URIs are relative to *http://192.168.100.10:8080/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**listBooks**](BooksApi.md#listBooks) | **GET** /books | List of books


# **listBooks**
> \Bookstore\Client\Model\Bookresponse[] listBooks()

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
    $result = $apiInstance->listBooks();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BooksApi->listBooks: ', $e->getMessage(), PHP_EOL;
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

