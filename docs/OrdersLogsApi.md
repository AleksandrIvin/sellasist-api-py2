# sellasist_api.OrdersLogsApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**orders_logs_get**](OrdersLogsApi.md#orders_logs_get) | **GET** /orders_logs | Zwraca listę logów zamówienia


# **orders_logs_get**
> object orders_logs_get(accept=accept, offset=offset, limit=limit, operation_tag=operation_tag, has_operation_tag=has_operation_tag, sort=sort, date_from=date_from, date_to=date_to, orders=orders)

Zwraca listę logów zamówienia

Zwraca listę logów zamówienia

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
    api_instance = sellasist_api.OrdersLogsApi(api_client)
    accept = 'application/json' # str |  (optional)
offset = 4072 # int | Offset (optional)
limit = 4072 # int | Limit (optional)
operation_tag = 'order_edit' # str |  (optional)
has_operation_tag = 'has_operation_tag_example' # str | Posiada operation_tag (true/false) (optional)
sort = 'string' # str | sortowanie asc/desc (optional)
date_from = '2022-11-20 09:08:13' # str | Data akcji od (optional)
date_to = '2022-11-20 09:08:13' # str | Data akcji do (optional)
orders = 'string' # str | Identyfikatory zamówień oddzielone przecinkami (optional)

    try:
        # Zwraca listę logów zamówienia
        api_response = api_instance.orders_logs_get(accept=accept, offset=offset, limit=limit, operation_tag=operation_tag, has_operation_tag=has_operation_tag, sort=sort, date_from=date_from, date_to=date_to, orders=orders)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling OrdersLogsApi->orders_logs_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accept** | **str**|  | [optional] 
 **offset** | **int**| Offset | [optional] 
 **limit** | **int**| Limit | [optional] 
 **operation_tag** | **str**|  | [optional] 
 **has_operation_tag** | **str**| Posiada operation_tag (true/false) | [optional] 
 **sort** | **str**| sortowanie asc/desc | [optional] 
 **date_from** | **str**| Data akcji od | [optional] 
 **date_to** | **str**| Data akcji do | [optional] 
 **orders** | **str**| Identyfikatory zamówień oddzielone przecinkami | [optional] 

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

