# sellasist_api.SetsMainProductIdApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**sets_main_product_id_get**](SetsMainProductIdApi.md#sets_main_product_id_get) | **GET** /sets/{main_product_id} | Zwraca szczegóły zestawu
[**sets_main_product_id_post**](SetsMainProductIdApi.md#sets_main_product_id_post) | **POST** /sets/{main_product_id} | Dodaje produkty do wskazanego zestawu
[**sets_main_product_id_put**](SetsMainProductIdApi.md#sets_main_product_id_put) | **PUT** /sets/{main_product_id} | Aktualizuje powiązania we wskazanym zestawie


# **sets_main_product_id_get**
> object sets_main_product_id_get(main_product_id, accept=accept)

Zwraca szczegóły zestawu

Zwraca szczegóły zestawu

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
    api_instance = sellasist_api.SetsMainProductIdApi(api_client)
    main_product_id = 'main_product_id_example' # str | Identyfikator zestawu - produktu
accept = 'application/json' # str |  (optional)

    try:
        # Zwraca szczegóły zestawu
        api_response = api_instance.sets_main_product_id_get(main_product_id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling SetsMainProductIdApi->sets_main_product_id_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **main_product_id** | **str**| Identyfikator zestawu - produktu | 
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

# **sets_main_product_id_post**
> object sets_main_product_id_post(main_product_id, content_type=content_type, accept=accept, body=body)

Dodaje produkty do wskazanego zestawu

Dodaje produkty do wskazanego zestawu

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
    api_instance = sellasist_api.SetsMainProductIdApi(api_client)
    main_product_id = 'main_product_id_example' # str | Identyfikator zestawu - produktu
content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Dodaje produkty do wskazanego zestawu
        api_response = api_instance.sets_main_product_id_post(main_product_id, content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling SetsMainProductIdApi->sets_main_product_id_post: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **main_product_id** | **str**| Identyfikator zestawu - produktu | 
 **content_type** | **str**|  | [optional] 
 **accept** | **str**|  | [optional] 
 **body** | **object**|  | [optional] 

### Return type

**object**

### Authorization

[apikeyAuth](../README.md#apikeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/plain

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  * Content-Type -  <br>  |
**401** | Unauthorized |  * Content-Type -  <br>  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **sets_main_product_id_put**
> object sets_main_product_id_put(main_product_id, content_type=content_type, accept=accept, body=body)

Aktualizuje powiązania we wskazanym zestawie

Aktualizuje powiązania we wskazanym zestawie

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
    api_instance = sellasist_api.SetsMainProductIdApi(api_client)
    main_product_id = 'main_product_id_example' # str | Identyfikator zestawu - produktu
content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Aktualizuje powiązania we wskazanym zestawie
        api_response = api_instance.sets_main_product_id_put(main_product_id, content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling SetsMainProductIdApi->sets_main_product_id_put: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **main_product_id** | **str**| Identyfikator zestawu - produktu | 
 **content_type** | **str**|  | [optional] 
 **accept** | **str**|  | [optional] 
 **body** | **object**|  | [optional] 

### Return type

**object**

### Authorization

[apikeyAuth](../README.md#apikeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/plain

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  * Content-Type -  <br>  |
**401** | Unauthorized |  * Content-Type -  <br>  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

