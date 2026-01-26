# sellasist_api.CorrectsCorrectIdApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**corrects_correct_id_delete**](CorrectsCorrectIdApi.md#corrects_correct_id_delete) | **DELETE** /corrects/{correct_id} | Usunięcie faktury
[**corrects_correct_id_get**](CorrectsCorrectIdApi.md#corrects_correct_id_get) | **GET** /corrects/{correct_id} | Zwraca informacje o wybranej fakturze
[**corrects_correct_id_put**](CorrectsCorrectIdApi.md#corrects_correct_id_put) | **PUT** /corrects/{correct_id} | Aktualizacja faktury


# **corrects_correct_id_delete**
> object corrects_correct_id_delete(correct_id, accept=accept)

Usunięcie faktury

Usunięcie faktury

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
    api_instance = sellasist_api.CorrectsCorrectIdApi(api_client)
    correct_id = 'correct_id_example' # str | Identyfikator faktury
accept = 'application/json' # str |  (optional)

    try:
        # Usunięcie faktury
        api_response = api_instance.corrects_correct_id_delete(correct_id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling CorrectsCorrectIdApi->corrects_correct_id_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **correct_id** | **str**| Identyfikator faktury | 
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

# **corrects_correct_id_get**
> object corrects_correct_id_get(correct_id, accept=accept)

Zwraca informacje o wybranej fakturze

Zwraca informacje o wybranej fakturze

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
    api_instance = sellasist_api.CorrectsCorrectIdApi(api_client)
    correct_id = 'correct_id_example' # str | Identyfikator faktury
accept = 'application/json' # str |  (optional)

    try:
        # Zwraca informacje o wybranej fakturze
        api_response = api_instance.corrects_correct_id_get(correct_id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling CorrectsCorrectIdApi->corrects_correct_id_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **correct_id** | **str**| Identyfikator faktury | 
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

# **corrects_correct_id_put**
> object corrects_correct_id_put(correct_id, content_type=content_type, accept=accept, body=body)

Aktualizacja faktury

Aktualizacja faktury

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
    api_instance = sellasist_api.CorrectsCorrectIdApi(api_client)
    correct_id = 'correct_id_example' # str | Identyfikator faktury
content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Aktualizacja faktury
        api_response = api_instance.corrects_correct_id_put(correct_id, content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling CorrectsCorrectIdApi->corrects_correct_id_put: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **correct_id** | **str**| Identyfikator faktury | 
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

