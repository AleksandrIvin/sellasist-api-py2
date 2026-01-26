# sellasist_api.OrdersFieldsFieldIdApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**orders_fields_field_id_delete**](OrdersFieldsFieldIdApi.md#orders_fields_field_id_delete) | **DELETE** /orders_fields/{field_id} | Usunięcie pola
[**orders_fields_field_id_get**](OrdersFieldsFieldIdApi.md#orders_fields_field_id_get) | **GET** /orders_fields/{field_id} | Pobieranie informacji o dodatkowym polu
[**orders_fields_field_id_put**](OrdersFieldsFieldIdApi.md#orders_fields_field_id_put) | **PUT** /orders_fields/{field_id} | Aktualizacja właściwości dodatkowego pola


# **orders_fields_field_id_delete**
> object orders_fields_field_id_delete(field_id, accept=accept)

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
    api_instance = sellasist_api.OrdersFieldsFieldIdApi(api_client)
    field_id = 'field_id_example' # str | Identyfikator dodatkowego pola
accept = 'application/json' # str |  (optional)

    try:
        # Usunięcie pola
        api_response = api_instance.orders_fields_field_id_delete(field_id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling OrdersFieldsFieldIdApi->orders_fields_field_id_delete: %s\n" % e)
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

# **orders_fields_field_id_get**
> object orders_fields_field_id_get(field_id, accept=accept)

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
    api_instance = sellasist_api.OrdersFieldsFieldIdApi(api_client)
    field_id = 'field_id_example' # str | Identyfikator dodatkowego pola
accept = 'application/json' # str |  (optional)

    try:
        # Pobieranie informacji o dodatkowym polu
        api_response = api_instance.orders_fields_field_id_get(field_id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling OrdersFieldsFieldIdApi->orders_fields_field_id_get: %s\n" % e)
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

# **orders_fields_field_id_put**
> object orders_fields_field_id_put(field_id, content_type=content_type, accept=accept, body=body)

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
    api_instance = sellasist_api.OrdersFieldsFieldIdApi(api_client)
    field_id = 'field_id_example' # str | Identyfikator dodatkowego pola
content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Aktualizacja właściwości dodatkowego pola
        api_response = api_instance.orders_fields_field_id_put(field_id, content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling OrdersFieldsFieldIdApi->orders_fields_field_id_put: %s\n" % e)
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

