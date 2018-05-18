﻿---
Description: 'Describes a surface.'
ms.assetid: 'fad8ffdb-36e5-4695-b343-e1315357c31a'
title: 'D3DSURFACE\_DESC structure'
---

# D3DSURFACE\_DESC structure

Describes a surface.

## Syntax


```C++
typedef struct D3DSURFACE_DESC {
  D3DFORMAT           Format;
  D3DRESOURCETYPE     Type;
  DWORD               Usage;
  D3DPOOL             Pool;
  D3DMULTISAMPLE_TYPE MultiSampleType;
  DWORD               MultiSampleQuality;
  UINT                Width;
  UINT                Height;
} D3DSURFACE_DESC, *LPD3DSURFACE_DESC;
```



## Members

<dl> <dt>

**Format**
</dt> <dd>

Type: **[D3DFORMAT](d3dformat.md)**

</dd> <dd>

Member of the [D3DFORMAT](d3dformat.md) enumerated type, describing the surface format.

</dd> <dt>

**Type**
</dt> <dd>

Type: **[**D3DRESOURCETYPE**](direct3d9.d3dresourcetype)**

</dd> <dd>

Member of the [**D3DRESOURCETYPE**](direct3d9.d3dresourcetype) enumerated type, identifying this resource as a surface.

</dd> <dt>

**Usage**
</dt> <dd>

Type: **[**DWORD**](winprog.windows_data_types)**

</dd> <dd>

Either the D3DUSAGE\_DEPTHSTENCIL or D3DUSAGE\_RENDERTARGET values. For more information, see [**D3DUSAGE**](d3dusage.md).

</dd> <dt>

**Pool**
</dt> <dd>

Type: **[**D3DPOOL**](direct3d9.d3dpool)**

</dd> <dd>

Member of the [**D3DPOOL**](direct3d9.d3dpool) enumerated type, specifying the class of memory allocated for this surface.

</dd> <dt>

**MultiSampleType**
</dt> <dd>

Type: **[**D3DMULTISAMPLE\_TYPE**](direct3d9.d3dmultisample_type)**

</dd> <dd>

Member of the [**D3DMULTISAMPLE\_TYPE**](direct3d9.d3dmultisample_type) enumerated type, specifying the levels of full-scene multisampling supported by the surface.

</dd> <dt>

**MultiSampleQuality**
</dt> <dd>

Type: **[**DWORD**](winprog.windows_data_types)**

</dd> <dd>

Quality level. The valid range is between zero and one less than the level returned by pQualityLevels used by [**CheckDeviceMultiSampleType**](idirect3d9--checkdevicemultisampletype.md). Passing a larger value returns the error, D3DERR\_INVALIDCALL. The MultisampleQuality values of paired render targets, depth stencil surfaces and the MultiSample type must all match.

</dd> <dt>

**Width**
</dt> <dd>

Type: **[**UINT**](winprog.windows_data_types)**

</dd> <dd>

Width of the surface, in pixels.

</dd> <dt>

**Height**
</dt> <dd>

Type: **[**UINT**](winprog.windows_data_types)**

</dd> <dd>

Height of the surface, in pixels.

</dd> </dl>

## Requirements



|                   |                                                                                        |
|-------------------|----------------------------------------------------------------------------------------|
| Header<br/> | <dl> <dt>D3D9Types.h</dt> </dl> |



## See also

<dl> <dt>

[Direct3D Structures](dx9-graphics-reference-d3d-structures.md)
</dt> <dt>

[**GetLevelDesc**](idirect3dcubetexture9--getleveldesc.md)
</dt> <dt>

[**GetDesc**](idirect3dsurface9--getdesc.md)
</dt> <dt>

[**GetLevelDesc**](idirect3dtexture9--getleveldesc.md)
</dt> </dl>

 

 



