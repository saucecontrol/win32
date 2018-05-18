﻿---
Description: 'Creates an empty volume texture, adjusting the calling parameters as needed.'
ms.assetid: '8fc515cd-2fb3-40c7-8192-a41d93ac1e99'
title: D3DXCreateVolumeTexture function
---

# D3DXCreateVolumeTexture function

Creates an empty volume texture, adjusting the calling parameters as needed.

## Syntax


```C++
HRESULT D3DXCreateVolumeTexture(
  _In_  LPDIRECT3DDEVICE9        pDevice,
  _In_  UINT                     Width,
  _In_  UINT                     Height,
  _In_  UINT                     Depth,
  _In_  UINT                     MipLevels,
  _In_  DWORD                    Usage,
  _In_  D3DFORMAT                Format,
  _In_  D3DPOOL                  Pool,
  _Out_ LPDIRECT3DVOLUMETEXTURE9 *ppVolumeTexture
);
```



## Parameters

<dl> <dt>

*pDevice* \[in\]
</dt> <dd>

Type: **[**LPDIRECT3DDEVICE9**](idirect3ddevice9.md)**

Pointer to an [**IDirect3DDevice9**](idirect3ddevice9.md) interface, representing the device to be associated with the volume texture.

</dd> <dt>

*Width* \[in\]
</dt> <dd>

Type: **[**UINT**](winprog.windows_data_types)**

Width in pixels. This value must be nonzero. The maximum dimension that a driver supports (for width, height, and depth) can be found in MaxVolumeExtent in [**D3DCAPS9**](d3dcaps9.md).

</dd> <dt>

*Height* \[in\]
</dt> <dd>

Type: **[**UINT**](winprog.windows_data_types)**

Height in pixels. This value must be nonzero. The maximum dimension that a driver supports (for width, height, and depth) can be found in MaxVolumeExtent in [**D3DCAPS9**](d3dcaps9.md).

</dd> <dt>

*Depth* \[in\]
</dt> <dd>

Type: **[**UINT**](winprog.windows_data_types)**

Depth in pixels. This value must be nonzero. The maximum dimension that a driver supports (for width, height, and depth) can be found in MaxVolumeExtent in [**D3DCAPS9**](d3dcaps9.md).

</dd> <dt>

*MipLevels* \[in\]
</dt> <dd>

Type: **[**UINT**](winprog.windows_data_types)**

Number of mip levels requested. If this value is zero or D3DX\_DEFAULT, a complete mipmap chain is created.

</dd> <dt>

*Usage* \[in\]
</dt> <dd>

Type: **[**DWORD**](winprog.windows_data_types)**

0 or D3DUSAGE\_DYNAMIC. For more information about using dynamic textures, see [Using Dynamic Textures](performance-optimizations.md).

</dd> <dt>

*Format* \[in\]
</dt> <dd>

Type: **[D3DFORMAT](d3dformat.md)**

Member of the [D3DFORMAT](d3dformat.md) enumerated type, describing the requested pixel format for the volume texture. The returned volume texture might have a different format from that specified by Format. Applications should check the format of the returned volume texture.

</dd> <dt>

*Pool* \[in\]
</dt> <dd>

Type: **[**D3DPOOL**](direct3d9.d3dpool)**

Member of the [**D3DPOOL**](direct3d9.d3dpool) enumerated type, describing the memory class into which the volume texture should be placed.

</dd> <dt>

*ppVolumeTexture* \[out\]
</dt> <dd>

Type: **[**LPDIRECT3DVOLUMETEXTURE9**](idirect3dvolumetexture9.md)\***

Address of a pointer to an [**IDirect3DVolumeTexture9**](idirect3dvolumetexture9.md) interface, representing the created volume texture object.

</dd> </dl>

## Return value

Type: **[**HRESULT**](455d07e9-52c3-4efb-a9dc-2955cbfd38cc)**

If the function succeeds, the return value is D3D\_OK. If the function fails, the return value can be one of the following: D3DERR\_NOTAVAILABLE, D3DERR\_OUTOFVIDEOMEMORY, D3DERR\_INVALIDCALL, E\_OUTOFMEMORY .

## Remarks

Internally, D3DXCreateVolumeTexture uses [**D3DXCheckVolumeTextureRequirements**](d3dxcheckvolumetexturerequirements.md) to adjust the calling parameters. Therefore, calls to D3DXCreateVolumeTexture will often succeed where calls to [**CreateVolumeTexture**](idirect3ddevice9--createvolumetexture.md) would fail.

## Requirements



|                    |                                                                                       |
|--------------------|---------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>D3dx9tex.h</dt> </dl> |
| Library<br/> | <dl> <dt>D3dx9.lib</dt> </dl>  |



## See also

<dl> <dt>

[Texture Functions in D3DX 9](dx9-graphics-reference-d3dx-functions-texture.md)
</dt> </dl>

 

 



