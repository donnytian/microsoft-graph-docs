﻿# Get deviceConfigurationUserStatus
Read properties and relationships of the [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) object.
### Prerequisites
One of the following **scopes** is required to execute this API:

*DeviceManagementConfiguration.ReadWrite.All; DeviceManagementConfiguration.Read.All*
### HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /deviceManagement/deviceConfigurations/<id>/userStatuses/<id>
GET /deviceManagement/deviceConfigurations/<id>/rootCertificate//userStatuses/<id>
GET /deviceManagement/deviceConfigurations/<id>/microsoft.graph.iosScepCertificateProfile/rootCertificate//userStatuses/<id>
GET /deviceManagement/deviceConfigurations/<id>/microsoft.graph.macOSScepCertificateProfile/rootCertificate//userStatuses/<id>
GET /deviceManagement/deviceConfigurations/<id>/microsoft.graph.windows10VpnConfiguration/identityCertificate//userStatuses/<id>
GET /deviceManagement/deviceConfigurations/<id>/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate//userStatuses/<id>
```

### Optional query parameters
This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.
### Request headers
|Header|Value|
|---|---|
|Authorization|Bearer &lt;token&gt; Required.|
|Accept|application/json|

### Request body
Do not supply a request body for this method.

### Response
If successful, this method returns a `200 OK` response code and [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) object in the response body.

### Example
##### Request
Here is an example of the request.
```http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/<id>/userStatuses/<id>
```

##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 241

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
    "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
  }
}
```



