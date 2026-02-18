# GetTableRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**table_name** | **str** | Table name in Dataverse | 
**columns** | **str** | Comma-separated column names to select from the table | [optional] 
**filter** | **str** | OData-style filter expression | [optional] 
**order_by** | **str** | NOT IMPLEMENTED - OData-style orderby expression | [optional] 
**fetch_xml** | **str** | NOT IMPLEMENTED - Fetch XML query for advanced customization | [optional] 
**row_count** | **int** | NOT IMPLEMENTED - Number of rows to return, default 2000 | [optional] 

## Example

```python
from allen_powerplatform_client.models.get_table_request import GetTableRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GetTableRequest from a JSON string
get_table_request_instance = GetTableRequest.from_json(json)
# print the JSON string representation of the object
print(GetTableRequest.to_json())

# convert the object into a dict
get_table_request_dict = get_table_request_instance.to_dict()
# create an instance of GetTableRequest from a dict
get_table_request_from_dict = GetTableRequest.from_dict(get_table_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


