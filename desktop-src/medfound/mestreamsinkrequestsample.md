﻿---
Description: 'Raised by a stream sink to request a new media sample from the pipeline.'
ms.assetid: '35020a15-942f-4dd0-9ca4-815affdacecf'
title: MEStreamSinkRequestSample event
---

# MEStreamSinkRequestSample event

Raised by a stream sink to request a new media sample from the pipeline. For each MEStreamSinkRequestSample event, the pipeline requests data from the next upstream component.

## Event values

Possible values retrieved from [**IMFMediaEvent::GetValue**](imfmediaevent-getvalue.md) include the following.



| VARTYPE              | Description                           |
|----------------------|---------------------------------------|
| VT\_EMPTY<br/> | No event data.<br/> <br/> |



## Requirements



|                                     |                                                                                                          |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista \[desktop apps only\]<br/>                                                           |
| Minimum supported server<br/> | Windows Server 2008 \[desktop apps only\]<br/>                                                     |
| Header<br/>                   | <dl> <dt>Mfobjects.h (include Mfidl.h)</dt> </dl> |



## See also

<dl> <dt>

[Media Foundation Events](media-foundation-events.md)
</dt> <dt>

[Media Sinks](media-sinks.md)
</dt> </dl>

 

 



