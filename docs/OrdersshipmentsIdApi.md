# sellasist_api.OrdersshipmentsIdApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ordersshipments_id_delete**](OrdersshipmentsIdApi.md#ordersshipments_id_delete) | **DELETE** /ordersshipments/{id} | Usuwa list przewozowy
[**ordersshipments_id_get**](OrdersshipmentsIdApi.md#ordersshipments_id_get) | **GET** /ordersshipments/{id} | Zwraca list przewozowy
[**ordersshipments_id_put**](OrdersshipmentsIdApi.md#ordersshipments_id_put) | **PUT** /ordersshipments/{id} | Aktualizuje list przewozowy


# **ordersshipments_id_delete**
> object ordersshipments_id_delete(id, accept=accept)

Usuwa list przewozowy

Usuwa list przewozowy

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
    api_instance = sellasist_api.OrdersshipmentsIdApi(api_client)
    id = 'id_example' # str | Identyfikator listu przewozowego
accept = 'application/json' # str |  (optional)

    try:
        # Usuwa list przewozowy
        api_response = api_instance.ordersshipments_id_delete(id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling OrdersshipmentsIdApi->ordersshipments_id_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| Identyfikator listu przewozowego | 
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
**401** | Unauthorized |  * Content-Type -  <br>  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ordersshipments_id_get**
> object ordersshipments_id_get(id, accept=accept)

Zwraca list przewozowy

Zwraca list przewozowy

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
    api_instance = sellasist_api.OrdersshipmentsIdApi(api_client)
    id = 'id_example' # str | Identyfikator listu przewozowego
accept = 'application/json' # str |  (optional)

    try:
        # Zwraca list przewozowy
        api_response = api_instance.ordersshipments_id_get(id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling OrdersshipmentsIdApi->ordersshipments_id_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| Identyfikator listu przewozowego | 
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
**401** | Unauthorized |  * Content-Type -  <br>  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ordersshipments_id_put**
> object ordersshipments_id_put(id, content_type=content_type, accept=accept, body=body)

Aktualizuje list przewozowy

Aktualizuje list przewozowy

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
    api_instance = sellasist_api.OrdersshipmentsIdApi(api_client)
    id = 'id_example' # str | Identyfikator listu przewozowego
content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Aktualizuje list przewozowy
        api_response = api_instance.ordersshipments_id_put(id, content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling OrdersshipmentsIdApi->ordersshipments_id_put: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| Identyfikator listu przewozowego | 
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
**401** | Unauthorized |  * Content-Type -  <br>  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

