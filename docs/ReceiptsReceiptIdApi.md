# sellasist_api.ReceiptsReceiptIdApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**receipts_receipt_id_delete**](ReceiptsReceiptIdApi.md#receipts_receipt_id_delete) | **DELETE** /receipts/{receipt_id} | Usunięcie paragonu
[**receipts_receipt_id_get**](ReceiptsReceiptIdApi.md#receipts_receipt_id_get) | **GET** /receipts/{receipt_id} | Zwraca informacje o wybranym paragonie
[**receipts_receipt_id_put**](ReceiptsReceiptIdApi.md#receipts_receipt_id_put) | **PUT** /receipts/{receipt_id} | Aktualizacja paragonu


# **receipts_receipt_id_delete**
> object receipts_receipt_id_delete(receipt_id, accept=accept)

Usunięcie paragonu

Usunięcie paragonu

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
    api_instance = sellasist_api.ReceiptsReceiptIdApi(api_client)
    receipt_id = 'receipt_id_example' # str | Identyfikator paragonu
accept = 'application/json' # str |  (optional)

    try:
        # Usunięcie paragonu
        api_response = api_instance.receipts_receipt_id_delete(receipt_id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ReceiptsReceiptIdApi->receipts_receipt_id_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **receipt_id** | **str**| Identyfikator paragonu | 
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

# **receipts_receipt_id_get**
> object receipts_receipt_id_get(receipt_id, accept=accept)

Zwraca informacje o wybranym paragonie

Zwraca informacje o wybranym paragonie

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
    api_instance = sellasist_api.ReceiptsReceiptIdApi(api_client)
    receipt_id = 'receipt_id_example' # str | Identyfikator paragonu
accept = 'application/json' # str |  (optional)

    try:
        # Zwraca informacje o wybranym paragonie
        api_response = api_instance.receipts_receipt_id_get(receipt_id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ReceiptsReceiptIdApi->receipts_receipt_id_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **receipt_id** | **str**| Identyfikator paragonu | 
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

# **receipts_receipt_id_put**
> object receipts_receipt_id_put(receipt_id, content_type=content_type, accept=accept, body=body)

Aktualizacja paragonu

Aktualizacja paragonu

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
    api_instance = sellasist_api.ReceiptsReceiptIdApi(api_client)
    receipt_id = 'receipt_id_example' # str | Identyfikator paragonu
content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Aktualizacja paragonu
        api_response = api_instance.receipts_receipt_id_put(receipt_id, content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ReceiptsReceiptIdApi->receipts_receipt_id_put: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **receipt_id** | **str**| Identyfikator paragonu | 
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

