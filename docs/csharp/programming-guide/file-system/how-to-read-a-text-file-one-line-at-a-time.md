---
title: 如何：一次一行地读取文本文件 (Visual C#)
ms.date: 07/20/2015
helpviewer_keywords:
- ReadLine method [C#]
- reading text files, line by line
- text files [C#]
ms.assetid: d62e22c5-a13c-48db-af9b-f10c801b0cb1
ms.openlocfilehash: 4e6c4cfce1b5e97f70040b318eb68ee78ee4a953
ms.sourcegitcommit: 2701302a99cafbe0d86d53d540eb0fa7e9b46b36
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2019
ms.locfileid: "64595391"
---
# <a name="how-to-read-a-text-file-one-line-at-a-time-visual-c"></a>如何：一次一行地读取文本文件 (Visual C#)
此示例使用 `StreamReader` 类的 `ReadLine` 方法，一次一行地将文本文件内容读入字符串。 每个文本行都存储到字符串 `line` 中并显示在屏幕上。  
  
## <a name="example"></a>示例  
  
```csharp
int counter = 0;  
string line;  
  
// Read the file and display it line by line.  
System.IO.StreamReader file =   
    new System.IO.StreamReader(@"c:\test.txt");  
while((line = file.ReadLine()) != null)  
{  
    System.Console.WriteLine(line);  
    counter++;  
}  
  
file.Close();  
System.Console.WriteLine("There were {0} lines.", counter);  
// Suspend the screen.  
System.Console.ReadLine();  
```  
  
## <a name="compiling-the-code"></a>编译代码  
 复制代码，并将其粘贴到控制台应用程序的 `Main` 方法中。  
  
 将 `"c:\test.txt"` 替换为实际文件名。  
  
## <a name="robust-programming"></a>可靠编程  
 以下情况可能会导致异常：  
  
- 文件可能不存在。  
  
## <a name="net-framework-security"></a>.NET Framework 安全性  
 不要根据文件的名称来判断文件的内容。 例如，文件 `myFile.cs` 可能不是 C# 源文件。  
  
## <a name="see-also"></a>请参阅

- <xref:System.IO?displayProperty=nameWithType>
- [C# 编程指南](../../../csharp/programming-guide/index.md)
- [文件系统和注册表（C# 编程指南）](../../../csharp/programming-guide/file-system/index.md)
