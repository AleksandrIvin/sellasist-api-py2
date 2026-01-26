# sellasist_api.ReturnsApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**returns_get**](ReturnsApi.md#returns_get) | **GET** /returns | Zwraca listę wszystkich zwrotów


# **returns_get**
> object returns_get(accept=accept, order_id=order_id, source_id=source_id, offset=offset, limit=limit, sort=sort, date_from=date_from, date_to=date_to)

Zwraca listę wszystkich zwrotów

Zwraca listę wszystkich zwrotów

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
    api_instance = sellasist_api.ReturnsApi(api_client)
    accept = 'application/json' # str |  (optional)
order_id = 4072 # int | numer zamówienia (optional)
source_id = 4072 # int | numer źródła (optional)
offset = 4072 # int | Offset (optional)
limit = 4072 # int | Limit (optional)
sort = 'string' # str | sortowanie asc/desc (optional)
date_from = '2022-11-20 09:08:13' # str | Data akcji od (optional)
date_to = '2022-11-20 09:08:13' # str | Data akcji do (optional)

    try:
        # Zwraca listę wszystkich zwrotów
        api_response = api_instance.returns_get(accept=accept, order_id=order_id, source_id=source_id, offset=offset, limit=limit, sort=sort, date_from=date_from, date_to=date_to)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ReturnsApi->returns_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accept** | **str**|  | [optional] 
 **order_id** | **int**| numer zamówienia | [optional] 
 **source_id** | **int**| numer źródła | [optional] 
 **offset** | **int**| Offset | [optional] 
 **limit** | **int**| Limit | [optional] 
 **sort** | **str**| sortowanie asc/desc | [optional] 
 **date_from** | **str**| Data akcji od | [optional] 
 **date_to** | **str**| Data akcji do | [optional] 

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

