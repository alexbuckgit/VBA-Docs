---
title: Dialog.Creator property (Excel)
keywords: vbaxl10.chm255074
f1_keywords:
- vbaxl10.chm255074
api_name:
- Excel.Dialog.Creator
ms.assetid: d912fae1-0b08-ff00-ad84-eab8e8e88340
ms.date: 04/25/2019
ms.localizationpriority: medium
---


# Dialog.Creator property (Excel)

Returns a 32-bit integer that indicates the application in which this object was created. Read-only **Long**.


## Syntax

_expression_.**Creator**

_expression_ A variable that represents a **[Dialog](Excel.Dialog.md)** object.


## Remarks

If the object was created in Microsoft Excel, this property returns the string XCEL, which is equivalent to the hexadecimal number 5843454C. The **Creator** property is designed to be used in Microsoft Excel for the Macintosh, where each application has a four-character creator code. For example, Microsoft Excel has the creator code XCEL.



[!include[Support and feedback](~/includes/feedback-boilerplate.md)]