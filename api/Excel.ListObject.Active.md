---
title: ListObject.Active property (Excel)
keywords: vbaxl10.chm734081
f1_keywords:
- vbaxl10.chm734081
api_name:
- Excel.ListObject.Active
ms.assetid: abe995da-6471-e611-ee04-d24f8518327c
ms.date: 04/30/2019
ms.localizationpriority: medium
---


# ListObject.Active property (Excel)

Returns a **Boolean** value indicating whether a **ListObject** object on a worksheet is active—that is, whether the active cell is inside the range of the **ListObject** object. Read-only **Boolean**.


## Syntax

_expression_.**Active**

_expression_ A variable that represents a **[ListObject](Excel.ListObject.md)** object.


## Remarks

Because there is no **Activate** method for the **ListObject** object, you can activate a **ListObject** object only by activating a cell range within the list.


## Example

The following example activates the list in the default **ListObject** object in the first worksheet of the active workbook. Invoking the **[Activate](excel.range.activate.md)** method of the **Range** object without cell parameters activates the entire range for the list.


```vb
Function MakeListActive() As Boolean 
 Dim wrksht As Worksheet 
 Dim objList As ListObject 
 
 Set wrksht = ActiveWorkbook.Worksheets("Sheet1") 
 Set objList = wrksht.ListObjects(1) 
 objList.Range.Activate 
 
 MakeListActive = objList.Active 
End Function
```




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]