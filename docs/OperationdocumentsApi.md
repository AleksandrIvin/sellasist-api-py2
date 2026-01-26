# sellasist_api.OperationdocumentsApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**operationdocuments_get**](OperationdocumentsApi.md#operationdocuments_get) | **GET** /operationdocuments | Pobierz listę dokumentów operacyjnych
[**operationdocuments_post**](OperationdocumentsApi.md#operationdocuments_post) | **POST** /operationdocuments | Dodaj nowy dokument operacyjny


# **operationdocuments_get**
> object operationdocuments_get(accept=accept, limit=limit, offset=offset, series_id=series_id, type=type, subtype=subtype, date_from=date_from, date_to=date_to, order_id=order_id, is_printed=is_printed, print_suspended=print_suspended, sort=sort)

Pobierz listę dokumentów operacyjnych

Zwraca listę dokumentów operacyjnych z opcjonalnymi parametrami filtrowania.

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
    api_instance = sellasist_api.OperationdocumentsApi(api_client)
    accept = 'application/json' # str |  (optional)
limit = 50 # int | Liczba wyników do zwrócenia (maksymalnie 100). (optional)
offset = 10 # int | Przesunięcie (offset) dla paginacji wyników. (optional)
series_id = 3 # int | Filtruje według identyfikatora serii dokumentów. (optional)
type = 'sale' # str | Filtruje według typu dokumentu [`sale`, `stock`, `correct`]. (optional)
subtype = 'invoice' # str | Filtruje według podtypu dokumentu [`invoice`, `receipt`, `proforma`, `bill`, `correction`, `reservation`, `release`, `internal_release`, `internal_admission`, `admission`, `mov`]. (optional)
date_from = '2023-01-01' # str | Data początkowa (od) dla filtrowania dokumentów (po polu `issue_date`). (optional)
date_to = '2023-12-31' # str | Data końcowa (do) dla filtrowania dokumentów (po polu `issue_date`). (optional)
order_id = 202 # int | Filtruje dokumenty według ID zamówienia. (optional)
is_printed = true # bool | Filtruje według statusu wydruku. Prawidłowe wartości: `true` lub `false`. (optional)
print_suspended = true # bool | Filtruje według statusu wstrzymania wydruku. Prawidłowe wartości: `true` lub `false`. (optional)
sort = 'desc' # str | Kolejność sortowania wyników. Wartości: `asc` (rosnąco) lub `desc` (malejąco). (optional)

    try:
        # Pobierz listę dokumentów operacyjnych
        api_response = api_instance.operationdocuments_get(accept=accept, limit=limit, offset=offset, series_id=series_id, type=type, subtype=subtype, date_from=date_from, date_to=date_to, order_id=order_id, is_printed=is_printed, print_suspended=print_suspended, sort=sort)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling OperationdocumentsApi->operationdocuments_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accept** | **str**|  | [optional] 
 **limit** | **int**| Liczba wyników do zwrócenia (maksymalnie 100). | [optional] 
 **offset** | **int**| Przesunięcie (offset) dla paginacji wyników. | [optional] 
 **series_id** | **int**| Filtruje według identyfikatora serii dokumentów. | [optional] 
 **type** | **str**| Filtruje według typu dokumentu [&#x60;sale&#x60;, &#x60;stock&#x60;, &#x60;correct&#x60;]. | [optional] 
 **subtype** | **str**| Filtruje według podtypu dokumentu [&#x60;invoice&#x60;, &#x60;receipt&#x60;, &#x60;proforma&#x60;, &#x60;bill&#x60;, &#x60;correction&#x60;, &#x60;reservation&#x60;, &#x60;release&#x60;, &#x60;internal_release&#x60;, &#x60;internal_admission&#x60;, &#x60;admission&#x60;, &#x60;mov&#x60;]. | [optional] 
 **date_from** | **str**| Data początkowa (od) dla filtrowania dokumentów (po polu &#x60;issue_date&#x60;). | [optional] 
 **date_to** | **str**| Data końcowa (do) dla filtrowania dokumentów (po polu &#x60;issue_date&#x60;). | [optional] 
 **order_id** | **int**| Filtruje dokumenty według ID zamówienia. | [optional] 
 **is_printed** | **bool**| Filtruje według statusu wydruku. Prawidłowe wartości: &#x60;true&#x60; lub &#x60;false&#x60;. | [optional] 
 **print_suspended** | **bool**| Filtruje według statusu wstrzymania wydruku. Prawidłowe wartości: &#x60;true&#x60; lub &#x60;false&#x60;. | [optional] 
 **sort** | **str**| Kolejność sortowania wyników. Wartości: &#x60;asc&#x60; (rosnąco) lub &#x60;desc&#x60; (malejąco). | [optional] 

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
**400** | Bad Request |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **operationdocuments_post**
> object operationdocuments_post(content_type=content_type, accept=accept, body=body)

Dodaj nowy dokument operacyjny

Tworzy nowy dokument operacyjny na podstawie przekazanych danych.

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
    api_instance = sellasist_api.OperationdocumentsApi(api_client)
    content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Dodaj nowy dokument operacyjny
        api_response = api_instance.operationdocuments_post(content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling OperationdocumentsApi->operationdocuments_post: %s\n" % e)
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
 - **Accept**: application/json, text/plain

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Created |  * Content-Type -  <br>  |
**400** | Bad Request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

