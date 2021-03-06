﻿# managedIOSStoreApp resource type

> **Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.

Contains properties and inherited properties for an iOS store app that you can manage with an Intune app protection policy.

Inherits from [managedApp](../resources/intune_apps_managedapp.md)

## Methods
|Method|Return Type|Description|
|---|---|---|
|[List managedIOSStoreApps](../api/intune_apps_managediosstoreapp_list.md)|[managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) collection|List properties and relationships of the [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) objects.|
|[Get managedIOSStoreApp](../api/intune_apps_managediosstoreapp_get.md)|[managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md)|Read properties and relationships of the [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) object.|
|[Create managedIOSStoreApp](../api/intune_apps_managediosstoreapp_create.md)|[managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md)|Create a new [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) object.|
|[Delete managedIOSStoreApp](../api/intune_apps_managediosstoreapp_delete.md)|None|Deletes a [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md).|
|[Update managedIOSStoreApp](../api/intune_apps_managediosstoreapp_update.md)|[managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md)|Update the properties of a [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) object.|
|[List mobileAppCategories](../api/intune_apps_managediosstoreapp_list_mobileappcategory.md)|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) collection|Get the mobileAppCategories from the categories navigation property.|
|[List mobileAppGroupAssignments](../api/intune_apps_managediosstoreapp_list_mobileappgroupassignment.md)|[mobileAppGroupAssignment](../resources/intune_apps_mobileappgroupassignment.md) collection|Get the mobileAppGroupAssignments from the groupAssignments navigation property.|
|[Get mobileAppInstallSummary](../api/intune_apps_managediosstoreapp_get_mobileappinstallsummary.md)|[mobileAppInstallSummary](../resources/intune_apps_mobileappinstallsummary.md)|Get the [mobileAppInstallSummary](../resources/intune_apps_mobileappinstallsummary.md) from the installSummary navigation property.|
|[List mobileAppInstallStatuses](../api/intune_apps_managediosstoreapp_list_mobileappinstallstatus.md)|[mobileAppInstallStatus](../resources/intune_apps_mobileappinstallstatus.md) collection|Get the mobileAppInstallStatuses from the deviceStatuses navigation property.|
|[List userAppInstallStatuses](../api/intune_apps_managediosstoreapp_list_userappinstallstatus.md)|[userAppInstallStatus](../resources/intune_apps_userappinstallstatus.md) collection|Get the userAppInstallStatuses from the userStatuses navigation property.|

## Properties
|Property|Type|Description|
|---|---|---|
|id|String|Key of the entity. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)|
|displayName|String|The admin provided or imported title of the app. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)|
|description|String|The description of the app. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)|
|publisher|String|The publisher of the app. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune_apps_mimecontent.md)|The large icon, to be displayed in the app details and used for upload of the icon. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)|
|createdDateTime|DateTimeOffset|The date and time the app was created. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the app was last modified. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)|
|isFeatured|Boolean|The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)|
|privacyInformationUrl|String|The privacy statement Url. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)|
|informationUrl|String|The more information Url. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)|
|owner|String|The owner of the app. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)|
|developer|String|The developer of the app. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)|
|notes|String|Notes for the app. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)|
|uploadState|Int32|The upload state. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)|
|appAvailability|String|The Application's availability. Inherited from [managedApp](../resources/intune_apps_managedapp.md) Possible values are: `global`, `lineOfBusiness`.|
|version|String|The Application's version. Inherited from [managedApp](../resources/intune_apps_managedapp.md)|
|bundleId|String|The app's bundle ID.|

## Relationships
|Relationship|Type|Description|
|---|---|---|
|categories|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) collection|The list of categories for this app. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)|
|groupAssignments|[mobileAppGroupAssignment](../resources/intune_apps_mobileappgroupassignment.md) collection|The list of group assignments for this mobile app. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)|
|installSummary|[mobileAppInstallSummary](../resources/intune_apps_mobileappinstallsummary.md)|Mobile App Install Summary. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune_apps_mobileappinstallstatus.md) collection|The list of installation states for this mobile app. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)|
|userStatuses|[userAppInstallStatus](../resources/intune_apps_userappinstallstatus.md) collection|The list of installation states for this mobile app. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedIOSStoreApp"
}
-->
```json
{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "uploadState": 1024,
  "appAvailability": "String",
  "version": "String",
  "bundleId": "String"
}
```



