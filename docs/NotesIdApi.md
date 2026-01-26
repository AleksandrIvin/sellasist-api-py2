# sellasist_api.NotesIdApi

All URIs are relative to *http://}*

Method | HTTP request | Description
------------- | ------------- | -------------
[**notes_id_delete**](NotesIdApi.md#notes_id_delete) | **DELETE** /notes/{id} | Usuwa notatkę


# **notes_id_delete**
> object notes_id_delete(id, accept=accept)

Usuwa notatkę

Usuwa notatkę

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
    api_instance = sellasist_api.NotesIdApi(api_client)
    id = 4072 # int | ID notatki do usunięcia
accept = 'application/json' # str |  (optional)

    try:
        # Usuwa notatkę
        api_response = api_instance.notes_id_delete(id, accept=accept)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling NotesIdApi->notes_id_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ID notatki do usunięcia | 
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
**404** | Not Found |  * Content-Type -  <br>  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

