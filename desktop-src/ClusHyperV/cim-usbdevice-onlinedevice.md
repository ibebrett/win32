---
title: OnlineDevice method of the CIM\_USBDevice class
description: Deprecated description Brings the logical device online so it can accept requests, or offline so it can no longer accept requests. This method is deprecated. Instead we recommend that you use the RequestStateChange method.
audience: developer
author: REDMOND\\markl
manager: REDMOND\\markl
ms.assetid: 'c98c232d-4a49-48f8-9b37-c13466a55349'
ms.prod: 'windows-server-dev'
ms.technology:
- 'failover-cluster-hyperv'
- 'windows-management-instrumentation'
ms.tgt_platform: multiple
keywords: ["OnlineDevice method", "OnlineDevice method, CIM_USBDevice class", "CIM_USBDevice class, OnlineDevice method"]
topic_type:
- apiref
api_name:
- CIM_USBDevice.OnlineDevice
api_location:
- VMMS.exe
api_type:
- COM
---

# OnlineDevice method of the CIM\_USBDevice class

**Deprecated description:** Brings the logical device online so it can accept requests, or offline so it can no longer accept requests.

This method is deprecated. Instead we recommend that you use the **RequestStateChange** method.

## Syntax


```mof
uint32 OnlineDevice(
  [in]�boolean Online
);
```



## Parameters

<dl> <dt>

*Online* \[in\]
</dt> <dd>

**true** to bring the device online, **false** to take the device offline.

</dd> </dl>

## Return value

The possible return values are:

<dl> <dt>


</dt> <dd>

0

The operation completed successfully.

</dd> <dt>


</dt> <dd>

1

The operation was not completed because it is not supported.

</dd> <dt>


</dt> <dd>

2

The operation is not supported when the device is in the current state.

</dd> <dt>


</dt> <dd>

3�...

The operation was not completed because an error occurred.

</dd> </dl>

## Requirements



|                                     |                                                                                                        |
|-------------------------------------|--------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | None supported<br/>                                                                              |
| Minimum supported server<br/> | Windows Server�2016<br/>                                                                         |
| Namespace<br/>                | Root\\HyperVCluster\\v2<br/>                                                                     |
| MOF<br/>                      | <dl> <dt>WindowsHyperVCluster.V2.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>VMMS.exe</dt> </dl>                    |



## See also

<dl> <dt>

[**CIM\_USBDevice**](cim-usbdevice.md)
</dt> </dl>

�

�




