---
title: IVMGuestOS ComputerName property
description: The computer name of the guest operating system running in the virtual machine.
ms.assetid: 'b35fa1a1-e105-43e6-9a2f-a5c7e71772cf'
keywords: ["ComputerName property Virtual PC", "ComputerName property Virtual PC , IVMGuestOS interface", "IVMGuestOS interface Virtual PC , ComputerName property"]
topic_type:
- apiref
api_name:
- IVMGuestOS.ComputerName
- IVMGuestOS.get_ComputerName
api_location:
- VPCCOMInterfaces.h
api_type:
- COM
---

# IVMGuestOS::ComputerName property

\[Windows Virtual PC is no longer available for use as of Windows�8. Instead, use the [Hyper-V WMI provider (V2)](https://msdn.microsoft.com/library/windows/desktop/hh850319).\]

Retrieves the computer name of the guest operating system running in the virtual machine (VM).

This property is read-only.

## Syntax


```C++
HRESULT get_ComputerName(
  [out, retval]�BSTR *guestComputerName
);
```



## Property value

The computer name of the guest operating system.

## Error codes



| Name/value                                                                                                                                                                       | Meaning                                                         |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------|
| <dl> <dt>S\_OK</dt> <dt>0</dt> </dl>                                          | The operation was successful.<br/>                        |
| <dl> <dt>E\_INVALIDARG</dt> <dt>0x80000003</dt> </dl>                         | The parameter is not valid or not specified.<br/>         |
| <dl> <dt>VM\_E\_VM\_NOT\_RUNNING</dt> <dt>0xA0040206</dt> </dl>               | The VM is not running.<br/>                               |
| <dl> <dt>VM\_E\_ADDITIONS\_FEATURE\_NOT\_AVAIL</dt> <dt>0xA0040505</dt> </dl> | Integration components are not installed in this VM.<br/> |
| <dl> <dt>DISP\_E\_EXCEPTION</dt> <dt>0x80020009</dt> </dl>                    | An unexpected error has occurred.<br/>                    |



## Requirements



|                                     |                                                                                               |
|-------------------------------------|-----------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�7 \[desktop apps only\]<br/>                                                    |
| Minimum supported server<br/> | None supported<br/>                                                                     |
| End of client support<br/>    | Windows�7<br/>                                                                          |
| Product<br/>                  | Windows Virtual PC<br/>                                                                 |
| Header<br/>                   | <dl> <dt>VPCCOMInterfaces.h</dt> </dl> |
| IID<br/>                      | IID\_IVMGuestOS is defined as 99fea0db-4880-499a-b6d8-73dff9bc91be<br/>                 |



## See also

<dl> <dt>

[**IVMGuestOS**](ivmguestos.md)
</dt> </dl>

�

�




