# sellasist_api.AttributesPropertiesAttributePropertyIdApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**attributes_properties_attribute_property_id_delete**](AttributesPropertiesAttributePropertyIdApi.md#attributes_properties_attribute_property_id_delete) | **DELETE** /attributes_properties/{attribute_property_id} | Usuwa dany atrybut
[**attributes_properties_attribute_property_id_get**](AttributesPropertiesAttributePropertyIdApi.md#attributes_properties_attribute_property_id_get) | **GET** /attributes_properties/{attribute_property_id} | Zwraca szczegóły właściwości
[**attributes_properties_attribute_property_id_put**](AttributesPropertiesAttributePropertyIdApi.md#attributes_properties_attribute_property_id_put) | **PUT** /attributes_properties/{attribute_property_id} | Aktualizuje właściwość atrybutu


# **attributes_properties_attribute_property_id_delete**
> object attributes_properties_attribute_property_id_delete(attribute_property_id, accept=accept)

Usuwa dany atrybut

Usuwa dany atrybut

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
    api_instance = sellasist_api.AttributesPropertiesAttributePropertyIdApi(api_client)
    attribute_property_id = 'attribute_property_id_example' # str | Identyfikator atrybutu
accept = 'application/json' # str |  (optional)

    try:
        # Usuwa dany atrybut
        api_response = api_instance.attributes_properties_attribute_property_id_delete(attribute_property_id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling AttributesPropertiesAttributePropertyIdApi->attributes_properties_attribute_property_id_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **attribute_property_id** | **str**| Identyfikator atrybutu | 
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

# **attributes_properties_attribute_property_id_get**
> object attributes_properties_attribute_property_id_get(attribute_property_id, accept=accept)

Zwraca szczegóły właściwości

Zwraca szczegóły właściwości

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
    api_instance = sellasist_api.AttributesPropertiesAttributePropertyIdApi(api_client)
    attribute_property_id = 'attribute_property_id_example' # str | Identyfikator atrybutu
accept = 'application/json' # str |  (optional)

    try:
        # Zwraca szczegóły właściwości
        api_response = api_instance.attributes_properties_attribute_property_id_get(attribute_property_id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling AttributesPropertiesAttributePropertyIdApi->attributes_properties_attribute_property_id_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **attribute_property_id** | **str**| Identyfikator atrybutu | 
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

# **attributes_properties_attribute_property_id_put**
> object attributes_properties_attribute_property_id_put(attribute_property_id, content_type=content_type, accept=accept, body=body)

Aktualizuje właściwość atrybutu

Aktualizuje właściwość atrybutu

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
    api_instance = sellasist_api.AttributesPropertiesAttributePropertyIdApi(api_client)
    attribute_property_id = 'attribute_property_id_example' # str | Identyfikator właściwości atrybutu
content_type = 'application/json' # str |  (optional)
accept = 'application/json' # str |  (optional)
body = None # object |  (optional)

    try:
        # Aktualizuje właściwość atrybutu
        api_response = api_instance.attributes_properties_attribute_property_id_put(attribute_property_id, content_type=content_type, accept=accept, body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling AttributesPropertiesAttributePropertyIdApi->attributes_properties_attribute_property_id_put: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **attribute_property_id** | **str**| Identyfikator właściwości atrybutu | 
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

