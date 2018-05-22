---
title: BG\_JOB\_PRIORITY enumeration
description: The BG\_JOB\_PRIORITY enumeration defines the constant values that specify the priority level of a job.
ms.assetid: 'AF1F1F6D-473A-49E5-B24D-644A70DF304C'
keywords: ["BG_JOB_PRIORITY enumeration", "BG_JOB_PRIORITY enumeration"]
topic_type:
- apiref
api_name:
- BG_JOB_PRIORITY
api_location:
- deliveryoptimization.h
api_type:
- HeaderDef
---

# BG\_JOB\_PRIORITY enumeration

The **BG\_JOB\_PRIORITY** enumeration defines the constant values that specify the priority level of a job.

## Syntax


```C++
typedef enum  { 
  BG_JOB_PRIORITY_FOREGROUND,
  BG_JOB_PRIORITY_HIGH,
  BG_JOB_PRIORITY_NORMAL,
  BG_JOB_PRIORITY_LOW
} BG_JOB_PRIORITY;
```



## Constants

<dl> <dt>

<span id="BG_JOB_PRIORITY_FOREGROUND"></span><span id="bg_job_priority_foreground"></span>**BG\_JOB\_PRIORITY\_FOREGROUND**
</dt> <dd>

Transfers the job in the foreground. Foreground transfers compete for network bandwidth with other applications, which can impede the user's network experience. This is the highest priority level.

</dd> <dt>

<span id="BG_JOB_PRIORITY_HIGH"></span><span id="bg_job_priority_high"></span>**BG\_JOB\_PRIORITY\_HIGH**
</dt> <dd>

Transfers the job in the background. Background transfers use a small percentage of network bandwidth.

</dd> <dt>

<span id="BG_JOB_PRIORITY_NORMAL"></span><span id="bg_job_priority_normal"></span>**BG\_JOB\_PRIORITY\_NORMAL**
</dt> <dd>

DO behavior is same for all non foreground job. See comments in BG\_JOB\_PRIORITY\_HIGH for details.

</dd> <dt>

<span id="BG_JOB_PRIORITY_LOW"></span><span id="bg_job_priority_low"></span>**BG\_JOB\_PRIORITY\_LOW**
</dt> <dd>

DO behavior is same for all non foreground job. See comments in BG\_JOB\_PRIORITY\_HIGH for details.

</dd> </dl>

## Remarks

Multiple foreground and background transfers can take place simultaneously.

## Requirements



|                                     |                                                                                                   |
|-------------------------------------|---------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�10, version 1709 \[desktop apps only\]<br/>                                         |
| Minimum supported server<br/> | Windows Server, version 1709 \[desktop apps only\]<br/>                                     |
| Header<br/>                   | <dl> <dt>Deliveryoptimization.h</dt> </dl> |



## See also

<dl> <dt>

[**IBackgroundCopyJob::GetPriority**](ibackgroundcopyjob-getpriority.md)
</dt> <dt>

[**IBackgroundCopyJob::SetPriority**](ibackgroundcopyjob-setpriority.md)
</dt> </dl>

�

�




