# ValidateMouseInWaterRestrictedMiceTableDefaultResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status_code** | **int** | status_code | [optional] 
**status_message** | **str** | status_message | [optional] 
**waterrestrictionguid** | **str** | waterrestrictionguid | [optional] 
**activerecord** | **bool** | activerecord | [optional] 
**mouseguid** | **str** | mouseguid | [optional] 
**mouseid** | **str** | mouseid | [optional] 
**baseline_weight** | **float** | baseline_weight | [optional] 
**target_weight_percentage** | **float** | target_weight_percentage | [optional] 
**target_weight** | **float** | target_weight | [optional] 
**low_weight_threshold** | **float** | low_weight_threshold | [optional] 
**team_guid** | **str** | team_guid | [optional] 
**team_name** | **str** | team_name | [optional] 
**behavior_training_guid** | **str** | behavior_training_guid | [optional] 
**watering_shift_value** | **int** | watering_shift_value | [optional] 
**watering_shift_label** | **str** | watering_shift_label | [optional] 
**water_restriction_status_value** | **int** | water_restriction_status_value | [optional] 
**water_restriction_status_label** | **str** | water_restriction_status_label | [optional] 
**watered_today** | **bool** | watered_today | [optional] 
**last_watered_datetime** | **str** | last_watered_datetime | [optional] 
**record_name** | **str** | record_name | [optional] 

## Example

```python
from allen_powerplatform_client.models.validate_mouse_in_water_restricted_mice_table_default_response import ValidateMouseInWaterRestrictedMiceTableDefaultResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ValidateMouseInWaterRestrictedMiceTableDefaultResponse from a JSON string
validate_mouse_in_water_restricted_mice_table_default_response_instance = ValidateMouseInWaterRestrictedMiceTableDefaultResponse.from_json(json)
# print the JSON string representation of the object
print(ValidateMouseInWaterRestrictedMiceTableDefaultResponse.to_json())

# convert the object into a dict
validate_mouse_in_water_restricted_mice_table_default_response_dict = validate_mouse_in_water_restricted_mice_table_default_response_instance.to_dict()
# create an instance of ValidateMouseInWaterRestrictedMiceTableDefaultResponse from a dict
validate_mouse_in_water_restricted_mice_table_default_response_from_dict = ValidateMouseInWaterRestrictedMiceTableDefaultResponse.from_dict(validate_mouse_in_water_restricted_mice_table_default_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


