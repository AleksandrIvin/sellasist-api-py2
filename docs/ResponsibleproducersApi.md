# sellasist_api.ResponsibleproducersApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**responsibleproducers_get**](ResponsibleproducersApi.md#responsibleproducers_get) | **GET** /responsibleproducers | Pobierz listę odpowiedzialnych producentów
[**responsibleproducers_post**](ResponsibleproducersApi.md#responsibleproducers_post) | **POST** /responsibleproducers | Dodaj nowego odpowiedzialnego producenta


# **responsibleproducers_get**
> object responsibleproducers_get(accept=accept, manufacturer_id=manufacturer_id, limit=limit, offset=offset, sort=sort)

Pobierz listę odpowiedzialnych producentów

Zwraca listę odpowiedzialnych producentów z opcjonalnymi parametrami filtrowania.

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
    api_instance = sellasist_api.ResponsibleproducersApi(api_client)
    accept = 'application/json' # str |  (optional)
manufacturer_id = 456 # int | Filtruje wyniki według ID producenta. (optional)
limit = 50 # int | Liczba wyników do zwrócenia (maksymalnie 100). (optional)
offset = 10 # int | Przesunięcie (offset) dla paginacji wyników. (optional)
sort = 'desc' # str | Kolejność sortowania wyników. Wartości: `asc` (rosnąco) lub `desc` (malejąco). (optional)

    try:
        # Pobierz listę odpowiedzialnych producentów
        api_response = api_instance.responsibleproducers_get(accept=accept, manufacturer_id=manufacturer_id, limit=limit, offset=offset, sort=sort)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ResponsibleproducersApi->responsibleproducers_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accept** | **str**|  | [optional] 
 **manufacturer_id** | **int**| Filtruje wyniki według ID producenta. | [optional] 
 **limit** | **int**| Liczba wyników do zwrócenia (maksymalnie 100). | [optional] 
 **offset** | **int**| Przesunięcie (offset) dla paginacji wyników. | [optional] 
 **sort** | **str**| Kolejność sortowania wyników. Wartości: &#x60;asc&#x60; (rosnąco) lub &#x60;desc&#x60; (malejąco). | [optional] 

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
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **responsibleproducers_post**
> object responsibleproducers_post(content_type=content_type, accept=accept, body=body)

Dodaj nowego odpowiedzialnego producenta

Tworzy nowego odpowiedzialnego producenta na podstawie przekazanych danych.

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
    api_instance = sellasist_api.ResponsibleproducersApi(api_client)
    content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Dodaj nowego odpowiedzialnego producenta
        api_response = api_instance.responsibleproducers_post(content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ResponsibleproducersApi->responsibleproducers_post: %s\n" % e)
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
**400** | Bad Request |  * Content-Type -  <br>  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

