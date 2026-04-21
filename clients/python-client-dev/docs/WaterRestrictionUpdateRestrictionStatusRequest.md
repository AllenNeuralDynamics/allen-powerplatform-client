# WaterRestrictionUpdateRestrictionStatusRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**water_restriction_guid** | **str** | water_restriction_guid | [optional] 
**updated_water_restriction_status** | **str** | updated_water_restriction_status | [optional] 

## Example

```python
from allen_powerplatform_client.models.water_restriction_update_restriction_status_request import WaterRestrictionUpdateRestrictionStatusRequest

# TODO update the JSON string below
json = "{}"
# create an instance of WaterRestrictionUpdateRestrictionStatusRequest from a JSON string
water_restriction_update_restriction_status_request_instance = WaterRestrictionUpdateRestrictionStatusRequest.from_json(json)
# print the JSON string representation of the object
print(WaterRestrictionUpdateRestrictionStatusRequest.to_json())

# convert the object into a dict
water_restriction_update_restriction_status_request_dict = water_restriction_update_restriction_status_request_instance.to_dict()
# create an instance of WaterRestrictionUpdateRestrictionStatusRequest from a dict
water_restriction_update_restriction_status_request_from_dict = WaterRestrictionUpdateRestrictionStatusRequest.from_dict(water_restriction_update_restriction_status_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


