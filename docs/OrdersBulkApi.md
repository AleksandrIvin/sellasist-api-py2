# sellasist_api.OrdersBulkApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**orders_bulk_put**](OrdersBulkApi.md#orders_bulk_put) | **PUT** /orders_bulk | Masowa aktualizacja zamówień


# **orders_bulk_put**
> object orders_bulk_put(content_type=content_type, accept=accept, body=body)

Masowa aktualizacja zamówień

Masowa aktualizacja zamówień

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
    api_instance = sellasist_api.OrdersBulkApi(api_client)
    content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Masowa aktualizacja zamówień
        api_response = api_instance.orders_bulk_put(content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling OrdersBulkApi->orders_bulk_put: %s\n" % e)
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

