---
title: Application.Excel4MacroSheets property (Excel)
keywords: vbaxl10.chm132118
f1_keywords:
- vbaxl10.chm132118
api_name:
- Excel.Application.Excel4MacroSheets
ms.assetid: d1ee907a-302c-4bd5-5455-75c328f94268
ms.date: 04/04/2019
ms.localizationpriority: medium
---


# Application.Excel4MacroSheets property (Excel)

Returns a **[Sheets](Excel.Sheets.md)** collection that represents all the Microsoft Excel 4.0 macro sheets in the specified workbook. Read-only.


## Syntax

_expression_.**Excel4MacroSheets**

_expression_ A variable that represents an **[Application](Excel.Application(object).md)** object.


## Remarks

Using this property with the **Application** object or without an object qualifier is equivalent to using ActiveWorkbook.Excel4MacroSheets.


## Example

This example displays the number of Microsoft Excel 4.0 macro sheets in the active workbook.

```vb
MsgBox "There are " & ActiveWorkbook.Excel4MacroSheets.Count & _ 
 " Microsoft Excel 4.0 macro sheets in this workbook."
```




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]