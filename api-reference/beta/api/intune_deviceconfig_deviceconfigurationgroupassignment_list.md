﻿# List deviceConfigurationGroupAssignments
List properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune_deviceconfig_deviceconfigurationgroupassignment.md) objects.
### Prerequisites
One of the following **scopes** is required to execute this API:

*DeviceManagementConfiguration.ReadWrite.All; DeviceManagementConfiguration.Read.All*
### HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /deviceConfigurationGroupAssignment/
GET /deviceManagement/deviceConfigurations/<id>/groupAssignments/
GET /deviceManagement/deviceConfigurations/<id>/rootCertificate//groupAssignments/
GET /deviceManagement/deviceConfigurations/<id>/microsoft.graph.iosScepCertificateProfile/rootCertificate//groupAssignments/
GET /deviceManagement/deviceConfigurations/<id>/microsoft.graph.macOSScepCertificateProfile/rootCertificate//groupAssignments/
GET /deviceManagement/deviceConfigurations/<id>/microsoft.graph.windows10VpnConfiguration/identityCertificate//groupAssignments/
GET /deviceManagement/deviceConfigurations/<id>/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate//groupAssignments/
```

### Request headers
|Header|Value|
|---|---|
|Authorization|Bearer &lt;token&gt; Required.|
|Accept|application/json|

### Request body
Do not supply a request body for this method.

### Response
If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationGroupAssignment](../resources/intune_deviceconfig_deviceconfigurationgroupassignment.md) objects in the response body.

### Example
##### Request
Here is an example of the request.
```http
GET https://graph.microsoft.com/beta/deviceConfigurationGroupAssignment/
```

##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 215

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
      "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
      "targetGroupId": "Target Group Id value"
    }
  ]
}
```



