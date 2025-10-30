# FetchProjectByNameRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**project_name** | **str** | Project name from Projects table | [optional] 

## Example

```python
from allen_powerplatform_client.models.fetch_project_by_name_request import FetchProjectByNameRequest

# TODO update the JSON string below
json = "{}"
# create an instance of FetchProjectByNameRequest from a JSON string
fetch_project_by_name_request_instance = FetchProjectByNameRequest.from_json(json)
# print the JSON string representation of the object
print(FetchProjectByNameRequest.to_json())

# convert the object into a dict
fetch_project_by_name_request_dict = fetch_project_by_name_request_instance.to_dict()
# create an instance of FetchProjectByNameRequest from a dict
fetch_project_by_name_request_from_dict = FetchProjectByNameRequest.from_dict(fetch_project_by_name_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


