# sellasist_api.ImagesProductIdApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**images_product_id_get**](ImagesProductIdApi.md#images_product_id_get) | **GET** /images/{product_id} | Zwraca obrazy dla danego produktu


# **images_product_id_get**
> object images_product_id_get(product_id, accept=accept)

Zwraca obrazy dla danego produktu

Zwraca obrazy dla danego produktu

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
    api_instance = sellasist_api.ImagesProductIdApi(api_client)
    product_id = 'product_id_example' # str | Identyfikator produktu
accept = 'application/json' # str |  (optional)

    try:
        # Zwraca obrazy dla danego produktu
        api_response = api_instance.images_product_id_get(product_id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ImagesProductIdApi->images_product_id_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **product_id** | **str**| Identyfikator produktu | 
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

