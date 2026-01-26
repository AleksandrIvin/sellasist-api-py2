# sellasist_api.OperationdocumentsIdApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**operationdocuments_id_delete**](OperationdocumentsIdApi.md#operationdocuments_id_delete) | **DELETE** /operationdocuments/{id} | Usuń dokument operacyjny
[**operationdocuments_id_get**](OperationdocumentsIdApi.md#operationdocuments_id_get) | **GET** /operationdocuments/{id} | Pobierz dokument operacyjny według ID
[**operationdocuments_id_put**](OperationdocumentsIdApi.md#operationdocuments_id_put) | **PUT** /operationdocuments/{id} | Zaktualizuj dokument operacyjny


# **operationdocuments_id_delete**
> str operationdocuments_id_delete(id)

Usuń dokument operacyjny

Trwale usuwa dokument operacyjny o podanym ID.

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
    api_instance = sellasist_api.OperationdocumentsIdApi(api_client)
    id = 123 # int | ID dokumentu operacyjnego do usunięcia.

    try:
        # Usuń dokument operacyjny
        api_response = api_instance.operationdocuments_id_delete(id)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling OperationdocumentsIdApi->operationdocuments_id_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ID dokumentu operacyjnego do usunięcia. | 

### Return type

**str**

### Authorization

[apikeyAuth](../README.md#apikeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**204** | No Content |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **operationdocuments_id_get**
> object operationdocuments_id_get(id, accept=accept)

Pobierz dokument operacyjny według ID

Zwraca szczegółowe informacje o dokumencie operacyjnym.

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
    api_instance = sellasist_api.OperationdocumentsIdApi(api_client)
    id = 123 # int | ID dokumentu operacyjnego.
accept = 'application/json' # str |  (optional)

    try:
        # Pobierz dokument operacyjny według ID
        api_response = api_instance.operationdocuments_id_get(id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling OperationdocumentsIdApi->operationdocuments_id_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ID dokumentu operacyjnego. | 
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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **operationdocuments_id_put**
> str operationdocuments_id_put(id, content_type=content_type, body=body)

Zaktualizuj dokument operacyjny

Zaktualizuj istniejące dane dokumentu operacyjnego.

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
    api_instance = sellasist_api.OperationdocumentsIdApi(api_client)
    id = 123 # int | ID dokumentu operacyjnego do aktualizacji.
content_type = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Zaktualizuj dokument operacyjny
        api_response = api_instance.operationdocuments_id_put(id, content_type=content_type, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling OperationdocumentsIdApi->operationdocuments_id_put: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ID dokumentu operacyjnego do aktualizacji. | 
 **content_type** | **str**|  | [optional] 
 **body** | **object**|  | [optional] 

### Return type

**str**

### Authorization

[apikeyAuth](../README.md#apikeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: text/plain

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |
**400** | Bad Request |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

