---
title: Name.CategoryLocal property (Excel)
keywords: vbaxl10.chm490076
f1_keywords:
- vbaxl10.chm490076
api_name:
- Excel.Name.CategoryLocal
ms.assetid: 5f80e0a4-e12d-a85d-69a1-979652f62ac3
ms.date: 05/01/2019
ms.localizationpriority: medium
---


# Name.CategoryLocal property (Excel)

Returns or sets the category for the specified name, in the language of the user, if the name refers to a custom function or command. Read/write **String**.


## Syntax

_expression_.**CategoryLocal**

_expression_ A variable that represents a **[Name](Excel.Name.md)** object.


## Example

This example displays, in the language of the user, the function category of either a custom function or a command created on a Microsoft Excel 4.0 macro sheet. The example assumes that the custom function name or command name is the only name in the workbook.

```vb
With ActiveWorkbook.Names(1) 
 If .MacroType <> xlNone Then 
 MsgBox "The category for this name is " & .CategoryLocal 
 Else 
 MsgBox "This name does not refer to" & _ 
 " a custom function or command." 
 End If 
End With
```




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]