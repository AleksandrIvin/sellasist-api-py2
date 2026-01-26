# sellasist_api.ReceiptsLinesLineIdApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**receipts_lines_line_id_delete**](ReceiptsLinesLineIdApi.md#receipts_lines_line_id_delete) | **DELETE** /receipts_lines/{line_id} | Usunięcie pozycji na paragonie
[**receipts_lines_line_id_put**](ReceiptsLinesLineIdApi.md#receipts_lines_line_id_put) | **PUT** /receipts_lines/{line_id} | Aktualizacja pozycji na paragonie


# **receipts_lines_line_id_delete**
> object receipts_lines_line_id_delete(line_id, accept=accept)

Usunięcie pozycji na paragonie

Usunięcie pozycji na paragonie

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
    api_instance = sellasist_api.ReceiptsLinesLineIdApi(api_client)
    line_id = 'line_id_example' # str | Identyfikator linii
accept = 'application/json' # str |  (optional)

    try:
        # Usunięcie pozycji na paragonie
        api_response = api_instance.receipts_lines_line_id_delete(line_id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ReceiptsLinesLineIdApi->receipts_lines_line_id_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **line_id** | **str**| Identyfikator linii | 
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

# **receipts_lines_line_id_put**
> object receipts_lines_line_id_put(line_id, content_type=content_type, accept=accept, body=body)

Aktualizacja pozycji na paragonie

Aktualizacja pozycji na paragonie

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
    api_instance = sellasist_api.ReceiptsLinesLineIdApi(api_client)
    line_id = 'line_id_example' # str | Identyfikator linii
content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Aktualizacja pozycji na paragonie
        api_response = api_instance.receipts_lines_line_id_put(line_id, content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ReceiptsLinesLineIdApi->receipts_lines_line_id_put: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **line_id** | **str**| Identyfikator linii | 
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

