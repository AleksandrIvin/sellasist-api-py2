# sellasist_api.OrdersWithCartsApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**orders_with_carts_get**](OrdersWithCartsApi.md#orders_with_carts_get) | **GET** /orders_with_carts | Zwraca listę zamówień


# **orders_with_carts_get**
> object orders_with_carts_get(accept=accept, offset=offset, limit=limit, status_id=status_id, email=email, payment_status=payment_status, payment_id=payment_id, shipment_id=shipment_id, currency=currency, sale_document=sale_document, date_from=date_from, date_to=date_to, sort=sort, source=source)

Zwraca listę zamówień

Zwraca listę zamówień

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
    api_instance = sellasist_api.OrdersWithCartsApi(api_client)
    accept = 'application/json' # str |  (optional)
offset = 4072 # int | Offset (optional)
limit = 4072 # int | Limit (optional)
status_id = 4072 # int | Identyfikator statusu (optional)
email = 'string' # str | Adres email (optional)
payment_status = 'excess' # str | status płatności (optional)
payment_id = 4072 # int | Identyfikator metody płatności (optional)
shipment_id = 4072 # int | Identyfikator metody dostawy (optional)
currency = 'string' # str | symbol waluty (optional)
sale_document = 'invoice' # str | dokument sprzedaży (optional)
date_from = '2020-11-20 09:08:13' # str | Data zamówienia od (optional)
date_to = '2020-11-20 09:08:13' # str | Data zamówienia do (optional)
sort = 'string' # str | Sortowanie (asc/desc), domyślnie desc (optional)
source = 'arena' # str | źródło zamówienia (optional)

    try:
        # Zwraca listę zamówień
        api_response = api_instance.orders_with_carts_get(accept=accept, offset=offset, limit=limit, status_id=status_id, email=email, payment_status=payment_status, payment_id=payment_id, shipment_id=shipment_id, currency=currency, sale_document=sale_document, date_from=date_from, date_to=date_to, sort=sort, source=source)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling OrdersWithCartsApi->orders_with_carts_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accept** | **str**|  | [optional] 
 **offset** | **int**| Offset | [optional] 
 **limit** | **int**| Limit | [optional] 
 **status_id** | **int**| Identyfikator statusu | [optional] 
 **email** | **str**| Adres email | [optional] 
 **payment_status** | **str**| status płatności | [optional] 
 **payment_id** | **int**| Identyfikator metody płatności | [optional] 
 **shipment_id** | **int**| Identyfikator metody dostawy | [optional] 
 **currency** | **str**| symbol waluty | [optional] 
 **sale_document** | **str**| dokument sprzedaży | [optional] 
 **date_from** | **str**| Data zamówienia od | [optional] 
 **date_to** | **str**| Data zamówienia do | [optional] 
 **sort** | **str**| Sortowanie (asc/desc), domyślnie desc | [optional] 
 **source** | **str**| źródło zamówienia | [optional] 

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
**401** | Unauthorized |  * Content-Type -  <br>  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

