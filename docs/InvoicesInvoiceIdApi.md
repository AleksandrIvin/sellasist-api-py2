# sellasist_api.InvoicesInvoiceIdApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**invoices_invoice_id_delete**](InvoicesInvoiceIdApi.md#invoices_invoice_id_delete) | **DELETE** /invoices/{invoice_id} | Usunięcie faktury
[**invoices_invoice_id_get**](InvoicesInvoiceIdApi.md#invoices_invoice_id_get) | **GET** /invoices/{invoice_id} | Zwraca informacje o wybranej fakturze
[**invoices_invoice_id_put**](InvoicesInvoiceIdApi.md#invoices_invoice_id_put) | **PUT** /invoices/{invoice_id} | Aktualizacja faktury


# **invoices_invoice_id_delete**
> object invoices_invoice_id_delete(invoice_id, accept=accept)

Usunięcie faktury

Usunięcie faktury

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
    api_instance = sellasist_api.InvoicesInvoiceIdApi(api_client)
    invoice_id = 'invoice_id_example' # str | Identyfikator faktury
accept = 'application/json' # str |  (optional)

    try:
        # Usunięcie faktury
        api_response = api_instance.invoices_invoice_id_delete(invoice_id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling InvoicesInvoiceIdApi->invoices_invoice_id_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **str**| Identyfikator faktury | 
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

# **invoices_invoice_id_get**
> object invoices_invoice_id_get(invoice_id, accept=accept)

Zwraca informacje o wybranej fakturze

Zwraca informacje o wybranej fakturze

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
    api_instance = sellasist_api.InvoicesInvoiceIdApi(api_client)
    invoice_id = 'invoice_id_example' # str | Identyfikator faktury
accept = 'application/json' # str |  (optional)

    try:
        # Zwraca informacje o wybranej fakturze
        api_response = api_instance.invoices_invoice_id_get(invoice_id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling InvoicesInvoiceIdApi->invoices_invoice_id_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **str**| Identyfikator faktury | 
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

# **invoices_invoice_id_put**
> object invoices_invoice_id_put(invoice_id, content_type=content_type, accept=accept, body=body)

Aktualizacja faktury

Aktualizacja faktury

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
    api_instance = sellasist_api.InvoicesInvoiceIdApi(api_client)
    invoice_id = 'invoice_id_example' # str | Identyfikator faktury
content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Aktualizacja faktury
        api_response = api_instance.invoices_invoice_id_put(invoice_id, content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling InvoicesInvoiceIdApi->invoices_invoice_id_put: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **str**| Identyfikator faktury | 
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

