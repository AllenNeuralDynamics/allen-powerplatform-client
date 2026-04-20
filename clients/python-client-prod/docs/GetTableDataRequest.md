# GetTableDataRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**table_name** | **str** | table_name | [optional] 
**columns** | **str** | columns | [optional] 
**filter** | **str** | filter | [optional] 
**order_by** | **str** | order_by | [optional] 
**fetch_xml** | **str** | fetch_xml | [optional] 
**row_count** | **int** | row_count | [optional] 

## Example

```python
from allen_powerplatform_client.models.get_table_data_request import GetTableDataRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GetTableDataRequest from a JSON string
get_table_data_request_instance = GetTableDataRequest.from_json(json)
# print the JSON string representation of the object
print(GetTableDataRequest.to_json())

# convert the object into a dict
get_table_data_request_dict = get_table_data_request_instance.to_dict()
# create an instance of GetTableDataRequest from a dict
get_table_data_request_from_dict = GetTableDataRequest.from_dict(get_table_data_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


