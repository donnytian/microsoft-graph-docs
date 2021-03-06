﻿# Update mobileAppCategory
Update the properties of a [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) object.
### Prerequisites
One of the following **scopes** is required to execute this API:

*DeviceManagementApps.ReadWrite.All*
### HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
```http
PATCH /deviceAppManagement/mobileAppCategories/<id>
PATCH /deviceAppManagement/mobileApps/<id>/categories/<id>
```

### Request headers
|Header|Value|
|---|---|
|Authorization|Bearer &lt;token&gt; Required.|
|Accept|application/json|

### Request body
In the request body, supply a JSON representation of a [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) object.
The following table shows the properties that are required when you create a [mobileAppCategory](../resources/intune_apps_mobileappcategory.md).

|Property|Type|Description|
|---|---|---|
|id|String|The key of the entity.|
|displayName|String|The name of the app category.|



### Response
If successful, this method returns a `200 OK` response code and an updated [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) object in the response body.

### Example
##### Request
Here is an example of the request.
```http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories/<id>
Content-type: application/json
Content-length: 43

{
  "displayName": "Display Name value"
}
```

##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 148

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
  "displayName": "Display Name value"
}
```



