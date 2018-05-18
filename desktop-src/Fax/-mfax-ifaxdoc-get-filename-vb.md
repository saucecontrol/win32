﻿---
Description: 'Sets or retrieves the FileName property for a FaxDoc object. The FileName property is a null-terminated string that contains the name of the document file associated with the object.'
ms.assetid: '5b1cda1b-0313-4761-b8cb-c21eddd922d5'
title: 'FaxDoc.FileName property'
---

# FaxDoc.FileName property

Sets or retrieves the **FileName** property for a [FaxDoc](-mfax-faxdoc.md) object. The **FileName** property is a null-terminated string that contains the name of the document file associated with the object.

This property is read/write.

## Syntax


```VB
Property FileName As String
```



## Property value

A **String** that specifies or receives the fully qualified path and name of the file to transmit.

## Remarks

The **FileName** property is required to send a fax transmission using a call to the [**Send**](-mfax-ifaxdoc-send-vb.md) method. For more information, see [Transmitting Faxes](-mfax-transmitting-faxes.md).

The **get\_FileName** method allocates the memory required for the buffer pointed to by the *pVal* parameter. The client application must call the [SysFreeString](8f230ee3-5f6e-4cb9-a910-9c90b754dcd3) function to deallocate the resources associated with this parameter. For more information, see [Freeing Fax Resources](-mfax-freeing-fax-resources.md).

## Requirements



|                                     |                                                                                       |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 2000 Professional \[desktop apps only\]<br/>                            |
| Minimum supported server<br/> | Windows 2000 Server \[desktop apps only\]<br/>                                  |
| Header<br/>                   | <dl> <dt>Faxcom.h</dt> </dl>   |
| DLL<br/>                      | <dl> <dt>Faxcom.dll</dt> </dl> |



## See also

<dl> <dt>

[**FaxDoc**](-mfax-faxdoc-object-visual-basic-.md)
</dt> <dt>

[Fax Service Client API for Windows 2000](-mfax-fax-service-client-api-for-windows-2000.md)
</dt> <dt>

[Fax Service Client API Interfaces](-mfax-fax-service-client-api-interfaces.md)
</dt> <dt>

[**IFaxDoc**](-mfax-ifaxdoc.md)
</dt> <dt>

[SysFreeString](8f230ee3-5f6e-4cb9-a910-9c90b754dcd3)
</dt> </dl>

 

 



