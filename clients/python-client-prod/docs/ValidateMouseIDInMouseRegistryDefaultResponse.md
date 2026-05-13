# ValidateMouseIDInMouseRegistryDefaultResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status_code** | **int** | StatusCode | [optional] 
**status_message** | **str** | StatusMessage | [optional] 
**mouse_guid** | **str** | MouseGUID | [optional] 
**mouse_id** | **str** | MouseID | [optional] 
**sex** | **str** | Sex | [optional] 
**date_of_birth** | **str** | DateOfBirth | [optional] 
**date_of_death** | **str** | DateOfDeath | [optional] 
**deceased** | **str** | Deceased | [optional] 
**reverse_light_cycle** | **str** | ReverseLightCycle | [optional] 
**project_guid** | **str** | ProjectGUID | [optional] 
**project_name** | **str** | ProjectName | [optional] 
**iacuc_guid** | **str** | IACUC GUID | [optional] 
**iacuc_protocol** | **str** | IACUCProtocol | [optional] 
**genotype** | **str** | Genotype | [optional] 

## Example

```python
from allen_powerplatform_client.models.validate_mouse_idin_mouse_registry_default_response import ValidateMouseIDInMouseRegistryDefaultResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ValidateMouseIDInMouseRegistryDefaultResponse from a JSON string
validate_mouse_idin_mouse_registry_default_response_instance = ValidateMouseIDInMouseRegistryDefaultResponse.from_json(json)
# print the JSON string representation of the object
print(ValidateMouseIDInMouseRegistryDefaultResponse.to_json())

# convert the object into a dict
validate_mouse_idin_mouse_registry_default_response_dict = validate_mouse_idin_mouse_registry_default_response_instance.to_dict()
# create an instance of ValidateMouseIDInMouseRegistryDefaultResponse from a dict
validate_mouse_idin_mouse_registry_default_response_from_dict = ValidateMouseIDInMouseRegistryDefaultResponse.from_dict(validate_mouse_idin_mouse_registry_default_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


