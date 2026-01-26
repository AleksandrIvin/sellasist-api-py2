# sellasist_api.StoragesStorageIdApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**storages_storage_id_delete**](StoragesStorageIdApi.md#storages_storage_id_delete) | **DELETE** /storages/{storage_id} | Usuwa magazyn
[**storages_storage_id_get**](StoragesStorageIdApi.md#storages_storage_id_get) | **GET** /storages/{storage_id} | Pobiera informacje o magazynie
[**storages_storage_id_put**](StoragesStorageIdApi.md#storages_storage_id_put) | **PUT** /storages/{storage_id} | Aktualizuje magazyn


# **storages_storage_id_delete**
> object storages_storage_id_delete(storage_id, accept=accept)

Usuwa magazyn

Usuwa magazyn

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
    api_instance = sellasist_api.StoragesStorageIdApi(api_client)
    storage_id = 'storage_id_example' # str | Identyfikator magazynu
accept = 'application/json' # str |  (optional)

    try:
        # Usuwa magazyn
        api_response = api_instance.storages_storage_id_delete(storage_id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling StoragesStorageIdApi->storages_storage_id_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **storage_id** | **str**| Identyfikator magazynu | 
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
**406** | Not Acceptable |  * Content-Type -  <br>  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **storages_storage_id_get**
> object storages_storage_id_get(storage_id, accept=accept)

Pobiera informacje o magazynie

Pobiera informacje o magazynie

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
    api_instance = sellasist_api.StoragesStorageIdApi(api_client)
    storage_id = 'storage_id_example' # str | Identyfikator magazynu
accept = 'application/json' # str |  (optional)

    try:
        # Pobiera informacje o magazynie
        api_response = api_instance.storages_storage_id_get(storage_id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling StoragesStorageIdApi->storages_storage_id_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **storage_id** | **str**| Identyfikator magazynu | 
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
**406** | Not Acceptable |  * Content-Type -  <br>  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **storages_storage_id_put**
> object storages_storage_id_put(storage_id, content_type=content_type, accept=accept, body=body)

Aktualizuje magazyn

Aktualizuje magazyn

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
    api_instance = sellasist_api.StoragesStorageIdApi(api_client)
    storage_id = 'storage_id_example' # str | Identyfikator magazynu
content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Aktualizuje magazyn
        api_response = api_instance.storages_storage_id_put(storage_id, content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling StoragesStorageIdApi->storages_storage_id_put: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **storage_id** | **str**| Identyfikator magazynu | 
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
**406** | Not Acceptable |  * Content-Type -  <br>  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

