# allen_powerplatform_client.DefaultApi

All URIs are relative to *https://8fd02505cbdee9558087f7d04a48a5.11.environment.api.powerplatform.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_table_data**](DefaultApi.md#get_table_data) | **POST** /powerautomate/automations/direct/workflows/0438716ee92b4378811dbc975401decd/triggers/manual/paths/invoke | Get Table Data
[**get_table_names**](DefaultApi.md#get_table_names) | **POST** /powerautomate/automations/direct/workflows/70452d9b21584637a8023e3d66fc37ea/triggers/manual/paths/invoke | Get Table Name
[**post_mouse_weight_record**](DefaultApi.md#post_mouse_weight_record) | **POST** /powerautomate/automations/direct/workflows/7d8cc42d4198490f82d60659142cb848/triggers/manual/paths/invoke | Post Weight Record
[**validate_email_in_system_users**](DefaultApi.md#validate_email_in_system_users) | **POST** /powerautomate/automations/direct/workflows/fd45230267514933bd9e79a37e207e58/triggers/manual/paths/invoke | Validate Email in Users Table, Return Data
[**validate_mouse_guidin_mouse_registry**](DefaultApi.md#validate_mouse_guidin_mouse_registry) | **POST** /powerautomate/automations/direct/workflows/33e400168f5142fc84e2edcf85739dc4/triggers/manual/paths/invoke | validate mouseGUID in Mouse Registry, return data
[**validate_mouse_idin_mouse_registry**](DefaultApi.md#validate_mouse_idin_mouse_registry) | **POST** /powerautomate/automations/direct/workflows/2aca0c8f806f4403a57c9ebdb44ecc2f/triggers/manual/paths/invoke | Validate Mouse ID in Mouse Registry
[**validate_mouse_in_behavior_training**](DefaultApi.md#validate_mouse_in_behavior_training) | **POST** /powerautomate/automations/direct/workflows/51d8892464a94b0690310a88d2c6ebd8/triggers/manual/paths/invoke | validate mouse in Behavior Training, return data
[**validate_mouse_in_water_restricted_mice_table**](DefaultApi.md#validate_mouse_in_water_restricted_mice_table) | **POST** /powerautomate/automations/direct/workflows/d29134243d37405989d740693cf74eab/triggers/manual/paths/invoke | Validate Mouse Active in Water Restriction, Return Data
[**water_restriction_post_baseline_weight**](DefaultApi.md#water_restriction_post_baseline_weight) | **POST** /powerautomate/automations/direct/workflows/162463486d584978bfd17a5dbd2ed223/triggers/manual/paths/invoke | Post Baseline Weight
[**water_restriction_post_weight_and_water_records**](DefaultApi.md#water_restriction_post_weight_and_water_records) | **DELETE** /powerautomate/automations/direct/workflows/00ebb4b476e84e999d10d1034cf13492/triggers/manual/paths/invoke | Post Weight and Water Record
[**water_restriction_update_restriction_status**](DefaultApi.md#water_restriction_update_restriction_status) | **POST** /powerautomate/automations/direct/workflows/1c3c611c372246cd86d8597774beeafe/triggers/manual/paths/invoke | Update Water Restriction Status
[**water_restriction_update_target_weight_percent**](DefaultApi.md#water_restriction_update_target_weight_percent) | **POST** /powerautomate/automations/direct/workflows/f970e9425e6148aabdbb6a316802e92e/triggers/manual/paths/invoke | Update Target Weight Percent


# **get_table_data**
> object get_table_data(api_version=api_version, body=body)

Get Table Data

Gets all data for a table

### Example

* OAuth Authentication (oauth2-auth):
* OAuth Authentication (oAuthClientCredentials):
* OAuth Authentication (certOauth):

```python
import allen_powerplatform_client
from allen_powerplatform_client.models.get_table_data_request import GetTableDataRequest
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
    body = allen_powerplatform_client.GetTableDataRequest() # GetTableDataRequest |  (optional)

    try:
        # Get Table Data
        api_response = api_instance.get_table_data(api_version=api_version, body=body)
        print("The response of DefaultApi->get_table_data:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->get_table_data: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_version** | **int**|  | [optional] 
 **body** | [**GetTableDataRequest**](GetTableDataRequest.md)|  | [optional] 

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
**0** | default |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_table_names**
> object get_table_names(api_version=api_version, body=body)

Get Table Name

Gets all dataverse table names

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
    body = None # object |  (optional)

    try:
        # Get Table Name
        api_response = api_instance.get_table_names(api_version=api_version, body=body)
        print("The response of DefaultApi->get_table_names:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->get_table_names: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_version** | **int**|  | [optional] 
 **body** | **object**|  | [optional] 

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
**0** | default |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **post_mouse_weight_record**
> object post_mouse_weight_record(api_version=api_version, body=body)

Post Weight Record

post a weight record for a mouse

### Example

* OAuth Authentication (oauth2-auth):
* OAuth Authentication (oAuthClientCredentials):
* OAuth Authentication (certOauth):

```python
import allen_powerplatform_client
from allen_powerplatform_client.models.post_mouse_weight_record_request import PostMouseWeightRecordRequest
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
    body = allen_powerplatform_client.PostMouseWeightRecordRequest() # PostMouseWeightRecordRequest |  (optional)

    try:
        # Post Weight Record
        api_response = api_instance.post_mouse_weight_record(api_version=api_version, body=body)
        print("The response of DefaultApi->post_mouse_weight_record:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->post_mouse_weight_record: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_version** | **int**|  | [optional] 
 **body** | [**PostMouseWeightRecordRequest**](PostMouseWeightRecordRequest.md)|  | [optional] 

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
**0** | default |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validate_email_in_system_users**
> object validate_email_in_system_users(api_version=api_version, body=body)

Validate Email in Users Table, Return Data

validate email in system users table, return data

### Example

* OAuth Authentication (oauth2-auth):
* OAuth Authentication (oAuthClientCredentials):
* OAuth Authentication (certOauth):

```python
import allen_powerplatform_client
from allen_powerplatform_client.models.validate_email_in_system_users_request import ValidateEmailInSystemUsersRequest
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
    body = allen_powerplatform_client.ValidateEmailInSystemUsersRequest() # ValidateEmailInSystemUsersRequest |  (optional)

    try:
        # Validate Email in Users Table, Return Data
        api_response = api_instance.validate_email_in_system_users(api_version=api_version, body=body)
        print("The response of DefaultApi->validate_email_in_system_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->validate_email_in_system_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_version** | **int**|  | [optional] 
 **body** | [**ValidateEmailInSystemUsersRequest**](ValidateEmailInSystemUsersRequest.md)|  | [optional] 

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
**0** | default |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validate_mouse_guidin_mouse_registry**
> object validate_mouse_guidin_mouse_registry(api_version=api_version, body=body)

validate mouseGUID in Mouse Registry, return data

validate mouseGUID in Mouse Registry, return data

### Example

* OAuth Authentication (oauth2-auth):
* OAuth Authentication (oAuthClientCredentials):
* OAuth Authentication (certOauth):

```python
import allen_powerplatform_client
from allen_powerplatform_client.models.validate_mouse_guidin_mouse_registry_request import ValidateMouseGUIDInMouseRegistryRequest
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
    body = allen_powerplatform_client.ValidateMouseGUIDInMouseRegistryRequest() # ValidateMouseGUIDInMouseRegistryRequest |  (optional)

    try:
        # validate mouseGUID in Mouse Registry, return data
        api_response = api_instance.validate_mouse_guidin_mouse_registry(api_version=api_version, body=body)
        print("The response of DefaultApi->validate_mouse_guidin_mouse_registry:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->validate_mouse_guidin_mouse_registry: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_version** | **int**|  | [optional] 
 **body** | [**ValidateMouseGUIDInMouseRegistryRequest**](ValidateMouseGUIDInMouseRegistryRequest.md)|  | [optional] 

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
**0** | default |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validate_mouse_idin_mouse_registry**
> object validate_mouse_idin_mouse_registry(api_version=api_version, body=body)

Validate Mouse ID in Mouse Registry

validate a mouse id (6 digit labtracks ID) is in the mouse registry, return data

### Example

* OAuth Authentication (oauth2-auth):
* OAuth Authentication (oAuthClientCredentials):
* OAuth Authentication (certOauth):

```python
import allen_powerplatform_client
from allen_powerplatform_client.models.validate_mouse_idin_mouse_registry_request import ValidateMouseIDInMouseRegistryRequest
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
    body = allen_powerplatform_client.ValidateMouseIDInMouseRegistryRequest() # ValidateMouseIDInMouseRegistryRequest |  (optional)

    try:
        # Validate Mouse ID in Mouse Registry
        api_response = api_instance.validate_mouse_idin_mouse_registry(api_version=api_version, body=body)
        print("The response of DefaultApi->validate_mouse_idin_mouse_registry:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->validate_mouse_idin_mouse_registry: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_version** | **int**|  | [optional] 
 **body** | [**ValidateMouseIDInMouseRegistryRequest**](ValidateMouseIDInMouseRegistryRequest.md)|  | [optional] 

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
**0** | default |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validate_mouse_in_behavior_training**
> object validate_mouse_in_behavior_training(api_version=api_version, body=body)

validate mouse in Behavior Training, return data

validate mouse in Behavior Training, return data

### Example

* OAuth Authentication (oauth2-auth):
* OAuth Authentication (oAuthClientCredentials):
* OAuth Authentication (certOauth):

```python
import allen_powerplatform_client
from allen_powerplatform_client.models.validate_mouse_in_water_restricted_mice_table_request import ValidateMouseInWaterRestrictedMiceTableRequest
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
    body = allen_powerplatform_client.ValidateMouseInWaterRestrictedMiceTableRequest() # ValidateMouseInWaterRestrictedMiceTableRequest |  (optional)

    try:
        # validate mouse in Behavior Training, return data
        api_response = api_instance.validate_mouse_in_behavior_training(api_version=api_version, body=body)
        print("The response of DefaultApi->validate_mouse_in_behavior_training:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->validate_mouse_in_behavior_training: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_version** | **int**|  | [optional] 
 **body** | [**ValidateMouseInWaterRestrictedMiceTableRequest**](ValidateMouseInWaterRestrictedMiceTableRequest.md)|  | [optional] 

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
**0** | default |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validate_mouse_in_water_restricted_mice_table**
> object validate_mouse_in_water_restricted_mice_table(api_version=api_version, body=body)

Validate Mouse Active in Water Restriction, Return Data

Validate mouse in water restriction, return data

### Example

* OAuth Authentication (oauth2-auth):
* OAuth Authentication (oAuthClientCredentials):
* OAuth Authentication (certOauth):

```python
import allen_powerplatform_client
from allen_powerplatform_client.models.validate_mouse_in_water_restricted_mice_table_request import ValidateMouseInWaterRestrictedMiceTableRequest
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
    body = allen_powerplatform_client.ValidateMouseInWaterRestrictedMiceTableRequest() # ValidateMouseInWaterRestrictedMiceTableRequest |  (optional)

    try:
        # Validate Mouse Active in Water Restriction, Return Data
        api_response = api_instance.validate_mouse_in_water_restricted_mice_table(api_version=api_version, body=body)
        print("The response of DefaultApi->validate_mouse_in_water_restricted_mice_table:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->validate_mouse_in_water_restricted_mice_table: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_version** | **int**|  | [optional] 
 **body** | [**ValidateMouseInWaterRestrictedMiceTableRequest**](ValidateMouseInWaterRestrictedMiceTableRequest.md)|  | [optional] 

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
**0** | default |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **water_restriction_post_baseline_weight**
> object water_restriction_post_baseline_weight(api_version=api_version, body=body)

Post Baseline Weight

Post the baseline weight for a mouse on water restriction

### Example

* OAuth Authentication (oauth2-auth):
* OAuth Authentication (oAuthClientCredentials):
* OAuth Authentication (certOauth):

```python
import allen_powerplatform_client
from allen_powerplatform_client.models.water_restriction_post_baseline_weight_request import WaterRestrictionPostBaselineWeightRequest
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
    body = allen_powerplatform_client.WaterRestrictionPostBaselineWeightRequest() # WaterRestrictionPostBaselineWeightRequest |  (optional)

    try:
        # Post Baseline Weight
        api_response = api_instance.water_restriction_post_baseline_weight(api_version=api_version, body=body)
        print("The response of DefaultApi->water_restriction_post_baseline_weight:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->water_restriction_post_baseline_weight: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_version** | **int**|  | [optional] 
 **body** | [**WaterRestrictionPostBaselineWeightRequest**](WaterRestrictionPostBaselineWeightRequest.md)|  | [optional] 

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
**0** | default |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **water_restriction_post_weight_and_water_records**
> object water_restriction_post_weight_and_water_records(api_version=api_version, body=body)

Post Weight and Water Record

Post paired weight and water records for a water restricted mouse

### Example

* OAuth Authentication (oauth2-auth):
* OAuth Authentication (oAuthClientCredentials):
* OAuth Authentication (certOauth):

```python
import allen_powerplatform_client
from allen_powerplatform_client.models.water_restriction_post_weight_and_water_records_request import WaterRestrictionPostWeightAndWaterRecordsRequest
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
    body = allen_powerplatform_client.WaterRestrictionPostWeightAndWaterRecordsRequest() # WaterRestrictionPostWeightAndWaterRecordsRequest |  (optional)

    try:
        # Post Weight and Water Record
        api_response = api_instance.water_restriction_post_weight_and_water_records(api_version=api_version, body=body)
        print("The response of DefaultApi->water_restriction_post_weight_and_water_records:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->water_restriction_post_weight_and_water_records: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_version** | **int**|  | [optional] 
 **body** | [**WaterRestrictionPostWeightAndWaterRecordsRequest**](WaterRestrictionPostWeightAndWaterRecordsRequest.md)|  | [optional] 

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
**0** | default |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **water_restriction_update_restriction_status**
> object water_restriction_update_restriction_status(api_version=api_version, body=body)

Update Water Restriction Status

Update water restriction status for mouse in water restricted mice table

### Example

* OAuth Authentication (oauth2-auth):
* OAuth Authentication (oAuthClientCredentials):
* OAuth Authentication (certOauth):

```python
import allen_powerplatform_client
from allen_powerplatform_client.models.water_restriction_update_restriction_status_request import WaterRestrictionUpdateRestrictionStatusRequest
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
    body = allen_powerplatform_client.WaterRestrictionUpdateRestrictionStatusRequest() # WaterRestrictionUpdateRestrictionStatusRequest |  (optional)

    try:
        # Update Water Restriction Status
        api_response = api_instance.water_restriction_update_restriction_status(api_version=api_version, body=body)
        print("The response of DefaultApi->water_restriction_update_restriction_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->water_restriction_update_restriction_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_version** | **int**|  | [optional] 
 **body** | [**WaterRestrictionUpdateRestrictionStatusRequest**](WaterRestrictionUpdateRestrictionStatusRequest.md)|  | [optional] 

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
**0** | default |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **water_restriction_update_target_weight_percent**
> object water_restriction_update_target_weight_percent(api_version=api_version, body=body)

Update Target Weight Percent

Update the target weight percent for a water restricted mouse

### Example

* OAuth Authentication (oauth2-auth):
* OAuth Authentication (oAuthClientCredentials):
* OAuth Authentication (certOauth):

```python
import allen_powerplatform_client
from allen_powerplatform_client.models.water_restriction_update_target_weight_percent_request import WaterRestrictionUpdateTargetWeightPercentRequest
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
    body = allen_powerplatform_client.WaterRestrictionUpdateTargetWeightPercentRequest() # WaterRestrictionUpdateTargetWeightPercentRequest |  (optional)

    try:
        # Update Target Weight Percent
        api_response = api_instance.water_restriction_update_target_weight_percent(api_version=api_version, body=body)
        print("The response of DefaultApi->water_restriction_update_target_weight_percent:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->water_restriction_update_target_weight_percent: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_version** | **int**|  | [optional] 
 **body** | [**WaterRestrictionUpdateTargetWeightPercentRequest**](WaterRestrictionUpdateTargetWeightPercentRequest.md)|  | [optional] 

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
**0** | default |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

