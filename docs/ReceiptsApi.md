# sellasist_api.ReceiptsApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**receipts_get**](ReceiptsApi.md#receipts_get) | **GET** /receipts | Zwraca listę paragonów
[**receipts_post**](ReceiptsApi.md#receipts_post) | **POST** /receipts | Tworzenie nowego paragonu


# **receipts_get**
> object receipts_get(accept=accept, date_from=date_from, date_to=date_to, printed=printed, print_suspended=print_suspended, offset=offset, limit=limit, sort=sort, series_id=series_id)

Zwraca listę paragonów

Zwraca listę paragonów

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
    api_instance = sellasist_api.ReceiptsApi(api_client)
    accept = 'application/json' # str |  (optional)
date_from = '2020-11-20 09:08:13' # str | Data utworzenia paragonu od (optional)
date_to = '2020-11-20 09:08:13' # str | Data utworzenia paragonu do (optional)
printed = 'printed_example' # str | Wydrukowane (true/false) (optional)
print_suspended = 'print_suspended_example' # str | Wydruk zawieszony (true/false) (optional)
offset = 4072 # int | Offset (optional)
limit = 4072 # int | Limit (optional)
sort = 'string' # str | Sortowanie (asc/desc), domyślnie desc (optional)
series_id = 4072 # int | Identyfikator serii (optional)

    try:
        # Zwraca listę paragonów
        api_response = api_instance.receipts_get(accept=accept, date_from=date_from, date_to=date_to, printed=printed, print_suspended=print_suspended, offset=offset, limit=limit, sort=sort, series_id=series_id)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ReceiptsApi->receipts_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accept** | **str**|  | [optional] 
 **date_from** | **str**| Data utworzenia paragonu od | [optional] 
 **date_to** | **str**| Data utworzenia paragonu do | [optional] 
 **printed** | **str**| Wydrukowane (true/false) | [optional] 
 **print_suspended** | **str**| Wydruk zawieszony (true/false) | [optional] 
 **offset** | **int**| Offset | [optional] 
 **limit** | **int**| Limit | [optional] 
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

# **receipts_post**
> object receipts_post(content_type=content_type, accept=accept, body=body)

Tworzenie nowego paragonu

Tworzenie nowego paragonu

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
    api_instance = sellasist_api.ReceiptsApi(api_client)
    content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Tworzenie nowego paragonu
        api_response = api_instance.receipts_post(content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ReceiptsApi->receipts_post: %s\n" % e)
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

