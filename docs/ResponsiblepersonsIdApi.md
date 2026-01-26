# sellasist_api.ResponsiblepersonsIdApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**responsiblepersons_id_get**](ResponsiblepersonsIdApi.md#responsiblepersons_id_get) | **GET** /responsiblepersons/{id} | Pobierz osobę odpowiedzialną według ID
[**responsiblepersons_id_put**](ResponsiblepersonsIdApi.md#responsiblepersons_id_put) | **PUT** /responsiblepersons/{id} | Zaktualizuj osobę odpowiedzialną


# **responsiblepersons_id_get**
> object responsiblepersons_id_get(id, accept=accept)

Pobierz osobę odpowiedzialną według ID

Zwraca szczegółowe informacje o osobie odpowiedzialnej.

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
    api_instance = sellasist_api.ResponsiblepersonsIdApi(api_client)
    id = 123 # int | ID osoby odpowiedzialnej.
accept = 'application/json' # str |  (optional)

    try:
        # Pobierz osobę odpowiedzialną według ID
        api_response = api_instance.responsiblepersons_id_get(id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ResponsiblepersonsIdApi->responsiblepersons_id_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ID osoby odpowiedzialnej. | 
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

# **responsiblepersons_id_put**
> object responsiblepersons_id_put(id, content_type=content_type, accept=accept, body=body)

Zaktualizuj osobę odpowiedzialną

Aktualizuje istniejące dane osoby odpowiedzialnej.

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
    api_instance = sellasist_api.ResponsiblepersonsIdApi(api_client)
    id = 123 # int | ID osoby odpowiedzialnej do aktualizacji.
content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Zaktualizuj osobę odpowiedzialną
        api_response = api_instance.responsiblepersons_id_put(id, content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ResponsiblepersonsIdApi->responsiblepersons_id_put: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ID osoby odpowiedzialnej do aktualizacji. | 
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

