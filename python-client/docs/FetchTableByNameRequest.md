# FetchTableByNameRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**table_name** | **str** | Table name in Dataverse | 

## Example

```python
from allen_powerplatform_client.models.fetch_table_by_name_request import FetchTableByNameRequest

# TODO update the JSON string below
json = "{}"
# create an instance of FetchTableByNameRequest from a JSON string
fetch_table_by_name_request_instance = FetchTableByNameRequest.from_json(json)
# print the JSON string representation of the object
print(FetchTableByNameRequest.to_json())

# convert the object into a dict
fetch_table_by_name_request_dict = fetch_table_by_name_request_instance.to_dict()
# create an instance of FetchTableByNameRequest from a dict
fetch_table_by_name_request_from_dict = FetchTableByNameRequest.from_dict(fetch_table_by_name_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


