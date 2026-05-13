# ValidateMouseInBehaviorTrainingDefaultResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status_code** | **int** | status_code | [optional] 
**status_message** | **str** | status_message | [optional] 
**behavior_training_guid** | **str** | behavior_training_guid | [optional] 
**active_record** | **bool** | active_record | [optional] 
**mouse_guid** | **str** | mouse_guid | [optional] 
**mouse_id** | **str** | mouse_id | [optional] 
**project_guid** | **str** | project_guid | [optional] 
**project_name** | **str** | project_name | [optional] 
**project_code** | **str** | project_code | [optional] 
**training_protocol** | **str** | training_protocol | [optional] 
**mouse_assignment_status_choice_value** | **int** | mouse_assignment_status_choice_value | [optional] 
**mouse_assignment_status_choice_label** | **str** | mouse_assignment_status_choice_label | [optional] 
**assigned_trainer_userguid** | **str** | assigned_trainer_userguid | [optional] 
**assigned_trainer_name** | **str** | assigned_trainer_name | [optional] 
**assigned_trainer_email** | **str** | assigned_trainer_email | [optional] 
**backup_trainer_userguid** | **str** | backup_trainer_userguid | [optional] 
**backup_trainer_name** | **str** | backup_trainer_name | [optional] 
**backup_trainer_email** | **str** | backup_trainer_email | [optional] 
**scientific_contact_userguid** | **str** | scientific_contact_userguid | [optional] 
**scientific_contact_name** | **str** | scientific_contact_name | [optional] 
**scientific_contact_email** | **str** | scientific_contact_email | [optional] 
**water_restriction_guid** | **str** | water_restriction_guid | [optional] 

## Example

```python
from allen_powerplatform_client.models.validate_mouse_in_behavior_training_default_response import ValidateMouseInBehaviorTrainingDefaultResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ValidateMouseInBehaviorTrainingDefaultResponse from a JSON string
validate_mouse_in_behavior_training_default_response_instance = ValidateMouseInBehaviorTrainingDefaultResponse.from_json(json)
# print the JSON string representation of the object
print(ValidateMouseInBehaviorTrainingDefaultResponse.to_json())

# convert the object into a dict
validate_mouse_in_behavior_training_default_response_dict = validate_mouse_in_behavior_training_default_response_instance.to_dict()
# create an instance of ValidateMouseInBehaviorTrainingDefaultResponse from a dict
validate_mouse_in_behavior_training_default_response_from_dict = ValidateMouseInBehaviorTrainingDefaultResponse.from_dict(validate_mouse_in_behavior_training_default_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


