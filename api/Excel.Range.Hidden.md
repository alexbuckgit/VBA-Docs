---
title: Range.Hidden property (Excel)
keywords: vbaxl10.chm144145
f1_keywords:
- vbaxl10.chm144145
api_name:
- Excel.Range.Hidden
ms.assetid: 7e785c38-a8ae-3810-a88a-0bfb7b74e2d6
ms.date: 05/11/2019
ms.localizationpriority: medium
---


# Range.Hidden property (Excel)

Returns or sets a **Variant** value that indicates if the rows or columns are hidden.


## Syntax

_expression_.**Hidden**

_expression_ A variable that represents a **[Range](excel.range(object).md)** object.


## Remarks

Set this property to **True** to hide a row or column. The specified range must span an entire column or row.

Don't confuse this property with the **[FormulaHidden](Excel.Range.FormulaHidden.md)** property.


## Example

This example hides column C on Sheet1.

```vb
Worksheets("Sheet1").Columns("C").Hidden = True
```



[!include[Support and feedback](~/includes/feedback-boilerplate.md)]
