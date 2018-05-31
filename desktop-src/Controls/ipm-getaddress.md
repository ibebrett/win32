---
title: IPM\_GETADDRESS message
description: Gets the address values for all four fields in the IP address control.
ms.assetid: 4fe68d45-7d7f-46da-a110-65f899b3c393
keywords:
- IPM_GETADDRESS message Windows Controls
topic_type:
- apiref
api_name:
- IPM_GETADDRESS
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# IPM\_GETADDRESS message

Gets the address values for all four fields in the IP address control.

## Parameters

<dl> <dt>

*wParam* 
</dt> <dd>Must be zero.</dd> <dt>

*lParam* 
</dt> <dd>

A pointer to a **DWORD** value that receives the address. The field 3 value will be contained in bits 0 through 7. The field 2 value will be contained in bits 8 through 15. The field 1 value will be contained in bits 16 through 23. The field 0 value will be contained in bits 24 through 31. The [**FIRST\_IPADDRESS**](/windows/win32/Commctrl/nf-commctrl-first_ipaddress?branch=master), [**SECOND\_IPADDRESS**](/windows/win32/Commctrl/nf-commctrl-second_ipaddress?branch=master), [**THIRD\_IPADDRESS**](/windows/win32/Commctrl/nf-commctrl-third_ipaddress?branch=master), and [**FOURTH\_IPADDRESS**](/windows/win32/Commctrl/nf-commctrl-fourth_ipaddress?branch=master) macros can also be used to extract the address information. Zero will be returned as the address for any blank fields.

</dd> </dl>

## Return value

Returns the number of nonblank fields.

## Requirements



|                                     |                                                                                       |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista \[desktop apps only\]<br/>                                        |
| Minimum supported server<br/> | Windows Server 2003 \[desktop apps only\]<br/>                                  |
| Header<br/>                   | <dl> <dt>Commctrl.h</dt> </dl> |



 

 




