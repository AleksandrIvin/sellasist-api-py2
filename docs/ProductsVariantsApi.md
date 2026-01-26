# sellasist_api.ProductsVariantsApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**products_variants_get**](ProductsVariantsApi.md#products_variants_get) | **GET** /products_variants | Zwraca listę wariantów w produktach
[**products_variants_post**](ProductsVariantsApi.md#products_variants_post) | **POST** /products_variants | Tworzenie nowego wariantu w produkcie


# **products_variants_get**
> object products_variants_get(accept=accept, offset=offset, limit=limit, ean=ean, symbol=symbol, catalog_number=catalog_number, auction_id=auction_id)

Zwraca listę wariantów w produktach

Zwraca listę wariantów w produktach

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
    api_instance = sellasist_api.ProductsVariantsApi(api_client)
    accept = 'application/json' # str |  (optional)
offset = 4072 # int | Offset (optional)
limit = 4072 # int | Limit (optional)
ean = 'string' # str | Kod EAN (optional)
symbol = 'string' # str | Symbol wariantu (optional)
catalog_number = 'string' # str | Numer katalogowy wariantu (optional)
auction_id = 'string' # str | Identyfikator w portalach aukcyjnych (optional)

    try:
        # Zwraca listę wariantów w produktach
        api_response = api_instance.products_variants_get(accept=accept, offset=offset, limit=limit, ean=ean, symbol=symbol, catalog_number=catalog_number, auction_id=auction_id)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ProductsVariantsApi->products_variants_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accept** | **str**|  | [optional] 
 **offset** | **int**| Offset | [optional] 
 **limit** | **int**| Limit | [optional] 
 **ean** | **str**| Kod EAN | [optional] 
 **symbol** | **str**| Symbol wariantu | [optional] 
 **catalog_number** | **str**| Numer katalogowy wariantu | [optional] 
 **auction_id** | **str**| Identyfikator w portalach aukcyjnych | [optional] 

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

# **products_variants_post**
> object products_variants_post(content_type=content_type, accept=accept, body=body)

Tworzenie nowego wariantu w produkcie

Tworzenie nowego wariantu w produkcie

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
    api_instance = sellasist_api.ProductsVariantsApi(api_client)
    content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Tworzenie nowego wariantu w produkcie
        api_response = api_instance.products_variants_post(content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ProductsVariantsApi->products_variants_post: %s\n" % e)
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

