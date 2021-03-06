---
title: 互操作性 - C# 编程指南
ms.custom: seodec18
ms.date: 07/20/2015
helpviewer_keywords:
- COM interop
- interoperability
- platform invoke, accessing APIs with C#
- C# language, interoperability
ms.assetid: 238bb95a-e962-4026-bbd5-197055bdb8ee
ms.openlocfilehash: b568bdc149123b490f3b058afc668aabcf558d55
ms.sourcegitcommit: c7a7e1468bf0fa7f7065de951d60dfc8d5ba89f5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/14/2019
ms.locfileid: "65585465"
---
# <a name="interoperability-c-programming-guide"></a>互操作性（C# 编程指南）
借助互操作性，可以保留和利用对非托管代码的现有投资工作。 在公共语言运行时 (CLR) 控制下运行的代码称为*托管代码*，不在 CLR 控制下运行的代码称为*非托管代码*。 例如，COM、COM+、C++ 组件、ActiveX 组件和 Microsoft Windows API 都是非托管代码。  
  
 使用 .NET Framework，可以通过平台调用服务、<xref:System.Runtime.InteropServices> 命名空间、C++ 互操作性和 COM 互操作性（COM 互操作），实现与非托管代码的互操作性。  
  
## <a name="in-this-section"></a>本节内容  
 [互操作性概述](../../../csharp/programming-guide/interop/interoperability-overview.md)  
 介绍了实现 C# 托管代码和非托管代码的互操作性的方法。  
  
 [如何：通过使用 Visual C# 功能访问 Office 互操作对象](../../../csharp/programming-guide/interop/how-to-access-office-onterop-objects.md)  
 介绍了 Visual C# 为了推动 Office 编程而引入的功能 。  
  
 [如何：在 COM 互操作编程中使用已编制索引的属性](../../../csharp/programming-guide/interop/how-to-use-indexed-properties-in-com-interop-rogramming.md)  
 介绍了如何使用已编入索引的属性来访问包含参数的 COM 属性。  
  
 [如何：使用平台调用播放波形文件](../../../csharp/programming-guide/interop/how-to-use-platform-invoke-to-play-a-wave-file.md)  
 介绍了如何使用平台调用服务在 Windows 操作系统中播放 .wav 声音文件。  
  
 [演练：Office 编程](../../../csharp/programming-guide/interop/walkthrough-office-programming.md)  
 展示了如何创建 Excel 工作簿和包含指向此工作簿的链接的 Word 文档。  
  
 [COM 类示例](../../../csharp/programming-guide/interop/example-com-class.md)  
 展示了如何将 C# 类公开为 COM 对象。  
  
## <a name="c-language-specification"></a>C# 语言规范  

有关详细信息，请参阅 [C# 语言规范](../../language-reference/language-specification/index.md)中的[基本概念](~/_csharplang/spec/unsafe-code.md)。 该语言规范是 C# 语法和用法的权威资料。
  
## <a name="see-also"></a>请参阅

- <xref:System.Runtime.InteropServices.Marshal.ReleaseComObject%2A?displayProperty=nameWithType>
- [C# 编程指南](../../../csharp/programming-guide/index.md)
- [与非托管代码交互操作](../../../../docs/framework/interop/index.md)
- [演练：Office 编程](../../../csharp/programming-guide/interop/walkthrough-office-programming.md)
