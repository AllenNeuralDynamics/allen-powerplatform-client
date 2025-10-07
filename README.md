# Auto-generated Client Code

This repository contains auto-generated Python client code for Allen Dataverse Service, created using OpenAPI Generator from PowerAutomate flow specifications.

## Installation

```bash
pip install allen-dataverse-service-client
```

## Contributing

This package is generated from PowerAutomate flows and OpenAPI specifications. To contribute:

### 1. Update PowerAutomate Flows

- Navigate to PowerAutomate and locate the relevant flow
- Make necessary changes to the flow logic, inputs, or outputs
- Test the flow to ensure it works correctly
- Note any changes to input/output schemas

### 2. Update OpenAPI Specification

- Edit `dataverse.yaml` to reflect changes made to the PowerAutomate flows
- Update paths, parameters, request/response schemas as needed
- Ensure environment variable placeholders are properly used:
  - `${DATAVERSE_HOST}` for the host
  - `${DATAVERSE_WORKFLOW_*_PATH}` for workflow endpoints
  - `${DATAVERSE_API_VERSION}`, `${DATAVERSE_SP}`, `${DATAVERSE_SV}` for query parameters

### 3. Regenerate the Client

Run the client generation script:

```bash
# Set required environment variables
export DATAVERSE_HOST="your-host"
export DATAVERSE_WORKFLOW_PROJECT_PATH="/workflows/project-id/triggers/manual/run"
export DATAVERSE_WORKFLOW_TABLE_PATH="/workflows/table-id/triggers/manual/run"
export DATAVERSE_WORKFLOW_TABLES_PATH="/workflows/tables-id/triggers/manual/run"
export DATAVERSE_API_VERSION="2024-10-01"
export DATAVERSE_SP="/triggers/manual/run"
export DATAVERSE_SV="1.0"

# Generate the client
openapi-generator-cli generate \
  -i dataverse.yaml \
  -g python \
  -o allen-dataverse-service-client \
  --skip-validate-spec \
  --additional-properties packageName=allen_dataverse_service_client,projectName=allen-dataverse-service-client
```

Or use the provided Python script:

```bash
cd scripts
python generate_openapi.py
```

## Architecture

```
Dataverse → PowerAutomate Flows → OpenAPI Spec → Generated Python Client
```

## Configuration

Set the following environment variables:

```bash
DATAVERSE_HOST=your-environment.api.powerplatform.com
DATAVERSE_API_VERSION=2024-10-01
DATAVERSE_SP=/triggers/manual/run
DATAVERSE_SV=1.0

# Workflow paths
DATAVERSE_WORKFLOW_PROJECT_PATH=/workflows/project-workflow-id/triggers/manual/run
DATAVERSE_WORKFLOW_TABLE_PATH=/workflows/table-workflow-id/triggers/manual/run
DATAVERSE_WORKFLOW_TABLES_PATH=/workflows/tables-workflow-id/triggers/manual/run

# Signatures for authentication
DATAVERSE_SIG_PROJECT_BY_NAME=your-project-signature
DATAVERSE_SIG_TABLE_BY_NAME=your-table-signature
DATAVERSE_SIG_ALL_TABLES=your-tables-signature
```

## Available Operations

### Fetch Project by Name
Retrieve project data by project name.

### Fetch Table by Name  
Retrieve records from a specified Dataverse table.

### Fetch Table Names
Get a list of available tables in the Dataverse environment.

## Contributing

This package is generated from PowerAutomate flows and OpenAPI specifications. To contribute:

### 1. Update PowerAutomate Flows

- Navigate to PowerAutomate and locate the relevant flow
- Make necessary changes to the flow logic, inputs, or outputs
- Test the flow to ensure it works correctly
- Note any changes to input/output schemas

### 2. Update OpenAPI Specification

- Edit `dataverse.yaml` to reflect changes made to the PowerAutomate flows
- Update paths, parameters, request/response schemas as needed
- Ensure environment variable placeholders are properly used:
  - `${DATAVERSE_HOST}` for the host
  - `${DATAVERSE_WORKFLOW_*_PATH}` for workflow endpoints
  - `${DATAVERSE_API_VERSION}`, `${DATAVERSE_SP}`, `${DATAVERSE_SV}` for query parameters

### 3. Regenerate the Client

Run the client generation script:

```bash
# Set required environment variables
export DATAVERSE_HOST="your-host"
export DATAVERSE_WORKFLOW_PROJECT_PATH="/workflows/project-id/triggers/manual/run"
export DATAVERSE_WORKFLOW_TABLE_PATH="/workflows/table-id/triggers/manual/run"
export DATAVERSE_WORKFLOW_TABLES_PATH="/workflows/tables-id/triggers/manual/run"
export DATAVERSE_API_VERSION="2024-10-01"
export DATAVERSE_SP="/triggers/manual/run"
export DATAVERSE_SV="1.0"

# Generate the client
openapi-generator-cli generate \
  -i dataverse.yaml \
  -g python \
  -o allen-dataverse-service-client \
  --skip-validate-spec \
  --additional-properties packageName=allen_dataverse_service_client,projectName=allen-dataverse-service-client
```

Or use the provided Python script:

```bash
cd scripts
python generate_openapi.py
```

### 4. Test Changes

- Install the updated client: `pip install -e .`
- Run tests to verify functionality
- Update documentation if needed

### Development Setup

1. Clone the repository
2. Install development dependencies: `pip install -r requirements-dev.txt`
3. Set up environment variables as described above
4. Make your changes following the contribution process above

## Architecture

```
Dataverse → PowerAutomate Flows → OpenAPI Spec → Generated Python Client
```

This architecture allows for:
- Visual flow design in PowerAutomate with built-in error handling
- Type-safe Python client with full IntelliSense support
- Automatic API documentation through OpenAPI specification
- Easy maintenance through the PowerAutomate UI

## License

See LICENSE file for details.
