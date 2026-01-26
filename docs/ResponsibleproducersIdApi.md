# sellasist_api.ResponsibleproducersIdApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**responsibleproducers_id_get**](ResponsibleproducersIdApi.md#responsibleproducers_id_get) | **GET** /responsibleproducers/{id} | Pobierz odpowiedzialnego producenta według ID
[**responsibleproducers_id_put**](ResponsibleproducersIdApi.md#responsibleproducers_id_put) | **PUT** /responsibleproducers/{id} | Zaktualizuj odpowiedzialnego producenta


# **responsibleproducers_id_get**
> object responsibleproducers_id_get(id, accept=accept)

Pobierz odpowiedzialnego producenta według ID

Zwraca szczegółowe informacje o odpowiedzialnym producencie.

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
    api_instance = sellasist_api.ResponsibleproducersIdApi(api_client)
    id = 123 # int | ID odpowiedzialnego producenta.
accept = 'application/json' # str |  (optional)

    try:
        # Pobierz odpowiedzialnego producenta według ID
        api_response = api_instance.responsibleproducers_id_get(id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ResponsibleproducersIdApi->responsibleproducers_id_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ID odpowiedzialnego producenta. | 
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
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **responsibleproducers_id_put**
> object responsibleproducers_id_put(id, content_type=content_type, accept=accept, body=body)

Zaktualizuj odpowiedzialnego producenta

Aktualizuje istniejące dane odpowiedzialnego producenta.

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
    api_instance = sellasist_api.ResponsibleproducersIdApi(api_client)
    id = 123 # int | ID odpowiedzialnego producenta do aktualizacji.
content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Zaktualizuj odpowiedzialnego producenta
        api_response = api_instance.responsibleproducers_id_put(id, content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ResponsibleproducersIdApi->responsibleproducers_id_put: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ID odpowiedzialnego producenta do aktualizacji. | 
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
**400** | Bad Request |  * Content-Type -  <br>  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

