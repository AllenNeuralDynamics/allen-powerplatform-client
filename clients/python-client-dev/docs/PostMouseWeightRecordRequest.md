# PostMouseWeightRecordRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**mouse_id** | **str** | mouse_ID | [optional] 
**mouse_guid** | **str** | mouse_GUID | [optional] 
**weight** | **float** | weight | [optional] 
**is_baseline_weight** | **bool** | is_baseline_weight | [optional] 
**date_time** | **str** | date_time | [optional] 
**operator_user_guid** | **str** | operator_userGUID | [optional] 
**notes** | **str** | notes | [optional] 
**workstation** | **str** | workstation | [optional] 
**software_source** | **str** | software_source | [optional] 
**software_version** | **str** | software_version | [optional] 

## Example

```python
from allen_powerplatform_client.models.post_mouse_weight_record_request import PostMouseWeightRecordRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PostMouseWeightRecordRequest from a JSON string
post_mouse_weight_record_request_instance = PostMouseWeightRecordRequest.from_json(json)
# print the JSON string representation of the object
print(PostMouseWeightRecordRequest.to_json())

# convert the object into a dict
post_mouse_weight_record_request_dict = post_mouse_weight_record_request_instance.to_dict()
# create an instance of PostMouseWeightRecordRequest from a dict
post_mouse_weight_record_request_from_dict = PostMouseWeightRecordRequest.from_dict(post_mouse_weight_record_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


