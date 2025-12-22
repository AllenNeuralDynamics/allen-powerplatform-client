# allen_powerplatform_client.DefaultApi

All URIs are relative to *https://8fd02505cbdee9558087f7d04a48a5.11.environment.api.powerplatform.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_table**](DefaultApi.md#get_table) | **GET** /powerautomate/automations/direct/workflows/0438716ee92b4378811dbc975401decd/triggers/manual/paths/invoke | Gets all data for a table by table name
[**post_water_record**](DefaultApi.md#post_water_record) | **POST** /powerautomate/automations/direct/workflows/6148df039f724a4da146cc793585b8d2/triggers/manual/paths/invoke | Posts a water record from WaterLog into the dataverse weights water table
[**post_weight_record**](DefaultApi.md#post_weight_record) | **POST** /powerautomate/automations/direct/workflows/4be33b76ba3843058033eeb4d82b5240/triggers/manual/paths/invoke | Posts a weight record from water log


# **get_table**
> object get_table(api_version=api_version, content_type=content_type)

Gets all data for a table by table name

gets all data for a table by table name

### Example

* OAuth Authentication (oauth2-auth):
* OAuth Authentication (oAuthClientCredentials):
* OAuth Authentication (certOauth):

```python
import allen_powerplatform_client
from allen_powerplatform_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://8fd02505cbdee9558087f7d04a48a5.11.environment.api.powerplatform.com
# See configuration.py for a list of all supported configuration parameters.
configuration = allen_powerplatform_client.Configuration(
    host = "https://8fd02505cbdee9558087f7d04a48a5.11.environment.api.powerplatform.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

configuration.access_token = os.environ["ACCESS_TOKEN"]

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with allen_powerplatform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = allen_powerplatform_client.DefaultApi(api_client)
    api_version = 56 # int |  (optional)
    content_type = 'content_type_example' # str |  (optional)

    try:
        # Gets all data for a table by table name
        api_response = api_instance.get_table(api_version=api_version, content_type=content_type)
        print("The response of DefaultApi->get_table:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->get_table: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_version** | **int**|  | [optional] 
 **content_type** | **str**|  | [optional] 

### Return type

**object**

### Authorization

[oauth2-auth](../README.md#oauth2-auth), [oAuthClientCredentials](../README.md#oAuthClientCredentials), [certOauth](../README.md#certOauth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | default |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **post_water_record**
> object post_water_record(api_version=api_version, content_type=content_type, body=body)

Posts a water record from WaterLog into the dataverse weights water table

Posts a water record from WaterLog into the dataverse weights water table

### Example

* OAuth Authentication (oauth2-auth):
* OAuth Authentication (oAuthClientCredentials):
* OAuth Authentication (certOauth):

```python
import allen_powerplatform_client
from allen_powerplatform_client.models.post_water_record_request import PostWaterRecordRequest
from allen_powerplatform_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://8fd02505cbdee9558087f7d04a48a5.11.environment.api.powerplatform.com
# See configuration.py for a list of all supported configuration parameters.
configuration = allen_powerplatform_client.Configuration(
    host = "https://8fd02505cbdee9558087f7d04a48a5.11.environment.api.powerplatform.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

configuration.access_token = os.environ["ACCESS_TOKEN"]

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with allen_powerplatform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = allen_powerplatform_client.DefaultApi(api_client)
    api_version = 56 # int |  (optional)
    content_type = 'content_type_example' # str |  (optional)
    body = allen_powerplatform_client.PostWaterRecordRequest() # PostWaterRecordRequest |  (optional)

    try:
        # Posts a water record from WaterLog into the dataverse weights water table
        api_response = api_instance.post_water_record(api_version=api_version, content_type=content_type, body=body)
        print("The response of DefaultApi->post_water_record:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->post_water_record: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_version** | **int**|  | [optional] 
 **content_type** | **str**|  | [optional] 
 **body** | [**PostWaterRecordRequest**](PostWaterRecordRequest.md)|  | [optional] 

### Return type

**object**

### Authorization

[oauth2-auth](../README.md#oauth2-auth), [oAuthClientCredentials](../README.md#oAuthClientCredentials), [certOauth](../README.md#certOauth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | default |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **post_weight_record**
> object post_weight_record(api_version=api_version, content_type=content_type, body=body)

Posts a weight record from water log

posts a weight record from waterlog

### Example

* OAuth Authentication (oauth2-auth):
* OAuth Authentication (oAuthClientCredentials):
* OAuth Authentication (certOauth):

```python
import allen_powerplatform_client
from allen_powerplatform_client.models.post_weight_record_request import PostWeightRecordRequest
from allen_powerplatform_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://8fd02505cbdee9558087f7d04a48a5.11.environment.api.powerplatform.com
# See configuration.py for a list of all supported configuration parameters.
configuration = allen_powerplatform_client.Configuration(
    host = "https://8fd02505cbdee9558087f7d04a48a5.11.environment.api.powerplatform.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

configuration.access_token = os.environ["ACCESS_TOKEN"]

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with allen_powerplatform_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = allen_powerplatform_client.DefaultApi(api_client)
    api_version = 56 # int |  (optional)
    content_type = 'content_type_example' # str |  (optional)
    body = allen_powerplatform_client.PostWeightRecordRequest() # PostWeightRecordRequest |  (optional)

    try:
        # Posts a weight record from water log
        api_response = api_instance.post_weight_record(api_version=api_version, content_type=content_type, body=body)
        print("The response of DefaultApi->post_weight_record:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->post_weight_record: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_version** | **int**|  | [optional] 
 **content_type** | **str**|  | [optional] 
 **body** | [**PostWeightRecordRequest**](PostWeightRecordRequest.md)|  | [optional] 

### Return type

**object**

### Authorization

[oauth2-auth](../README.md#oauth2-auth), [oAuthClientCredentials](../README.md#oAuthClientCredentials), [certOauth](../README.md#certOauth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | default |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

