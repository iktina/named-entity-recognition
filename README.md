# Named Entity Recognition
Named Entity Recognition service for SingularityNET
## Welcome
## What’s the point?
The service outputs recognize entities inside sentences.
## Model details:
Input a piece of text and identify specific ORGANIZATIONS, PLACES, and PERSONS within the provided text.
### The user must provide the following inputs in order to start the service and get a response:
### Inputs:
`value`: json string

Example of input file content:

`[{"id": "1", "sentence": "Microsoft is headquartered in the United States"}, {"id": "2", "sentence": "United States is a big country"}, {"id": "3", "sentence": "Mike lives in Brazil"}]`

### Outputs:
`value`: json string

Example of output file content:
`[{'id': '1', 'entities': [{'name': 'Microsoft', 'type': 'ORG', 'start_span': 0, 'end_span': 9}, {'name': 'United States', 'type': 'LOC', 'start_span': 34, 'end_span': 47}]}, {'id': '2', 'entities': [{'name': 'United States', 'type': 'LOC', 'start_span': 0, 'end_span': 13}]}, {'id': '3', 'entities': [{'name': 'Mike', 'type': 'PER', 'start_span': 0, 'end_span': 4}, {'name': 'Brazil', 'type': 'LOC', 'start_span': 14, 'end_span': 20}]}]`

## What to expect from this service?
### Inputs:
```"": [{"id": "1", "sentence": "Microsoft is headquartered in the United States"}, {"id": "2", "sentence": "United States is a big country"}, {"id": "3", "sentence": "Mike lives in Brazil"}]```
### Outputs:
```"": [{'id': '1', 'entities': [{'name': 'Microsoft', 'type': 'ORG', 'start_span': 0, 'end_span': 9}, {'name': 'United States', 'type': 'LOC', 'start_span': 34, 'end_span': 47}]}, {'id': '2', 'entities': [{'name': 'United States', 'type': 'LOC', 'start_span': 0, 'end_span': 13}]}, {'id': '3', 'entities': [{'name': 'Mike', 'type': 'PER', 'start_span': 0, 'end_span': 4}, {'name': 'Brazil', 'type': 'LOC', 'start_span': 14, 'end_span': 20}]}]```
