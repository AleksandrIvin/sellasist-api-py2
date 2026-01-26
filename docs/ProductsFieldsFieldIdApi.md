# sellasist_api.ProductsFieldsFieldIdApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**products_fields_field_id_delete**](ProductsFieldsFieldIdApi.md#products_fields_field_id_delete) | **DELETE** /products_fields/{field_id} | Usunięcie pola
[**products_fields_field_id_get**](ProductsFieldsFieldIdApi.md#products_fields_field_id_get) | **GET** /products_fields/{field_id} | Pobieranie informacji o dodatkowym polu
[**products_fields_field_id_put**](ProductsFieldsFieldIdApi.md#products_fields_field_id_put) | **PUT** /products_fields/{field_id} | Aktualizacja właściwości dodatkowego pola


# **products_fields_field_id_delete**
> object products_fields_field_id_delete(field_id, accept=accept)

Usunięcie pola

Usunięcie pola

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
    api_instance = sellasist_api.ProductsFieldsFieldIdApi(api_client)
    field_id = 'field_id_example' # str | Identyfikator dodatkowego pola
accept = 'application/json' # str |  (optional)

    try:
        # Usunięcie pola
        api_response = api_instance.products_fields_field_id_delete(field_id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ProductsFieldsFieldIdApi->products_fields_field_id_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **field_id** | **str**| Identyfikator dodatkowego pola | 
 **accept** | **str**|  | [optional] 

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **products_fields_field_id_get**
> object products_fields_field_id_get(field_id, accept=accept)

Pobieranie informacji o dodatkowym polu

Pobieranie informacji o dodatkowym polu

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
    api_instance = sellasist_api.ProductsFieldsFieldIdApi(api_client)
    field_id = 'field_id_example' # str | Identyfikator dodatkowego pola
accept = 'application/json' # str |  (optional)

    try:
        # Pobieranie informacji o dodatkowym polu
        api_response = api_instance.products_fields_field_id_get(field_id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ProductsFieldsFieldIdApi->products_fields_field_id_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **field_id** | **str**| Identyfikator dodatkowego pola | 
 **accept** | **str**|  | [optional] 

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **products_fields_field_id_put**
> object products_fields_field_id_put(field_id, content_type=content_type, accept=accept, body=body)

Aktualizacja właściwości dodatkowego pola

Aktualizacja właściwości dodatkowego pola

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
    api_instance = sellasist_api.ProductsFieldsFieldIdApi(api_client)
    field_id = 'field_id_example' # str | Identyfikator dodatkowego pola
content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Aktualizacja właściwości dodatkowego pola
        api_response = api_instance.products_fields_field_id_put(field_id, content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ProductsFieldsFieldIdApi->products_fields_field_id_put: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **field_id** | **str**| Identyfikator dodatkowego pola | 
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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

