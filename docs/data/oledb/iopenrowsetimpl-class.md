---
title: "IOpenRowsetImpl Class | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.technology: ["cpp-data"]
ms.topic: "reference"
f1_keywords: ["IOpenRowsetImpl"]
dev_langs: ["C++"]
helpviewer_keywords: ["IOpenRowsetImpl class"]
ms.assetid: d259cedc-1db4-41cf-bc9f-5030907ab486
author: "mikeblome"
ms.author: "mblome"
ms.workload: ["cplusplus", "data-storage"]
---
# IOpenRowsetImpl Class
Provides implementation for the `IOpenRowset` interface.  
  
## Syntax

```cpp
template <class SessionClass>  
class IOpenRowsetImpl : public IOpenRowset  
```  
  
#### Parameters  
 `SessionClass`  
 Your class, derived from `IOpenRowsetImpl`.  
  
## Members  
  
### Methods  
  
|||  
|-|-|  
|[CreateRowset](../../data/oledb/iopenrowsetimpl-createrowset.md)|Creates a rowset object. Not called directly by user.|  
|[OpenRowset](../../data/oledb/iopenrowsetimpl-openrowset.md)|Opens and returns a rowset that includes all rows from a single base table or index. (Not in ATLDB.H)|  
  
## Remarks  
 The [IOpenRowset](https://msdn.microsoft.com/en-us/library/ms716946.aspx) interface is mandatory for a session object. It opens and returns a rowset that includes all rows from a single base table or index.  
  
## Requirements  
 **Header:** atldb.h  
  
## See Also  
 [OLE DB Provider Templates](../../data/oledb/ole-db-provider-templates-cpp.md)   
 [OLE DB Provider Template Architecture](../../data/oledb/ole-db-provider-template-architecture.md)