# sellasist_api.SetsBulkApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**sets_bulk_get**](SetsBulkApi.md#sets_bulk_get) | **GET** /sets_bulk | Zwraca zestawy produktowe
[**sets_bulk_put**](SetsBulkApi.md#sets_bulk_put) | **PUT** /sets_bulk | Masowa aktualizacja zestawów


# **sets_bulk_get**
> object sets_bulk_get(accept=accept)

Zwraca zestawy produktowe

Zwraca zestawy produktowe

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
    api_instance = sellasist_api.SetsBulkApi(api_client)
    accept = 'application/json' # str |  (optional)

    try:
        # Zwraca zestawy produktowe
        api_response = api_instance.sets_bulk_get(accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling SetsBulkApi->sets_bulk_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accept** | **str**|  | [optional] 

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

# **sets_bulk_put**
> sets_bulk_put(content_type=content_type, body=body)

Masowa aktualizacja zestawów

Masowa aktualizacja zestawów

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
    api_instance = sellasist_api.SetsBulkApi(api_client)
    content_type = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Masowa aktualizacja zestawów
        api_instance.sets_bulk_put(content_type=content_type, body=body)
    except ApiException as e:
        print("Exception when calling SetsBulkApi->sets_bulk_put: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **body** | **object**|  | [optional] 

### Return type

void (empty response body)

### Authorization

[apikeyAuth](../README.md#apikeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

