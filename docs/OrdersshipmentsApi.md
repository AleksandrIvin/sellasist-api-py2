# sellasist_api.OrdersshipmentsApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ordersshipments_get**](OrdersshipmentsApi.md#ordersshipments_get) | **GET** /ordersshipments | Zwraca listę listów przewozowych
[**ordersshipments_post**](OrdersshipmentsApi.md#ordersshipments_post) | **POST** /ordersshipments | Tworzy list przewozowy


# **ordersshipments_get**
> object ordersshipments_get(accept=accept, offset=offset, limit=limit, order_id=order_id, sort=sort, date_from=date_from, date_to=date_to)

Zwraca listę listów przewozowych

Zwraca listę listów przewozowych

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
    api_instance = sellasist_api.OrdersshipmentsApi(api_client)
    accept = 'application/json' # str |  (optional)
offset = 4072 # int | Offset (optional)
limit = 4072 # int | Limit (optional)
order_id = 4072 # int | Identyfikator zamówienia (optional)
sort = 'string' # str | sortowanie asc/desc (optional)
date_from = '2022-11-20 09:08:13' # str | Data utworzenia od (optional)
date_to = '2022-11-20 09:08:13' # str | Data utworzenia do (optional)

    try:
        # Zwraca listę listów przewozowych
        api_response = api_instance.ordersshipments_get(accept=accept, offset=offset, limit=limit, order_id=order_id, sort=sort, date_from=date_from, date_to=date_to)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling OrdersshipmentsApi->ordersshipments_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accept** | **str**|  | [optional] 
 **offset** | **int**| Offset | [optional] 
 **limit** | **int**| Limit | [optional] 
 **order_id** | **int**| Identyfikator zamówienia | [optional] 
 **sort** | **str**| sortowanie asc/desc | [optional] 
 **date_from** | **str**| Data utworzenia od | [optional] 
 **date_to** | **str**| Data utworzenia do | [optional] 

### Return type

**object**

### Authorization

[apikeyAuth](../README.md#apikeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/plain

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  * Content-Type -  <br>  |
**401** | Unauthorized |  * Content-Type -  <br>  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ordersshipments_post**
> object ordersshipments_post(content_type=content_type, accept=accept, body=body)

Tworzy list przewozowy

Tworzy list przewozowy

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
    api_instance = sellasist_api.OrdersshipmentsApi(api_client)
    content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Tworzy list przewozowy
        api_response = api_instance.ordersshipments_post(content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling OrdersshipmentsApi->ordersshipments_post: %s\n" % e)
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
**401** | Unauthorized |  * Content-Type -  <br>  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

