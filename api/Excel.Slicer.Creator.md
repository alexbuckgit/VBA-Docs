---
title: Slicer.Creator property (Excel)
keywords: vbaxl10.chm904074
f1_keywords:
- vbaxl10.chm904074
api_name:
- Excel.Slicer.Creator
ms.assetid: 82991e7e-5bf8-e508-398a-413707ac70b1
ms.date: 05/16/2019
ms.localizationpriority: medium
---


# Slicer.Creator property (Excel)

Returns a 32-bit integer that indicates the application in which this object was created. Read-only **Long**.


## Syntax

_expression_.**Creator**

_expression_ A variable that represents a **[Slicer](Excel.Slicer.md)** object.


## Remarks

If the object was created in Microsoft Excel, this property returns the string XCEL, which is equivalent to the hexadecimal number 5843454C. The **Creator** property is designed to be used in Microsoft Excel for the Macintosh, where each application has a four-character creator code. For example, Microsoft Excel has the creator code XCEL.




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]