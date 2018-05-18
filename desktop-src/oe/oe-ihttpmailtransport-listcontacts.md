---
title: IHTTPMailTransport ListContacts method
description: Returns a list of contacts for the specified resource.
ms.assetid: 'd60bf242-f676-4b88-8c2a-264cbe87e8f9'
keywords: ["ListContacts method Windows Mail (formerly Outlook Express)", "ListContacts method Windows Mail (formerly Outlook Express) , IHTTPMailTransport interface", "IHTTPMailTransport interface Windows Mail (formerly Outlook Express) , ListContacts method"]
topic_type:
- apiref
api_name:
- IHTTPMailTransport.ListContacts
api_location:
- Inetcomm.dll
api_type:
- COM
---

# IHTTPMailTransport::ListContacts method

\[**IHTTPMailTransport::ListContacts** is available for use in the operating systems specified in the Requirements section. It may be altered or unavailable in subsequent versions.\]

Returns a list of contacts for the specified resource.

## Syntax


```C++
HRESULT ListContacts(
  [in]�LPCSTR pszPath,
  [in]�DWORD �dwContext
);
```



## Parameters

<dl> <dt>

*pszPath* \[in\]
</dt> <dd>

Type: **LPCSTR**

Specifies an **LPCSTR** that contains a **null**-terminated string that is the complete URL to the resource.

</dd> <dt>

*dwContext* \[in\]
</dt> <dd>

Type: **DWORD**

Currently unused. Should be set to zero.

</dd> </dl>

## Return value

Type: **HRESULT**

Returns one of the following values.



| Return code                                                                                   | Description                                                      |
|-----------------------------------------------------------------------------------------------|------------------------------------------------------------------|
| <dl> <dt>**S\_OK**</dt> </dl>          | Indicates success. <br/>                                   |
| <dl> <dt>**E\_INVALIDARG**</dt> </dl>  | Indicates that *pszPath* is **NULL**. <br/>                |
| <dl> <dt>**E\_OUTOFMEMORY**</dt> </dl> | Indicates that an attempt to allocate memory failed. <br/> |



�

## Requirements



|                                     |                                                                                                                |
|-------------------------------------|----------------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�XP \[desktop apps only\]<br/>                                                                    |
| Minimum supported server<br/> | Windows Server�2003 \[desktop apps only\]<br/>                                                           |
| Product<br/>                  | Outlook Express 6.0<br/>                                                                                 |
| Header<br/>                   | <dl> <dt>Imnxport.h</dt> </dl>                          |
| IDL<br/>                      | <dl> <dt>Imnxport.idl</dt> </dl>                        |
| DLL<br/>                      | <dl> <dt>Inetcomm.dll (version 6.0 or later)</dt> </dl> |



�

�




