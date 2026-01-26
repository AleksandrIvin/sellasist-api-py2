# sellasist_api.OptionsPropertiesOptionIdApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**options_properties_option_id_get**](OptionsPropertiesOptionIdApi.md#options_properties_option_id_get) | **GET** /options_properties/{option_id} | Zwraca szczegóły właściwości


# **options_properties_option_id_get**
> object options_properties_option_id_get(option_id, accept=accept)

Zwraca szczegóły właściwości

Zwraca szczegóły właściwości

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
    api_instance = sellasist_api.OptionsPropertiesOptionIdApi(api_client)
    option_id = 'option_id_example' # str | Identyfikator opcji
accept = 'application/json' # str |  (optional)

    try:
        # Zwraca szczegóły właściwości
        api_response = api_instance.options_properties_option_id_get(option_id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling OptionsPropertiesOptionIdApi->options_properties_option_id_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **option_id** | **str**| Identyfikator opcji | 
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

