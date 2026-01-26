# sellasist_api.ProductsApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**products_get**](ProductsApi.md#products_get) | **GET** /products | Zwraca listę produktów
[**products_post**](ProductsApi.md#products_post) | **POST** /products | Tworzenie nowego produktu


# **products_get**
> object products_get(accept=accept, offset=offset, limit=limit, ean=ean, symbol=symbol, catalog_number=catalog_number, from_id=from_id, auction_id=auction_id, sort=sort)

Zwraca listę produktów

Zwraca listę produktów

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
    api_instance = sellasist_api.ProductsApi(api_client)
    accept = 'application/json' # str |  (optional)
offset = 4072 # int | Offset (optional)
limit = 4072 # int | Limit (optional)
ean = 'string' # str | Kod EAN (optional)
symbol = 'string' # str | Symbol Produktu (optional)
catalog_number = 'string' # str | Numer katalogowy produktu (optional)
from_id = 4072 # int | Numer ID produktu(zostaną zwrócone produkty z wyższym numerem niż podany parametr) (optional)
auction_id = 'string' # str | Identyfikator w portalach aukcyjnych (optional)
sort = 'string' # str | Sortowanie (asc/desc), domyślnie desc (optional)

    try:
        # Zwraca listę produktów
        api_response = api_instance.products_get(accept=accept, offset=offset, limit=limit, ean=ean, symbol=symbol, catalog_number=catalog_number, from_id=from_id, auction_id=auction_id, sort=sort)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ProductsApi->products_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accept** | **str**|  | [optional] 
 **offset** | **int**| Offset | [optional] 
 **limit** | **int**| Limit | [optional] 
 **ean** | **str**| Kod EAN | [optional] 
 **symbol** | **str**| Symbol Produktu | [optional] 
 **catalog_number** | **str**| Numer katalogowy produktu | [optional] 
 **from_id** | **int**| Numer ID produktu(zostaną zwrócone produkty z wyższym numerem niż podany parametr) | [optional] 
 **auction_id** | **str**| Identyfikator w portalach aukcyjnych | [optional] 
 **sort** | **str**| Sortowanie (asc/desc), domyślnie desc | [optional] 

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

# **products_post**
> object products_post(content_type=content_type, accept=accept, body=body)

Tworzenie nowego produktu

Tworzenie nowego produktu

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
    api_instance = sellasist_api.ProductsApi(api_client)
    content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Tworzenie nowego produktu
        api_response = api_instance.products_post(content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ProductsApi->products_post: %s\n" % e)
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

