---
title: "IDebugBinder3::GetMemoryObject | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-sdk"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "IDebugBinder3::GetMemoryObject"
helpviewer_keywords: 
  - "IDebugBinder3::GetMemoryObject method"
ms.assetid: 71d959c7-45df-485f-b0ee-f1c0439d54fb
caps.latest.revision: 7
author: "gregvanl"
ms.author: "gregvanl"
manager: ghogen
ms.workload: 
  - "vssdk"
---
# IDebugBinder3::GetMemoryObject
This method retrieves a memory object that represents the memory that this object is bound to.  
  
## Syntax  
  
```cpp  
HRESULT GetMemoryObject(  
   IDebugField*   pField,  
   UINT64         uConstant,  
   IDebugObject** ppObject  
);  
```  
  
```csharp  
int GetMemoryObject(  
   IDebugField      pField,  
   long             uConstant,  
   out IDebugObject ppObject  
);  
```  
  
#### Parameters  
 `pField`  
 [in] Specifies which field to get the memory object for.  
  
 `uConstant`  
 [in] Represents a memory address or value for a constant value.  
  
 `ppObject`  
 [out] An [IDebugObject](../../../extensibility/debugger/reference/idebugobject.md) representing the memory that this object is bound to.  
  
## Return Value  
 If successful, returns `S_OK`; otherwise, returns an error code.  
  
## See Also  
 [IDebugBinder3](../../../extensibility/debugger/reference/idebugbinder3.md)   
 [IDebugField](../../../extensibility/debugger/reference/idebugfield.md)   
 [IDebugObject](../../../extensibility/debugger/reference/idebugobject.md)