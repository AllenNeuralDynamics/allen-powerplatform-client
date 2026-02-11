# UpdateWaterRestrictionStatusRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**mouse_id** | **str** | mouse_id | [optional] 
**updated_water_restriction_status** | **str** | updated_water_restriction_status | [optional] 

## Example

```python
from allen_powerplatform_client.models.update_water_restriction_status_request import UpdateWaterRestrictionStatusRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateWaterRestrictionStatusRequest from a JSON string
update_water_restriction_status_request_instance = UpdateWaterRestrictionStatusRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateWaterRestrictionStatusRequest.to_json())

# convert the object into a dict
update_water_restriction_status_request_dict = update_water_restriction_status_request_instance.to_dict()
# create an instance of UpdateWaterRestrictionStatusRequest from a dict
update_water_restriction_status_request_from_dict = UpdateWaterRestrictionStatusRequest.from_dict(update_water_restriction_status_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


