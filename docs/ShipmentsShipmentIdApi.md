# sellasist_api.ShipmentsShipmentIdApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**shipments_shipment_id_delete**](ShipmentsShipmentIdApi.md#shipments_shipment_id_delete) | **DELETE** /shipments/{shipment_id} | Usuwa daną metodę dostawy
[**shipments_shipment_id_get**](ShipmentsShipmentIdApi.md#shipments_shipment_id_get) | **GET** /shipments/{shipment_id} | Tworzy metodę dostawy
[**shipments_shipment_id_put**](ShipmentsShipmentIdApi.md#shipments_shipment_id_put) | **PUT** /shipments/{shipment_id} | Aktualizuje metodę dostawy


# **shipments_shipment_id_delete**
> object shipments_shipment_id_delete(shipment_id, accept=accept)

Usuwa daną metodę dostawy

Usuwa daną metodę dostawy

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
    api_instance = sellasist_api.ShipmentsShipmentIdApi(api_client)
    shipment_id = 'shipment_id_example' # str | Identyfikator metody dostawy
accept = 'application/json' # str |  (optional)

    try:
        # Usuwa daną metodę dostawy
        api_response = api_instance.shipments_shipment_id_delete(shipment_id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ShipmentsShipmentIdApi->shipments_shipment_id_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **shipment_id** | **str**| Identyfikator metody dostawy | 
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

# **shipments_shipment_id_get**
> object shipments_shipment_id_get(shipment_id, accept=accept)

Tworzy metodę dostawy

Tworzy metodę dostawy

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
    api_instance = sellasist_api.ShipmentsShipmentIdApi(api_client)
    shipment_id = 'shipment_id_example' # str | Identyfikator metody dostawy
accept = 'application/json' # str |  (optional)

    try:
        # Tworzy metodę dostawy
        api_response = api_instance.shipments_shipment_id_get(shipment_id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ShipmentsShipmentIdApi->shipments_shipment_id_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **shipment_id** | **str**| Identyfikator metody dostawy | 
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

# **shipments_shipment_id_put**
> object shipments_shipment_id_put(shipment_id, content_type=content_type, accept=accept, body=body)

Aktualizuje metodę dostawy

Aktualizuje metodę dostawy

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
    api_instance = sellasist_api.ShipmentsShipmentIdApi(api_client)
    shipment_id = 'shipment_id_example' # str | Identyfikator metody dostawy
content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Aktualizuje metodę dostawy
        api_response = api_instance.shipments_shipment_id_put(shipment_id, content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ShipmentsShipmentIdApi->shipments_shipment_id_put: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **shipment_id** | **str**| Identyfikator metody dostawy | 
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

