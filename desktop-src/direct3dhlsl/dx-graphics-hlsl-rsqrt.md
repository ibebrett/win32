---
title: rsqrt
description: Returns the reciprocal of the square root of the specified value.
ms.assetid: '4e266e41-cde9-4a59-8937-98bfc63f3b5d'
keywords: ["rsqrt HLSL"]
topic_type:
- apiref
api_name:
- rsqrt
api_type:
- NA
---

# rsqrt

Returns the reciprocal of the square root of the specified value.



| *ret* rsqrt(*x*) |
|------------------|



�

## Parameters



| Item                                                   | Description                            |
|--------------------------------------------------------|----------------------------------------|
| <span id="x"></span><span id="X"></span>*x*<br/> | \[in\] The specified value.<br/> |



�

## Return Value

The reciprocal of the square root of the *x* parameter.

## Remarks

This function uses the following formula: 1 / **sqrt**(*x*).

## Type Description



| Name  | [**Template Type**](dx-graphics-hlsl-intrinsic-functions.md)                                                  | [**Component Type**](dx-graphics-hlsl-intrinsic-functions.md) | Size                           |
|-------|----------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------|--------------------------------|
| *x*   | [**scalar**](dx-graphics-hlsl-intrinsic-functions.md#component-and-template-types), **vector**, or **matrix** | [**float**](https://msdn.microsoft.com/library/windows/desktop/aa383751)                        | any                            |
| *ret* | same as input *x*                                                                                              | [**float**](https://msdn.microsoft.com/library/windows/desktop/aa383751)                        | same dimension(s) as input *x* |



�

## Minimum Shader Model

This function is supported in the following shader models.



| Shader Model                                                                       | Supported           |
|------------------------------------------------------------------------------------|---------------------|
| [Shader Model 2 (DirectX HLSL)](dx-graphics-hlsl-sm2.md) and higher shader models | yes                 |
| [Shader Model 1 (DirectX HLSL)](dx-graphics-hlsl-sm1.md)                          | yes (vs\_1\_1 only) |



�

## See also

<dl> <dt>

[**Intrinsic Functions (DirectX HLSL)**](dx-graphics-hlsl-intrinsic-functions.md)
</dt> </dl>

�

�




