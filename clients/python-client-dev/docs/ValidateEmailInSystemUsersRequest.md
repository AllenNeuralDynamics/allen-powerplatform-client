# ValidateEmailInSystemUsersRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email_address** | **str** | email_address | [optional] 

## Example

```python
from allen_powerplatform_client.models.validate_email_in_system_users_request import ValidateEmailInSystemUsersRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ValidateEmailInSystemUsersRequest from a JSON string
validate_email_in_system_users_request_instance = ValidateEmailInSystemUsersRequest.from_json(json)
# print the JSON string representation of the object
print(ValidateEmailInSystemUsersRequest.to_json())

# convert the object into a dict
validate_email_in_system_users_request_dict = validate_email_in_system_users_request_instance.to_dict()
# create an instance of ValidateEmailInSystemUsersRequest from a dict
validate_email_in_system_users_request_from_dict = ValidateEmailInSystemUsersRequest.from_dict(validate_email_in_system_users_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


