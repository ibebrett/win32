﻿---
Description: 'Sent to a child window when the user clicks the window''s title bar or when the window is activated, moved, or sized.'
ms.assetid: '6e60725d-aa01-48bb-86a5-f17f56b97d35'
title: 'WM\_CHILDACTIVATE message'
---

# WM\_CHILDACTIVATE message

Sent to a child window when the user clicks the window's title bar or when the window is activated, moved, or sized.

A window receives this message through its [**WindowProc**](windowproc.md) function.


```C++
#define WM_CHILDACTIVATE                0x0022
```



## Parameters

<dl> <dt>

*wParam* 
</dt> <dd>

This parameter is not used.

</dd> <dt>

*lParam* 
</dt> <dd>

This parameter is not used.

</dd> </dl>

## Return value

Type: **LRESULT**

If an application processes this message, it should return zero.

## Requirements



|                                     |                                                                                                          |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 2000 Professional \[desktop apps only\]<br/>                                               |
| Minimum supported server<br/> | Windows 2000 Server \[desktop apps only\]<br/>                                                     |
| Header<br/>                   | <dl> <dt>Winuser.h (include Windows.h)</dt> </dl> |



## See also

<dl> <dt>

**Reference**
</dt> <dt>

[**MoveWindow**](movewindow.md)
</dt> <dt>

[**SetWindowPos**](setwindowpos.md)
</dt> <dt>

**Conceptual**
</dt> <dt>

[Windows](windows.md)
</dt> </dl>

 

 



