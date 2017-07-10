# @datafire/nrel_building_case_studies
The Buildings Database is a shared resource for the building industry. The Database, developed by the U.S. Department of Energy and the National Renewable Energy Laboratory (NREL), is a unique central repository of in-depth information and data on high-performance, green building projects across the United States and abroad.  

## Operation: project
A filterable list of projects.

### Input Schema
```json
{
  "type": "object",
  "properties": {
    "output_format": {
      "type": "string",
      "description": "Response Format",
      "enum": [
        "json",
        "xml"
      ]
    },
    "search": {
      "type": "string",
      "description": "Search Text"
    },
    "portal": {
      "type": "string",
      "description": "Portal ID"
    },
    "page": {
      "type": "integer",
      "description": "Page Number"
    },
    "city": {
      "type": "string",
      "description": "City"
    },
    "province": {
      "type": "string",
      "description": "State or Province (ex: 'CO', 'AZ')"
    },
    "region": {
      "type": "string",
      "description": "Climate Region.  Use integer from mapping (256: '1A: Very Hot - Humid', 257: '1B: Very Hot - Dry', 258: '2A: Hot - Humid', 259: '2B: Hot - Dry', 260: '3A: Warm - Humid', 261: '3B: Warm - Dry', 262: '3C: Warm - Marine', 263: '4A: Mixed - Humid', 264: '4B: Mixed - Dry', 265: '4C: Mixed - Marine', 266: '5A: Cool - Humid', 267: '5B: Cool - Dry', 268: '5C: Cool - Marine', 269: '6A: Cold - Humid', 270: '6B: Cold - Dry', 271: '7: Very Cold', 272: '8: Subarctic')"
    }
  },
  "additionalProperties": false,
  "required": [
    "output_format"
  ]
}
```
### Output Schema
```json
{}
```
## Operation: document
This API allows users to request metadata associated with the specific Document.

### Input Schema
```json
{
  "type": "object",
  "properties": {
    "output_format": {
      "type": "string",
      "description": "Response Format",
      "enum": [
        "json",
        "xml"
      ]
    },
    "project_id": {
      "type": "integer",
      "description": "Project ID"
    }
  },
  "additionalProperties": false,
  "required": [
    "output_format",
    "project_id"
  ]
}
```
### Output Schema
```json
{}
```