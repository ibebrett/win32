---
Description: 'This operator tests if one reference time is greater than another.'
ms.assetid: 'db281040-9bcf-41fc-95b4-5481ffc5061f'
title: 'COARefTime.operator&gt; method'
---

# COARefTime.operator&gt; method

This operator tests if one reference time is greater than another.

## Syntax


```C++
BOOL operator>(
  [ref]�const COARefTime &amp;rt
);
```



## Parameters

<dl> <dt>

*rt* \[ref\]
</dt> <dd>

Reference to the **COARefTime** object to compare.

</dd> </dl>

## Return value

Returns **TRUE** if this object is strictly greater than *rt*. Otherwise, returns **FALSE**.

## Requirements



|                    |                                                                                                                                                                                            |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Ctlutil.h (include Streams.h)</dt> </dl>                                                                                   |
| Library<br/> | <dl> <dt>Strmbase.lib (retail builds); </dt> <dt>Strmbasd.lib (debug builds)</dt> </dl> |



## See also

<dl> <dt>

[**COARefTime Class**](coareftime.md)
</dt> </dl>

�

�



