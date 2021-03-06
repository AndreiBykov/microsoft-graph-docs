﻿# detectedApp resource type

> **Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.

A managed or unmanaged app that is installed on a managed device. Unmanaged apps will only appear for devices marked as corporate owned.
## Methods
|Method|Return Type|Description|
|---|---|---|
|[List detectedApps](../api/intune_devicefe_detectedapp_list.md)|[detectedApp](../resources/intune_devicefe_detectedapp.md) collection|List properties and relationships of the [detectedApp](../resources/intune_devicefe_detectedapp.md) objects.|
|[Get detectedApp](../api/intune_devicefe_detectedapp_get.md)|[detectedApp](../resources/intune_devicefe_detectedapp.md)|Read properties and relationships of the [detectedApp](../resources/intune_devicefe_detectedapp.md) object.|
|[List managedDevices](../api/intune_devicefe_manageddevice_list.md)|[managedDevice](../resources/intune_devicefe_manageddevice.md) collection|List properties and relationships of the [managedDevice](../resources/intune_devicefe_manageddevice.md) objects.|

## Properties
|Property|Type|Description|
|---|---|---|
|id|String|The unique Identifier for the detected application. This is automatically generated by Intune at the time the application is created. Read-only.|
|displayName|String|Name of the discovered application. Read-only|
|version|String|Version of the discovered application. Read-only|
|sizeInByte|Int64|Discovered application size in bytes. Read-only|
|deviceCount|Int32|The number of devices that have installed this application|

## Relationships
|Relationship|Type|Description|
|---|---|---|
|managedDevices|[managedDevice](../resources/intune_devicefe_manageddevice.md) collection|The devices that have the discovered application installed|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.detectedApp"
}
-->
```json
{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "String (identifier)",
  "displayName": "String",
  "version": "String",
  "sizeInByte": 1024,
  "deviceCount": 1024
}
```



