---
title: ModelMeasureNames.Application property (Excel)
keywords: vbaxl10.chm971073
f1_keywords:
- vbaxl10.chm971073
ms.assetid: c755709d-d0f0-ac56-8d57-39230fd92486
ms.date: 05/01/2019
ms.localizationpriority: medium
---


# ModelMeasureNames.Application property (Excel)

Returns an **[Application](Excel.Application(object).md)** object that represents the Microsoft Excel application. Read-only.


## Syntax

_expression_.**Application**

_expression_ A variable that represents a **[ModelMeasureNames](Excel.modelmeasurenames.md)** object.


## Property value

**APPLICATION**


## Example

This example displays a message about the application that created _myObject_.

```vb
Set myObject = ActiveWorkbook 
If myObject.Application.Value = "Microsoft Excel" Then 
 MsgBox "This is an Excel Application object." 
Else 
 MsgBox "This is not an Excel Application object." 
End If
```



[!include[Support and feedback](~/includes/feedback-boilerplate.md)]