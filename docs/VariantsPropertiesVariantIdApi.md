# sellasist_api.VariantsPropertiesVariantIdApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**variants_properties_variant_id_get**](VariantsPropertiesVariantIdApi.md#variants_properties_variant_id_get) | **GET** /variants_properties/{variant_id} | Zwraca szczegóły właścwiości


# **variants_properties_variant_id_get**
> object variants_properties_variant_id_get(variant_id, accept=accept)

Zwraca szczegóły właścwiości

Zwraca szczegóły właścwiości

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
    api_instance = sellasist_api.VariantsPropertiesVariantIdApi(api_client)
    variant_id = 'variant_id_example' # str | Identyfikator wariantu
accept = 'application/json' # str |  (optional)

    try:
        # Zwraca szczegóły właścwiości
        api_response = api_instance.variants_properties_variant_id_get(variant_id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling VariantsPropertiesVariantIdApi->variants_properties_variant_id_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **variant_id** | **str**| Identyfikator wariantu | 
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

