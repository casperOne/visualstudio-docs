---
title: "CvReleaseProvider Function | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-debug"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "cvmarkers/CvReleaseProvider"
helpviewer_keywords: 
  - "CvReleaseProvider method"
ms.assetid: 8d74379e-295d-452b-bd5f-0769df387d4f
caps.latest.revision: 8
author: "mikejo5000"
ms.author: "mikejo"
manager: "ghogen"
---
# CvReleaseProvider Function
[!INCLUDE[vs2017banner](../includes/vs2017banner.md)]

The latest version of this topic can be found at [CvReleaseProvider Function](https://docs.microsoft.com/visualstudio/profiling/cvreleaseprovider-function).  
  
Releases marker provider. Releasing the marker provider will not affect previously created marker series of this provider. Marker series have to be release separately by CvReleaseMarkerSeries call. Failure to release provider causes a memory leak.  
  
## Syntax  
  
```  
HRESULT CvReleaseProvider(  
   _In_ PCV_PROVIDER pProvider  
);  
```  
  
#### Parameters  
 `pProvider`  
 Provider context. Cannot be NULL.  
  
## Return Value  
 S_OK when provider is successfully released or error code in case there were any errors. Use SUCCEEDED/FAILED macros to check for error condition.  
  
## Requirements  
 **Header:** cvmarkers.h  
  
## See Also  
 [C++ Library Reference](../profiling/cpp-library-reference.md)



