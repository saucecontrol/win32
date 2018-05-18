﻿---
Description: 'Get a pointer to the constant table.'
ms.assetid: '5d836d99-783f-41e1-b7bf-d874d09a4892'
title: 'ID3DXTextureShader::GetConstantBuffer method'
---

# ID3DXTextureShader::GetConstantBuffer method

Get a pointer to the constant table.

## Syntax


```C++
HRESULT GetConstantBuffer(
  [out] LPD3DXBUFFER *ppConstantBuffer
);
```



## Parameters

<dl> <dt>

*ppConstantBuffer* \[out\]
</dt> <dd>

Type: **[**LPD3DXBUFFER**](id3dxbuffer.md)\***

Pointer to an [**ID3DXBuffer**](id3dxbuffer.md) interface, which contains the constants.

</dd> </dl>

## Return value

Type: **[**HRESULT**](455d07e9-52c3-4efb-a9dc-2955cbfd38cc)**

If the method succeeds, the return value is D3D\_OK. If the method fails, the return value can be one of the following: D3DERR\_INVALIDCALL, D3DXERR\_INVALIDDATA.

## Requirements



|                    |                                                                                          |
|--------------------|------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>D3DX9Shader.h</dt> </dl> |
| Library<br/> | <dl> <dt>D3dx9.lib</dt> </dl>     |



## See also

<dl> <dt>

[ID3DXTextureShader](id3dxtextureshader.md)
</dt> </dl>

 

 



