# PostWaterRecordRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**mouse_id** | **str** | mouse_id | [optional] 
**weight** | **float** | weight | [optional] 
**date_time** | **str** | date_time | [optional] 
**water_total** | **float** | water_total | [optional] 
**water_supplemental_provided** | **float** | water_supplemental_provided | [optional] 
**water_supplemental_recommended** | **float** | water_supplemental_recommended | [optional] 
**water_task** | **float** | water_task | [optional] 
**user_email** | **str** | user_email | [optional] 
**operator_notes** | **str** | operator_notes | [optional] 
**workstation** | **str** | workstation | [optional] 
**software_source** | **str** | software_source | [optional] 
**software_version** | **str** | software_version | [optional] 

## Example

```python
from allen_powerplatform_client.models.post_water_record_request import PostWaterRecordRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PostWaterRecordRequest from a JSON string
post_water_record_request_instance = PostWaterRecordRequest.from_json(json)
# print the JSON string representation of the object
print(PostWaterRecordRequest.to_json())

# convert the object into a dict
post_water_record_request_dict = post_water_record_request_instance.to_dict()
# create an instance of PostWaterRecordRequest from a dict
post_water_record_request_from_dict = PostWaterRecordRequest.from_dict(post_water_record_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


