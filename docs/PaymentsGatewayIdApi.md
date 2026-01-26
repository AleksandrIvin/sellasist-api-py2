# sellasist_api.PaymentsGatewayIdApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**payments_gateway_id_delete**](PaymentsGatewayIdApi.md#payments_gateway_id_delete) | **DELETE** /payments/{gateway_id} | Usuwa dany kanał płatności
[**payments_gateway_id_get**](PaymentsGatewayIdApi.md#payments_gateway_id_get) | **GET** /payments/{gateway_id} | Zwraca szczegóły o danym kanale płatności
[**payments_gateway_id_put**](PaymentsGatewayIdApi.md#payments_gateway_id_put) | **PUT** /payments/{gateway_id} | Aktualizuje dany kanał płatności


# **payments_gateway_id_delete**
> object payments_gateway_id_delete(gateway_id, accept=accept)

Usuwa dany kanał płatności

Usuwa dany kanał płatności

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
    api_instance = sellasist_api.PaymentsGatewayIdApi(api_client)
    gateway_id = 'gateway_id_example' # str | Identyfikator kanału płatności
accept = 'application/json' # str |  (optional)

    try:
        # Usuwa dany kanał płatności
        api_response = api_instance.payments_gateway_id_delete(gateway_id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling PaymentsGatewayIdApi->payments_gateway_id_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **gateway_id** | **str**| Identyfikator kanału płatności | 
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

# **payments_gateway_id_get**
> object payments_gateway_id_get(gateway_id, accept=accept)

Zwraca szczegóły o danym kanale płatności

Zwraca szczegóły o danym kanale płatności

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
    api_instance = sellasist_api.PaymentsGatewayIdApi(api_client)
    gateway_id = 'gateway_id_example' # str | Identyfikator kanału płatności
accept = 'application/json' # str |  (optional)

    try:
        # Zwraca szczegóły o danym kanale płatności
        api_response = api_instance.payments_gateway_id_get(gateway_id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling PaymentsGatewayIdApi->payments_gateway_id_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **gateway_id** | **str**| Identyfikator kanału płatności | 
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

# **payments_gateway_id_put**
> object payments_gateway_id_put(gateway_id, content_type=content_type, accept=accept, body=body)

Aktualizuje dany kanał płatności

Aktualizuje dany kanał płatności

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
    api_instance = sellasist_api.PaymentsGatewayIdApi(api_client)
    gateway_id = 'gateway_id_example' # str | Identyfikator kanału płatności
content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Aktualizuje dany kanał płatności
        api_response = api_instance.payments_gateway_id_put(gateway_id, content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling PaymentsGatewayIdApi->payments_gateway_id_put: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **gateway_id** | **str**| Identyfikator kanału płatności | 
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
**404** | Not Found |  * Content-Type -  <br>  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

