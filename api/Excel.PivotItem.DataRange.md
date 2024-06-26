---
title: PivotItem.DataRange property (Excel)
keywords: vbaxl10.chm246075
f1_keywords:
- vbaxl10.chm246075
api_name:
- Excel.PivotItem.DataRange
ms.assetid: 6946f4eb-60ef-0d7a-394a-cd7904967a02
ms.date: 05/07/2019
ms.localizationpriority: medium
---


# PivotItem.DataRange property (Excel)

Returns a **[Range](Excel.Range(object).md)** object as shown in the following table. Read-only.


## Syntax

_expression_.**DataRange**

_expression_ A variable that represents a **[PivotItem](Excel.PivotItem.md)** object.


## Remarks

|Object|Data range|
|:-----|:-----|
|Data field|Data contained in the field|
|Row, column, or page field|Items in the field|
|Item|Data qualified by the item|

## Example

This example selects the PivotTable items in the field named REGION.

```vb
Set pvtTable = Worksheets("Sheet1").Range("A3").PivotTable 
Worksheets("Sheet1").Activate 
pvtTable.PivotFields("REGION").DataRange.Select
```



[!include[Support and feedback](~/includes/feedback-boilerplate.md)]