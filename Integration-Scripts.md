# Integration Scripts

## Example: REST API Integration
### Script to Create an Incident in ServiceNow
```javascript
var requestBody = {
  "short_description": "API-created incident",
  "priority": "2",
  "category": "Software",
};

var request = new sn_ws.RESTMessageV2();
request.setEndpoint('https://<instance>.service-now.com/api/now/table/incident');
request.setHttpMethod('POST');
request.setRequestBody(JSON.stringify(requestBody));
request.setBasicAuth('username', 'password');

var response = request.execute();
gs.info("Response: " + response.getBody());
