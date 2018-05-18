---
title: DMsgrSessionManagerEvents OnLockResult event
description: Returns the result of a Lock and Key authentication transaction between a Messenger client and the Microsoft .NET Messenger Service.
ms.assetid: '2bdc03e0-6688-4550-bb86-46d1db7b666f'
keywords: ["OnLockResult event Windows Messenger", "OnLockResult event Windows Messenger , DMsgrSessionManagerEvents interface", "DMsgrSessionManagerEvents interface Windows Messenger , OnLockResult event"]
topic_type:
- apiref
api_name:
- DMsgrSessionManagerEvents.OnLockResult
api_location:
- Msnmsgrexe.adeb440d_7847_4f65_80bd_899870ed2ec9
api_type:
- COM
---

# DMsgrSessionManagerEvents::OnLockResult event

\[**OnLockResult** is no longer available for use as of Windows�Vista. See [Windows Messenger](im-messenger-entry.md) for more information.\]

Returns the result of a Lock and Key authentication transaction between a Messenger client and the Microsoft .NET Messenger Service.

## Syntax


```C++
void OnLockResult(
  [in]�long ��������lCookie,
  [in]�VARIANT_BOOL fSucceed = VARIANT_FALSE
);
```



## Parameters

<dl> <dt>

*lCookie* \[in\]
</dt> <dd>

**LONG** that has the same value that the Messenger client passed to the Microsoft .NET Messenger Service as the *lCookie* parameter of the [**RequestChallenge**](im-imsgrlock-requestchallenge-method.md) method.

</dd> <dt>

*fSucceed* \[in\]
</dt> <dd>

**VARIANT\_BOOL** that defines one of the following possible values.



| Value                                                                                                                                                                                                                    | Meaning                                                     |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------|
| <span id="VARIANT_FALSE"></span><span id="variant_false"></span><dl> <dt>**VARIANT\_FALSE**</dt> <dt>false</dt> </dl> | The authentication transaction was unsuccessful.<br/> |
| <span id="VARIANT_TRUE"></span><span id="variant_true"></span><dl> <dt>**VARIANT\_TRUE**</dt> <dt>true</dt> </dl>     | The authentication transaction was successful.<br/>   |



�

</dd> </dl>

## Return value

This event does not return a value.

## Requirements



|                                     |                                                                                                                                |
|-------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�2000 Professional, Windows�XP \[desktop apps only\]<br/>                                                         |
| Minimum supported server<br/> | Windows Server�2003 \[desktop apps only\]<br/>                                                                           |
| End of client support<br/>    | Windows�XP<br/>                                                                                                          |
| End of server support<br/>    | Windows Server�2003<br/>                                                                                                 |
| Product<br/>                  | Messenger 4.5<br/>                                                                                                       |
| Header<br/>                   | <dl> <dt>Sessions.h (include Mdispid.h)</dt> </dl>                      |
| IDL<br/>                      | <dl> <dt>Sessions.idl</dt> </dl>                                        |
| DLL<br/>                      | <dl> <dt>Msnmsgrexe.adeb440d\_7847\_4f65\_80bd\_899870ed2ec9</dt> </dl> |



## See also

<dl> <dt>

[**DMsgrSessionManagerEvents**](im-dmsgrsessionmanagerevents.md)
</dt> <dt>

[**OnLockChallenge**](im-dmsgrsessionmanagerevents-onlockchallenge.md)
</dt> <dt>

[**OnLockEnable**](im-dmsgrsessionmanagerevents-onlockenable.md)
</dt> <dt>

[**RequestChallenge**](im-imsgrlock-requestchallenge-method.md)
</dt> <dt>

[Messenger Session Invite and Messenger Private APIs](im-session-invite-ovw.md)
</dt> <dt>

[Messenger Lock and Key API](im-lock-and-key-ovw.md)
</dt> </dl>

�

�




