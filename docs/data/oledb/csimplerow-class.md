---
title: "CSimpleRow Class | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.technology: ["cpp-data"]
ms.topic: "reference"
f1_keywords: ["CSimpleRow", "ATL::CSimpleRow", "ATL.CSimpleRow"]
dev_langs: ["C++"]
helpviewer_keywords: ["CSimpleRow class"]
ms.assetid: 06d9621d-60cc-4508-8b0c-528d1b1a809b
author: "mikeblome"
ms.author: "mblome"
ms.workload: ["cplusplus", "data-storage"]
---
# CSimpleRow Class
Provides a default implementation for the row handle, which is used in the [IRowsetImpl](../../data/oledb/irowsetimpl-class.md) class.  
  
## Syntax

```cpp
class CSimpleRow  
```  
  
## Members  
  
### Methods  
  
|||  
|-|-|  
|[AddRefRow](../../data/oledb/csimplerow-addrefrow.md)|Adds a reference count to an existing row handle.|  
|[Compare](../../data/oledb/csimplerow-compare.md)|Compares two rows to see if they refer to the same row instance.|  
|[CSimpleRow](../../data/oledb/csimplerow-csimplerow.md)|The constructor.|  
|[ReleaseRow](../../data/oledb/csimplerow-releaserow.md)|Releases rows.|  
  
### Data Members  
  
|||  
|-|-|  
|[m_dwRef](../../data/oledb/csimplerow-m-dwref.md)|Reference count to an existing row handle.|  
|[m_iRowset](../../data/oledb/csimplerow-m-irowset.md)|An index to the rowset representing the cursor.|  
  
## Remarks  
 A row handle is logically a unique tag for a result row. `IRowsetImpl` creates a new `CSimpleRow` for every row requested in [IRowsetImpl::GetNextRows](../../data/oledb/irowsetimpl-getnextrows.md). `CSimpleRow` can also be replaced with your own implementation of the row handle, as it is a default template argument to `IRowsetImpl`. The only requirement to replacing this class is to have the replacement class provide a constructor that accepts a single parameter of type **LONG**.  
  
## Requirements  
 **Header:** atldb.h  
  
## See Also  
 [OLE DB Provider Templates](../../data/oledb/ole-db-provider-templates-cpp.md)   
 [OLE DB Provider Template Architecture](../../data/oledb/ole-db-provider-template-architecture.md)   
 [IRowsetImpl Class](../../data/oledb/irowsetimpl-class.md)