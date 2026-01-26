# sellasist_api.CategoriesCategoryIdApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**categories_category_id_delete**](CategoriesCategoryIdApi.md#categories_category_id_delete) | **DELETE** /categories/{category_id} | Usuwa daną kategorię
[**categories_category_id_get**](CategoriesCategoryIdApi.md#categories_category_id_get) | **GET** /categories/{category_id} | Zwraca szczegóły kategorii
[**categories_category_id_put**](CategoriesCategoryIdApi.md#categories_category_id_put) | **PUT** /categories/{category_id} | Aktualizuje kategorię w oparciu o id


# **categories_category_id_delete**
> object categories_category_id_delete(category_id, accept=accept)

Usuwa daną kategorię

Usuwa daną kategorię

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
    api_instance = sellasist_api.CategoriesCategoryIdApi(api_client)
    category_id = 'category_id_example' # str | Identyfikator kategorii
accept = 'application/json' # str |  (optional)

    try:
        # Usuwa daną kategorię
        api_response = api_instance.categories_category_id_delete(category_id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling CategoriesCategoryIdApi->categories_category_id_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **category_id** | **str**| Identyfikator kategorii | 
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

# **categories_category_id_get**
> object categories_category_id_get(category_id, accept=accept)

Zwraca szczegóły kategorii

Zwraca szczegóły kategorii

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
    api_instance = sellasist_api.CategoriesCategoryIdApi(api_client)
    category_id = 'category_id_example' # str | Identyfikator kategorii
accept = 'application/json' # str |  (optional)

    try:
        # Zwraca szczegóły kategorii
        api_response = api_instance.categories_category_id_get(category_id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling CategoriesCategoryIdApi->categories_category_id_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **category_id** | **str**| Identyfikator kategorii | 
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

# **categories_category_id_put**
> object categories_category_id_put(category_id, content_type=content_type, accept=accept, body=body)

Aktualizuje kategorię w oparciu o id

Aktualizuje kategorię w oparciu o id

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
    api_instance = sellasist_api.CategoriesCategoryIdApi(api_client)
    category_id = 'category_id_example' # str | Identyfikator kategorii
content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Aktualizuje kategorię w oparciu o id
        api_response = api_instance.categories_category_id_put(category_id, content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling CategoriesCategoryIdApi->categories_category_id_put: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **category_id** | **str**| Identyfikator kategorii | 
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
**404** | Not Found |  * Content-Type -  <br>  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

