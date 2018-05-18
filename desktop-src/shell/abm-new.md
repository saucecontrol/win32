---
Description: 'Registers a new appbar and specifies the message identifier that the system should use to send it notification messages. An appbar should send this message before sending any other appbar messages.'
ms.assetid: '1da9db13-6fdc-44b3-9985-de32d572675a'
title: 'ABM\_NEW message'
---

# ABM\_NEW message

Registers a new appbar and specifies the message identifier that the system should use to send it notification messages. An appbar should send this message before sending any other appbar messages.


```C++
fRegistered = (BOOL) SHAppBarMessage(ABM_NEW, pabd); 
```



## Parameters

<dl> <dt>

*pabd* 
</dt> <dd>

A pointer to an [**APPBARDATA**](appbardata.md) structure that contains the new appbar's window handle and message identifier. You must specify the **cbSize**, **hWnd**, and **uCallbackMessage** members when sending this message; all other members are ignored.

</dd> </dl>

## Return value

Returns **TRUE** if successful, or **FALSE** if an error occurs or if the appbar is already registered.

## Requirements



|                                     |                                                                                       |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�XP \[desktop apps only\]<br/>                                           |
| Minimum supported server<br/> | Windows�2000 Server \[desktop apps only\]<br/>                                  |
| Header<br/>                   | <dl> <dt>Shellapi.h</dt> </dl> |



�

�



