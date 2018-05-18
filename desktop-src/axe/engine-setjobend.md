---
title: Engine SetJobEnd method
description: Specifies the native interface for the Engine to invoke to notify the solution of a job end event.
ms.assetid: 'BF3B1623-4A0E-4EA3-840F-B7CB4BB70079'
keywords: ["SetJobEnd method Access Execution Engine", "SetJobEnd method Access Execution Engine , Engine interface", "Engine interface Access Execution Engine , SetJobEnd method"]
topic_type:
- apiref
api_name:
- Engine.SetJobEnd
api_location:
- AxeCore.dll
api_type:
- COM
---

# Engine::SetJobEnd method

Specifies the native interface for the [**Engine**](engine-if.md) to invoke to notify the solution of a job end event.

## Syntax


```C++
virtual HRESULT SetJobEnd(
  [in, optional]�IJobEndEventHandler *jobEnd
) = 0;
```



## Parameters

<dl> <dt>

*jobEnd* \[in, optional\]
</dt> <dd>

The native interface invoked by [**Engine**](engine-if.md) when a job end event occurs. This parameter can be **NULL** to remove an existing handler.

</dd> </dl>

## Return value

If successful, the method returns **S\_OK**.

If a job is running, the method returns **AXE\_E\_JOB\_RUNNING**. Event handlers cannot be changed while a job is running.

If a there are events already queued with the Asynchronous Procedure Call mechanism in the operating system, the method returns **AXE\_E\_QUEUED\_APC\_EVENTS**. The threading model cannot be changed until these queued events are processed.

## Remarks

Managed code uses the [**Engine.JobEnd \| jobend**](axe-engine_jobend_om) event.

## Requirements



|                                     |                                                                                         |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�7 \[desktop apps only\]<br/>                                              |
| Minimum supported server<br/> | Windows Server�2008�R2 \[desktop apps only\]<br/>                                 |
| Header<br/>                   | <dl> <dt>AxeHosting.h</dt> </dl> |
| DLL<br/>                      | <dl> <dt>AxeCore.dll</dt> </dl>  |



## See also

<dl> <dt>

[**Engine**](engine-if.md)
</dt> <dt>

[**IJobEndEventHandler**](ijobendeventhandler.md)
</dt> <dt>

[**OnJobEnd**](ievents-onjobend.md)
</dt> </dl>

�

�




