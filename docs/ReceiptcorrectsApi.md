# sellasist_api.ReceiptcorrectsApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**receiptcorrects_get**](ReceiptcorrectsApi.md#receiptcorrects_get) | **GET** /receiptcorrects | Zwraca listę korekt paragonów
[**receiptcorrects_post**](ReceiptcorrectsApi.md#receiptcorrects_post) | **POST** /receiptcorrects | Tworzenie nowej korekty paragonu


# **receiptcorrects_get**
> object receiptcorrects_get(accept=accept, offset=offset, limit=limit, sort=sort)

Zwraca listę korekt paragonów

Zwraca listę korekt paragonów

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
    api_instance = sellasist_api.ReceiptcorrectsApi(api_client)
    accept = 'application/json' # str |  (optional)
offset = 4072 # int | Offset (optional)
limit = 4072 # int | Limit (optional)
sort = 'string' # str | Sortowanie (asc/desc), domyślnie desc (optional)

    try:
        # Zwraca listę korekt paragonów
        api_response = api_instance.receiptcorrects_get(accept=accept, offset=offset, limit=limit, sort=sort)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ReceiptcorrectsApi->receiptcorrects_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accept** | **str**|  | [optional] 
 **offset** | **int**| Offset | [optional] 
 **limit** | **int**| Limit | [optional] 
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

# **receiptcorrects_post**
> object receiptcorrects_post(content_type=content_type, accept=accept, body=body)

Tworzenie nowej korekty paragonu

Tworzenie nowej korekty paragonu

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
    api_instance = sellasist_api.ReceiptcorrectsApi(api_client)
    content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Tworzenie nowej korekty paragonu
        api_response = api_instance.receiptcorrects_post(content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ReceiptcorrectsApi->receiptcorrects_post: %s\n" % e)
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

