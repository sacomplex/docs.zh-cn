---
title: ICoreClrDebugTarget::FreeMemory 方法
ms.date: 03/30/2017
api_name:
- ICoreDebugTarget.FreeMemory
api_location:
- mscordbi_macx86.dll
api_type:
- COM
f1_keywords:
- ICoreClrDebugTarget::FreeMemory
helpviewer_keywords:
- remote debugging API [Silverlight]
- FreeMemory method, ICoreClrDebugTarget interface [Silverlight debugging]
- ICorClrDebugTarget::FreeMemory method [Silverlight debugging]
- Silverlight, remote debugging
ms.assetid: 98f2a0db-a6ec-4f9b-861d-f82485237d08
topic_type:
- apiref
author: rpetrusha
ms.author: ronpet
ms.openlocfilehash: ec156ca7590a2ec637cb59e022fc2dd1a71226e0
ms.sourcegitcommit: 9b552addadfb57fab0b9e7852ed4f1f1b8a42f8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "61993569"
---
# <a name="icoreclrdebugtargetfreememory-method"></a>ICoreClrDebugTarget::FreeMemory 方法
释放分配的内存[icoreclrdebugtarget:: Enumprocesses](../../../../docs/framework/unmanaged-api/debugging/icoreclrdebugtarget-enumprocesses-method.md)并[icoreclrdebugtarget:: Enumruntimes](../../../../docs/framework/unmanaged-api/debugging/icoreclrdebugtarget-enumruntimes-method.md)方法。  
  
## <a name="syntax"></a>语法  
  
```  
void FreeMemory (  
     [in] void*pMemory);  
```  
  
## <a name="parameters"></a>参数  
 `pMemory`  
 [in]指向通过以下任一方法返回的数组的指针[icoreclrdebugtarget:: Enumprocesses](../../../../docs/framework/unmanaged-api/debugging/icoreclrdebugtarget-enumprocesses-method.md)或[icoreclrdebugtarget:: Enumruntimes](../../../../docs/framework/unmanaged-api/debugging/icoreclrdebugtarget-enumruntimes-method.md)方法。  
  
## <a name="requirements"></a>要求  
 **平台：** 请参阅[系统需求](../../../../docs/framework/get-started/system-requirements.md)。  
  
 **标头：** CoreClrRemoteDebuggingInterfaces.h  
  
 **库：** mscordbi_macx86.dll  
  
 **.NET framework 版本：** 3.5 SP1  
  
## <a name="see-also"></a>请参阅

- [ICoreClrDebugTarget 接口](../../../../docs/framework/unmanaged-api/debugging/icoreclrdebugtarget-interface.md)
