# sellasist_api.ProductsBulkApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**products_bulk_get**](ProductsBulkApi.md#products_bulk_get) | **GET** /products_bulk | Zwraca informację o stanach magazynowych
[**products_bulk_put**](ProductsBulkApi.md#products_bulk_put) | **PUT** /products_bulk | Masowa aktualizacja produktów


# **products_bulk_get**
> object products_bulk_get(accept=accept, offset=offset, limit=limit)

Zwraca informację o stanach magazynowych

Zwraca informację o stanach magazynowych

### Example

```python
from __future__ import print_function
import time
import sellasist_api
from sellasist_api.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://}
# See configuration.py for a list of all supported configuration parameters.
configuration = sellasist_api.Configuration(
    host = "http://}"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Enter a context with an instance of the API client
with sellasist_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = sellasist_api.ProductsBulkApi(api_client)
    accept = 'application/json' # str |  (optional)
offset = 4072 # int | Offset (optional)
limit = 4072 # int | Limit (optional)

    try:
        # Zwraca informację o stanach magazynowych
        api_response = api_instance.products_bulk_get(accept=accept, offset=offset, limit=limit)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ProductsBulkApi->products_bulk_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accept** | **str**|  | [optional] 
 **offset** | **int**| Offset | [optional] 
 **limit** | **int**| Limit | [optional] 

### Return type

**object**

### Authorization

[apikeyAuth](../README.md#apikeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  * Content-Type -  <br>  |
**401** | Unauthorized |  * Content-Type -  <br>  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **products_bulk_put**
> object products_bulk_put(content_type=content_type, accept=accept, body=body)

Masowa aktualizacja produktów

Masowa aktualizacja produktów

### Example

```python
from __future__ import print_function
import time
import sellasist_api
from sellasist_api.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://}
# See configuration.py for a list of all supported configuration parameters.
configuration = sellasist_api.Configuration(
    host = "http://}"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Enter a context with an instance of the API client
with sellasist_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = sellasist_api.ProductsBulkApi(api_client)
    content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Masowa aktualizacja produktów
        api_response = api_instance.products_bulk_put(content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ProductsBulkApi->products_bulk_put: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **accept** | **str**|  | [optional] 
 **body** | **object**|  | [optional] 

### Return type

**object**

### Authorization

[apikeyAuth](../README.md#apikeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  * Content-Type -  <br>  |
**400** | Bad Request |  * Content-Type -  <br>  |
**401** | Unauthorized |  * Content-Type -  <br>  |
**413** | Request Entity Too Large |  * Content-Type -  <br>  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

