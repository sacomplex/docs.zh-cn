---
title: 运行时信息 ETW 事件
ms.date: 03/30/2017
helpviewer_keywords:
- runtime information events [.NET Framework]
- ETW, runtime information events
ms.assetid: 68b4edbc-7f3b-45f6-ab75-4fd066d6af9a
author: mairaw
ms.author: mairaw
ms.openlocfilehash: af27ddaa69d34976929f40055bc2cc668f877e87
ms.sourcegitcommit: 9b552addadfb57fab0b9e7852ed4f1f1b8a42f8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "61949209"
---
# <a name="runtime-information-etw-events"></a>运行时信息 ETW 事件
这些 ETW 事件记录有关运行时的信息，包括 SKU、版本号、激活运行时的方式、启动运行时所使用的命令行参数、GUID（如果适用）以及其他相关信息。 如果多个运行时在一个进程内执行，这些事件 (ClrInstanceID) 提供的信息可帮助消除不同运行时的歧义。  
  
 下表显示了两个运行时信息事件。 这两个事件可在任意关键字或掩码下引发。 （有关详细信息，请参阅 [CLR ETW Keywords and Levels](../../../docs/framework/performance/clr-etw-keywords-and-levels.md)。）  
  
|Event|事件 ID|提供程序|描述|  
|-----------|--------------|--------------|-----------------|  
|`RuntimeInformationEvent`|187|CLRRuntime|加载运行时时引发。|  
|`RuntimeInformationDCStart`|187|CLRRundown|枚举加载的运行时。|  
  
 下表显示了事件数据。  
  
|字段名|数据类型|描述|  
|----------------|---------------|-----------------|  
|ClrInstanceID|win:UInt16|CLR 或 CoreCLR 的实例的唯一 ID。|  
|Sku|win:UInt16|1 – 桌面 CLR。<br /><br /> 2 – CoreCLR。|  
|BclVersion – 主版本|win:UInt16|mscorlib.dll 的主版本。|  
|BclVersion – 次版本|win:UInt16|mscorlib.dll 的次版本号。|  
|BclVersion – 生成号|win:UInt16|mscorlib.dll 的生成号。|  
|BclVersion – QFE|win:UInt16|mscorlib.dll 的修补程序版本号。|  
|VMVersion – 主版本|win:UInt16|clr.dll 或 coreclr.dll 的版本（取决于 SKU）。|  
|VMVersion – 次版本|win:UInt16|clr.dll 或 coreclr.dll 的次版本（取决于 SKU）。|  
|VMVersion – 生成号|win:UInt16|clr.dll 或 coreclr.dll 的生成号。|  
|VMVersion – QFE|win:UInt16|clr.dll 或 coreclr.dll 的修补程序版本号。|  
|StartupFlags|win:UInt32|在 mscoree.h 中定义的启动标志。|  
|StartupMode|win:UInt8|0x01 - 托管可执行文件。<br /><br /> 0x02 - 托管 CLR。<br /><br /> 0x04 - C++ 托管互操作。<br /><br /> 0x08 - 已激活 COM。<br /><br /> 0x10 - 其他。|  
|CommandLine|win:UnicodeString|仅在 StartupMode=0x01 时为非 NULL。|  
|ComObjectGUID|win:GUID|仅在 StartupMode=0x08 时为非 NULL。|  
|RuntimeDLLPath|win:UnicodeString|已加载到进程的 CLR.dll 文件的路径。|  
  
## <a name="see-also"></a>请参阅

- [CLR ETW 事件](../../../docs/framework/performance/clr-etw-events.md)
