---
title: "GetArrayElement (Azure Stream Analytics) | Microsoft Docs"
ms.custom: ""
ms.date: "2016-04-22"
ms.prod: "azure"
ms.reviewer: ""
ms.service: "stream-analytics"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "reference"
applies_to: 
  - "Azure"
ms.assetid: 21dd9ec1-6722-4175-98db-c4e5e2f7cd6d
caps.latest.revision: 7
author: "SnehaGunda"
ms.author: "sngun"
manager: "jhubbard"
---
# GetArrayElement (Azure Stream Analytics)
  Returns the array element at the specified index.  
  
 **Syntax**  
  
```  
GetArrayElement ( array_expression, bigint_expression )  
```  
  
## Arguments  
 **array_expression**  
  
 Is the array expression to be evaluated as a source array. array_expression can be a column of type Array or result of another function call.  
  
 **bigint_expression**  
  
 Is the bigint expression to be evaluated as array index  
  
### Return Types  
 Return type is determined by the array element type and can be any of the [supported types.](https://msdn.microsoft.com/en-us/library/azure/dn835065.aspx)  
  
### Examples  
  
```  
SELECT   
    GetArrayElement(arrayField, 0) AS firstElement  
FROM input  
  
```  
  
  