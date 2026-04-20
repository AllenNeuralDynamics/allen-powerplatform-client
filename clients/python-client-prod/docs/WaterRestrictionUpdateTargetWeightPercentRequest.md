# WaterRestrictionUpdateTargetWeightPercentRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**water_restriction_guid** | **str** | WaterRestrictionGUID | [optional] 
**updated_percent** | **float** | updated_percent | [optional] 

## Example

```python
from allen_powerplatform_client.models.water_restriction_update_target_weight_percent_request import WaterRestrictionUpdateTargetWeightPercentRequest

# TODO update the JSON string below
json = "{}"
# create an instance of WaterRestrictionUpdateTargetWeightPercentRequest from a JSON string
water_restriction_update_target_weight_percent_request_instance = WaterRestrictionUpdateTargetWeightPercentRequest.from_json(json)
# print the JSON string representation of the object
print(WaterRestrictionUpdateTargetWeightPercentRequest.to_json())

# convert the object into a dict
water_restriction_update_target_weight_percent_request_dict = water_restriction_update_target_weight_percent_request_instance.to_dict()
# create an instance of WaterRestrictionUpdateTargetWeightPercentRequest from a dict
water_restriction_update_target_weight_percent_request_from_dict = WaterRestrictionUpdateTargetWeightPercentRequest.from_dict(water_restriction_update_target_weight_percent_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


