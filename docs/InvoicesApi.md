# sellasist_api.InvoicesApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**invoices_get**](InvoicesApi.md#invoices_get) | **GET** /invoices | Zwraca listę faktur
[**invoices_post**](InvoicesApi.md#invoices_post) | **POST** /invoices | Tworzenie nowej faktury


# **invoices_get**
> object invoices_get(accept=accept, offset=offset, limit=limit, date_from=date_from, date_to=date_to, sort=sort, series_id=series_id)

Zwraca listę faktur

Zwraca listę faktur

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
    api_instance = sellasist_api.InvoicesApi(api_client)
    accept = 'application/json' # str |  (optional)
offset = 4072 # int | Offset (optional)
limit = 4072 # int | Limit (optional)
date_from = '2020-11-20' # str | Data wystawienia od (optional)
date_to = '2020-11-20' # str | Data wystawienia do (optional)
sort = 'string' # str | Sortowanie (asc/desc), domyślnie desc (optional)
series_id = 4072 # int | Identyfikator serii (optional)

    try:
        # Zwraca listę faktur
        api_response = api_instance.invoices_get(accept=accept, offset=offset, limit=limit, date_from=date_from, date_to=date_to, sort=sort, series_id=series_id)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling InvoicesApi->invoices_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accept** | **str**|  | [optional] 
 **offset** | **int**| Offset | [optional] 
 **limit** | **int**| Limit | [optional] 
 **date_from** | **str**| Data wystawienia od | [optional] 
 **date_to** | **str**| Data wystawienia do | [optional] 
 **sort** | **str**| Sortowanie (asc/desc), domyślnie desc | [optional] 
 **series_id** | **int**| Identyfikator serii | [optional] 

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

# **invoices_post**
> object invoices_post(content_type=content_type, accept=accept, body=body)

Tworzenie nowej faktury

Tworzenie nowej faktury

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
    api_instance = sellasist_api.InvoicesApi(api_client)
    content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Tworzenie nowej faktury
        api_response = api_instance.invoices_post(content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling InvoicesApi->invoices_post: %s\n" % e)
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

