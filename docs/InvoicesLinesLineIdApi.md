# sellasist_api.InvoicesLinesLineIdApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**invoices_lines_line_id_delete**](InvoicesLinesLineIdApi.md#invoices_lines_line_id_delete) | **DELETE** /invoices_lines/{line_id} | Usunięcie pozycji na fakturze
[**invoices_lines_line_id_put**](InvoicesLinesLineIdApi.md#invoices_lines_line_id_put) | **PUT** /invoices_lines/{line_id} | Aktualizacja pozycji na fakturze


# **invoices_lines_line_id_delete**
> object invoices_lines_line_id_delete(line_id, accept=accept)

Usunięcie pozycji na fakturze

Usunięcie pozycji na fakturze

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
    api_instance = sellasist_api.InvoicesLinesLineIdApi(api_client)
    line_id = 'line_id_example' # str | Identyfikator linii
accept = 'application/json' # str |  (optional)

    try:
        # Usunięcie pozycji na fakturze
        api_response = api_instance.invoices_lines_line_id_delete(line_id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling InvoicesLinesLineIdApi->invoices_lines_line_id_delete: %s\n" % e)
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

# **invoices_lines_line_id_put**
> object invoices_lines_line_id_put(line_id, content_type=content_type, accept=accept, body=body)

Aktualizacja pozycji na fakturze

Aktualizacja pozycji na fakturze

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
    api_instance = sellasist_api.InvoicesLinesLineIdApi(api_client)
    line_id = 'line_id_example' # str | Identyfikator linii
content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Aktualizacja pozycji na fakturze
        api_response = api_instance.invoices_lines_line_id_put(line_id, content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling InvoicesLinesLineIdApi->invoices_lines_line_id_put: %s\n" % e)
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

