# sellasist_api.ProductsVariantsProductVariantIdApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**products_variants_product_variant_id_get**](ProductsVariantsProductVariantIdApi.md#products_variants_product_variant_id_get) | **GET** /products_variants/{product_variant_id} | Zwraca informacje o podanym wariancie produktu
[**products_variants_product_variant_id_put**](ProductsVariantsProductVariantIdApi.md#products_variants_product_variant_id_put) | **PUT** /products_variants/{product_variant_id} | Aktualizacja wariantu produktu


# **products_variants_product_variant_id_get**
> object products_variants_product_variant_id_get(product_variant_id, accept=accept)

Zwraca informacje o podanym wariancie produktu

Zwraca informacje o podanym wariancie produktu

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
    api_instance = sellasist_api.ProductsVariantsProductVariantIdApi(api_client)
    product_variant_id = 4072 # int | Identyfikator wariantu produktu
accept = 'application/json' # str |  (optional)

    try:
        # Zwraca informacje o podanym wariancie produktu
        api_response = api_instance.products_variants_product_variant_id_get(product_variant_id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ProductsVariantsProductVariantIdApi->products_variants_product_variant_id_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **product_variant_id** | **int**| Identyfikator wariantu produktu | 
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

# **products_variants_product_variant_id_put**
> object products_variants_product_variant_id_put(product_variant_id, content_type=content_type, accept=accept, body=body)

Aktualizacja wariantu produktu

Aktualizacja wariantu produktu

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
    api_instance = sellasist_api.ProductsVariantsProductVariantIdApi(api_client)
    product_variant_id = 'product_variant_id_example' # str | Identyfikator wariantu
content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Aktualizacja wariantu produktu
        api_response = api_instance.products_variants_product_variant_id_put(product_variant_id, content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ProductsVariantsProductVariantIdApi->products_variants_product_variant_id_put: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **product_variant_id** | **str**| Identyfikator wariantu | 
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

