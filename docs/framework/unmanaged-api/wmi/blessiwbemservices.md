---
title: BlessIWbemServices 函数 （非托管 API 参考）
description: BlessIWbemServices 函数指示用户凭据是否允许访问 IWbemServices 类。
ms.date: 11/06/2017
api_name:
- BlessIWbemServices
api_location:
- WMINet_Utils.dll
api_type:
- DLLExport
f1_keywords:
- BlessIWbemServices
helpviewer_keywords:
- BlessIWbemServices function [.NET WMI and performance counters]
topic_type:
- Reference
author: rpetrusha
ms.author: ronpet
ms.openlocfilehash: eb83bc3c0c7724dbcd3133465d4e7ad3a9eea3a9
ms.sourcegitcommit: 8699383914c24a0df033393f55db3369db728a7b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/15/2019
ms.locfileid: "65636509"
---
# <a name="blessiwbemservices-function"></a>BlessIWbemServices 函数
指示用户凭据是否允许访问指定[IWbemServices](/windows/desktop/api/wbemcli/nn-wbemcli-iwbemservices)类。   
  
[!INCLUDE[internalonly-unmanaged](../../../../includes/internalonly-unmanaged.md)]
  
## <a name="syntax"></a>语法  
  
```  
HRESULT BlessIWbemServices (
   [in] IWbemServices* pIWbemServices,
   [in] BSTR strUser, 
   [in] BSTR strPassword, 
   [in] BSTR strAuthority, 
   [in] DWORD impLevel, 
   [in] DWORD authnLevel
);
```  

## <a name="parameters"></a>参数

`pIWbemServices`\
[in]一个指向[IWbemServices](/windows/desktop/api/wbemcli/nn-wbemcli-iwbemservices)权限是必需的对象。

`strUser`\
[in]用户名称。

`strPassword`\
[in]与关联的密码`strUser`。

`strAuthority`\
[in]用户的域名。 请参阅[ConnectServerWmi](connectserverwmi.md)函数的详细信息。

`impLevel`\
[in]模拟级别。

`authnLevel`\
[in]授权级别。

## <a name="return-value"></a>返回值

此函数返回以下值中定义*WinError.h*标头文件，也可以在定义它们为常量在代码中：

|返回的常量  |值  |描述  |
|---------|---------|---------|
| `E_INVALIDARG` | 0x80070057 | 一个或多个参数均无效。 |
| `E_POINTER` | 0x80004003 | `pIWbemServices` 为 `null`。 | 
| `E_FAIL` | 0x80000008 | 发生未知的错误。 |
| `E_OUTOFMEMORY` | 0x80000002 | 没有足够的内存是可用于执行该操作。 | 
| `S_OK` | 0 | 函数调用成功。 | 

## <a name="requirements"></a>要求  

 **平台：** 请参阅[系统需求](../../../../docs/framework/get-started/system-requirements.md)。  
  
 **标头：** WMINet_Utils.idl  
  
 **.NET Framework 版本：**[!INCLUDE[net_current_v472plus](../../../../includes/net-current-v472plus.md)]  
  
## <a name="see-also"></a>请参阅

- [WMI 和性能计数器 （非托管 API 参考）](index.md)
