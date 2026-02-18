# UpdateTargetWeightPercentageRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**mouse_guid** | **str** | MouseGUID | [optional] 
**updated_percent** | **float** | updated_percent | [optional] 

## Example

```python
from allen_powerplatform_client.models.update_target_weight_percentage_request import UpdateTargetWeightPercentageRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateTargetWeightPercentageRequest from a JSON string
update_target_weight_percentage_request_instance = UpdateTargetWeightPercentageRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateTargetWeightPercentageRequest.to_json())

# convert the object into a dict
update_target_weight_percentage_request_dict = update_target_weight_percentage_request_instance.to_dict()
# create an instance of UpdateTargetWeightPercentageRequest from a dict
update_target_weight_percentage_request_from_dict = UpdateTargetWeightPercentageRequest.from_dict(update_target_weight_percentage_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


