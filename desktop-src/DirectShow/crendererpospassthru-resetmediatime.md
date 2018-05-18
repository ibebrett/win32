---
Description: 'The ResetMediaTime method resets the cached time stamps to zero.'
ms.assetid: '80dd2ae3-0a83-4017-8860-a089bef9a919'
title: 'CRendererPosPassThru.ResetMediaTime method'
---

# CRendererPosPassThru.ResetMediaTime method

The `ResetMediaTime` method resets the cached time stamps to zero.

## Syntax


```C++
HRESULT ResetMediaTime();
```



## Parameters

This method has no parameters.

## Return value

Returns S\_OK.

## Remarks

The filter should call this method whenever the time stamps cached by the [**CRendererPosPassThru::RegisterMediaTime**](crendererpospassthru-registermediatime.md) method become invalid. Specifically, it should call this method in response to the [**IPin::EndFlush**](ipin-endflush.md) and [**IMediaFilter::Stop**](imediafilter-stop.md) methods.

After this method is called, the [**CRendererPosPassThru::GetMediaTime**](crendererpospassthru-getmediatime.md) method returns zero for the start and end times.

## Requirements



|                    |                                                                                                                                                                                            |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Ctlutil.h (include Streams.h)</dt> </dl>                                                                                   |
| Library<br/> | <dl> <dt>Strmbase.lib (retail builds); </dt> <dt>Strmbasd.lib (debug builds)</dt> </dl> |



�

�



