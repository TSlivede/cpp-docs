---
title: "CDataSource::GetProperties | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.technology: ["cpp-data"]
ms.topic: "reference"
f1_keywords: ["CDataSource::GetProperties", "ATL.CDataSource.GetProperties", "CDataSource.GetProperties", "ATL::CDataSource::GetProperties", "GetProperties"]
dev_langs: ["C++"]
helpviewer_keywords: ["GetProperties method"]
ms.assetid: ffaecc17-9fe7-449e-94d6-43d31ad06cfc
author: "mikeblome"
ms.author: "mblome"
ms.workload: ["cplusplus", "data-storage"]
---
# CDataSource::GetProperties
Returns the property information requested for the connected data source object.  
  
## Syntax  
  
```
HRESULT GetProperties(ULONG ulPropIDSets,   
   constDBPROPIDSET* pPropIDSet,   
   ULONG* pulPropertySets,   
   DBPROPSET** ppPropsets) const throw();  
```  
  
#### Parameters  
 See [IDBProperties::GetProperties](https://msdn.microsoft.com/en-us/library/ms714344.aspx) in the *OLE DB Programmer's Reference* in the Windows SDK.  
  
## Return Value  
 A standard `HRESULT`.  
  
## Remarks  
 To get a single property, use [GetProperty](../../data/oledb/cdatasource-getproperty.md).  
  
## Requirements  
 **Header:** atldbcli.h  
  
## See Also  
 [CDataSource Class](../../data/oledb/cdatasource-class.md)