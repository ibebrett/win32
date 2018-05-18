---
Description: 'The SetPositions method sets the current position and the stop position. This method implements the IMediaSeeking::SetPositions method.'
ms.assetid: 'd4425221-e20f-4e51-8a33-a74fa21f9117'
title: 'CPosPassThru.SetPositions method'
---

# CPosPassThru.SetPositions method

The `SetPositions` method sets the current position and the stop position. This method implements the [**IMediaSeeking::SetPositions**](imediaseeking-setpositions.md) method.

## Syntax


```C++
HRESULT SetPositions(
  �LONGLONG *pCurrent,
  �DWORD ���dwCurrentFlags,
  �LONGLONG *pStop,
  �DWORD ���dwStopFlags
);
```



## Parameters

<dl> <dt>

*pCurrent* 
</dt> <dd>

Pointer to a variable that specifies the current position, in units of the current time format.

</dd> <dt>

*dwCurrentFlags* 
</dt> <dd>

Bitwise combination of flags. See [**IMediaSeeking::SetPositions**](imediaseeking-setpositions.md) for more information.

</dd> <dt>

*pStop* 
</dt> <dd>

Pointer to a variable that specifies the stop time, in units of the current time format.

</dd> <dt>

*dwStopFlags* 
</dt> <dd>

Bitwise combination of flags. See [**IMediaSeeking::SetPositions**](imediaseeking-setpositions.md) for more information.

</dd> </dl>

## Return value

Returns the **HRESULT** value from the connected pin.

## Requirements



|                    |                                                                                                                                                                                            |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Ctlutil.h (include Streams.h)</dt> </dl>                                                                                   |
| Library<br/> | <dl> <dt>Strmbase.lib (retail builds); </dt> <dt>Strmbasd.lib (debug builds)</dt> </dl> |



## See also

<dl> <dt>

[**CPosPassThru Class**](cpospassthru.md)
</dt> </dl>

�

�



