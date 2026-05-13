# ValidateEmailInSystemUsersDefaultResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status_code** | **int** | status_code | [optional] 
**status_message** | **str** | status_message | [optional] 
**user_guid** | **str** | user_guid | [optional] 
**full_name** | **str** | full_name | [optional] 
**email_address** | **str** | email_address | [optional] 

## Example

```python
from allen_powerplatform_client.models.validate_email_in_system_users_default_response import ValidateEmailInSystemUsersDefaultResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ValidateEmailInSystemUsersDefaultResponse from a JSON string
validate_email_in_system_users_default_response_instance = ValidateEmailInSystemUsersDefaultResponse.from_json(json)
# print the JSON string representation of the object
print(ValidateEmailInSystemUsersDefaultResponse.to_json())

# convert the object into a dict
validate_email_in_system_users_default_response_dict = validate_email_in_system_users_default_response_instance.to_dict()
# create an instance of ValidateEmailInSystemUsersDefaultResponse from a dict
validate_email_in_system_users_default_response_from_dict = ValidateEmailInSystemUsersDefaultResponse.from_dict(validate_email_in_system_users_default_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


