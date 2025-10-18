# allen_dataverse_client.DefaultApi

All URIs are relative to *https://8fd02505cbdee9558087f7d04a48a5.11.environment.api.powerplatform.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**fetch_project_by_name**](DefaultApi.md#fetch_project_by_name) | **POST** /powerautomate/automations/direct/workflows/3bd68c3caf34448db7d6e2cd53602f88/triggers/manual/paths/invoke | Get Project PowerAutomate Flow
[**fetch_table_by_name**](DefaultApi.md#fetch_table_by_name) | **POST** /powerautomate/automations/direct/workflows/0438716ee92b4378811dbc975401decd/triggers/manual/paths/invoke | Get Table Power Automate Flow
[**fetch_table_names**](DefaultApi.md#fetch_table_names) | **POST** /powerautomate/automations/direct/workflows/70452d9b21584637a8023e3d66fc37ea/triggers/manual/paths/invoke | Get Table Names Power Automate Flow


# **fetch_project_by_name**
> object fetch_project_by_name(api_version, body)

Get Project PowerAutomate Flow

Triggers a PowerAutomate flow to get project data from Projects table in Dataverse

### Example

* OAuth Authentication (oauth2-auth):
* OAuth Authentication (oAuthClientCredentials):
* OAuth Authentication (certOauth):

```python
import allen_dataverse_client
from allen_dataverse_client.models.fetch_project_by_name_request import FetchProjectByNameRequest
from allen_dataverse_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://8fd02505cbdee9558087f7d04a48a5.11.environment.api.powerplatform.com
# See configuration.py for a list of all supported configuration parameters.
configuration = allen_dataverse_client.Configuration(
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
with allen_dataverse_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = allen_dataverse_client.DefaultApi(api_client)
    api_version = 1 # int |  (default to 1)
    body = allen_dataverse_client.FetchProjectByNameRequest() # FetchProjectByNameRequest | 

    try:
        # Get Project PowerAutomate Flow
        api_response = api_instance.fetch_project_by_name(api_version, body)
        print("The response of DefaultApi->fetch_project_by_name:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->fetch_project_by_name: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_version** | **int**|  | [default to 1]
 **body** | [**FetchProjectByNameRequest**](FetchProjectByNameRequest.md)|  | 

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

# **fetch_table_by_name**
> object fetch_table_by_name(api_version, body)

Get Table Power Automate Flow

Triggers a PowerAutomate flow to get a full table in Dataverse by the logical table name

### Example

* OAuth Authentication (oauth2-auth):
* OAuth Authentication (oAuthClientCredentials):
* OAuth Authentication (certOauth):

```python
import allen_dataverse_client
from allen_dataverse_client.models.fetch_table_by_name_request import FetchTableByNameRequest
from allen_dataverse_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://8fd02505cbdee9558087f7d04a48a5.11.environment.api.powerplatform.com
# See configuration.py for a list of all supported configuration parameters.
configuration = allen_dataverse_client.Configuration(
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
with allen_dataverse_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = allen_dataverse_client.DefaultApi(api_client)
    api_version = 1 # int |  (default to 1)
    body = allen_dataverse_client.FetchTableByNameRequest() # FetchTableByNameRequest | 

    try:
        # Get Table Power Automate Flow
        api_response = api_instance.fetch_table_by_name(api_version, body)
        print("The response of DefaultApi->fetch_table_by_name:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->fetch_table_by_name: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_version** | **int**|  | [default to 1]
 **body** | [**FetchTableByNameRequest**](FetchTableByNameRequest.md)|  | 

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

# **fetch_table_names**
> object fetch_table_names(api_version)

Get Table Names Power Automate Flow

Triggers a Power Automate flow that fetches custom table names in Dataverse

### Example

* OAuth Authentication (oauth2-auth):
* OAuth Authentication (oAuthClientCredentials):
* OAuth Authentication (certOauth):

```python
import allen_dataverse_client
from allen_dataverse_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://8fd02505cbdee9558087f7d04a48a5.11.environment.api.powerplatform.com
# See configuration.py for a list of all supported configuration parameters.
configuration = allen_dataverse_client.Configuration(
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
with allen_dataverse_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = allen_dataverse_client.DefaultApi(api_client)
    api_version = 1 # int |  (default to 1)

    try:
        # Get Table Names Power Automate Flow
        api_response = api_instance.fetch_table_names(api_version)
        print("The response of DefaultApi->fetch_table_names:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->fetch_table_names: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_version** | **int**|  | [default to 1]

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

