---
title: "SMS_MeteredUser Class | Microsoft Docs"
ms.custom: ""
ms.date: "09/20/2016"
ms.prod: "configuration-manager"
ms.reviewer: ""
ms.suite: ""
ms.technology:
  - "configmgr-other"
ms.tgt_pltfrm: ""
ms.topic: "article"
applies_to:
  - "System Center Configuration Manager (current branch)"
ms.assetid: 368c8640-fb35-43bf-83c6-611c9fea173d
caps.latest.revision: 8
author: "shill-ms"
ms.author: "v-suhill"
manager: "mbaldwin"
---
# SMS_MeteredUser Server WMI Class
The `SMS_MeteredUser` Windows Management Instrumentation (WMI) class is an SMS Provider server class, in System Center Configuration Manager, that lists users that have used metered applications.  

 The following syntax is simplified from Managed Object Format (MOF) code and includes all inherited properties.  

## Syntax  

```  
Class SMS_MeteredUser : SMS_BaseClass  
{  
      String Domain;  
      String FullName;  
      UInt32 MeteredUserID;  
      String UserName;  
};  
```  

## Methods  
 The `SMS_MeteredUser` class does not define any methods.  

## Properties  
 `Domain`  
 Data type: `String`  

 Access type: Read/Write  

 Qualifiers: None  

 Domain to which the metered user belongs.  

 `FullName`  
 Data type: `String`  

 Access type: Read/Write  

 Qualifiers: None  

 Fully qualified domain name of the user in domain\user format.  

 `MeteredUserID`  
 Data type: `UInt32`  

 Access type: Read/Write  

 Qualifiers: [key]  

 ID for the metered user.  

 `UserName`  
 Data type: `String`  

 Access type: Read/Write  

 Qualifiers: None  

 Name of the metered user.  

## Remarks  
 There are no special class qualifiers for this class. For more information about both the class qualifiers and the property qualifiers included in the Properties section, see [Configuration Manager Class and Property Qualifiers](../../../develop/reference/misc/class-and-property-qualifiers.md).  

 This class is the source for the `MeteredUserID` foreign key used in other classes.  

## Requirements  

## Runtime Requirements  
 For more information, see [Configuration Manager Server Runtime Requirements](../../../develop/core/reqs/server-runtime-requirements.md).  

## Development Requirements  
 For more information, see [Configuration Manager Server Development Requirements](../../../develop/core/reqs/server-development-requirements.md).  

## See Also  
 [Software Metering Server WMI Classes](../../../develop/reference/apps/software-metering-server-wmi-classes.md)
