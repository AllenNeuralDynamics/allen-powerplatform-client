# WaterRestrictionPostBaselineWeightRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**water_restriction_guid** | **str** | WaterRestrictionGUID | [optional] 
**baseline_weight** | **float** | baseline_weight | [optional] 

## Example

```python
from allen_powerplatform_client.models.water_restriction_post_baseline_weight_request import WaterRestrictionPostBaselineWeightRequest

# TODO update the JSON string below
json = "{}"
# create an instance of WaterRestrictionPostBaselineWeightRequest from a JSON string
water_restriction_post_baseline_weight_request_instance = WaterRestrictionPostBaselineWeightRequest.from_json(json)
# print the JSON string representation of the object
print(WaterRestrictionPostBaselineWeightRequest.to_json())

# convert the object into a dict
water_restriction_post_baseline_weight_request_dict = water_restriction_post_baseline_weight_request_instance.to_dict()
# create an instance of WaterRestrictionPostBaselineWeightRequest from a dict
water_restriction_post_baseline_weight_request_from_dict = WaterRestrictionPostBaselineWeightRequest.from_dict(water_restriction_post_baseline_weight_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


