# WaterRestrictionPostWeightAndWaterRecordsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**date_time** | **str** | date_time | [optional] 
**mouse_id** | **str** | mouse_ID | [optional] 
**mouse_guid** | **str** | mouse_GUID | [optional] 
**water_restriction_guid** | **str** | water_restriction_GUID | [optional] 
**team_guid** | **str** | team_GUID | [optional] 
**operator_user_guid** | **str** | operator_userGUID | [optional] 
**water_total** | **float** | water_total | [optional] 
**water_supplemental_provided** | **float** | water_supplemental_provided | [optional] 
**water_supplemental_recommended** | **float** | water_supplemental_recommended | [optional] 
**water_task** | **int** | water_task | [optional] 
**weight** | **float** | weight | [optional] 
**is_baseline_weight** | **bool** | is_baseline_weight | [optional] 
**notes** | **str** | notes | [optional] 
**software_source** | **str** | software_source | [optional] 
**workstation** | **str** | workstation | [optional] 
**software_version** | **str** | software_version | [optional] 

## Example

```python
from allen_powerplatform_client.models.water_restriction_post_weight_and_water_records_request import WaterRestrictionPostWeightAndWaterRecordsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of WaterRestrictionPostWeightAndWaterRecordsRequest from a JSON string
water_restriction_post_weight_and_water_records_request_instance = WaterRestrictionPostWeightAndWaterRecordsRequest.from_json(json)
# print the JSON string representation of the object
print(WaterRestrictionPostWeightAndWaterRecordsRequest.to_json())

# convert the object into a dict
water_restriction_post_weight_and_water_records_request_dict = water_restriction_post_weight_and_water_records_request_instance.to_dict()
# create an instance of WaterRestrictionPostWeightAndWaterRecordsRequest from a dict
water_restriction_post_weight_and_water_records_request_from_dict = WaterRestrictionPostWeightAndWaterRecordsRequest.from_dict(water_restriction_post_weight_and_water_records_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


