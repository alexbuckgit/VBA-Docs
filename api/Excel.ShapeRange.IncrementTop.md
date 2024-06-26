---
title: ShapeRange.IncrementTop method (Excel)
keywords: vbaxl10.chm640085
f1_keywords:
- vbaxl10.chm640085
api_name:
- Excel.ShapeRange.IncrementTop
ms.assetid: 39004de1-dbae-b57b-e2ea-edfc9b3aa9e3
ms.date: 05/14/2019
ms.localizationpriority: medium
---


# ShapeRange.IncrementTop method (Excel)

Moves the specified shape vertically by the specified number of [points](../language/glossary/vbe-glossary.md#point).


## Syntax

_expression_.**IncrementTop** (_Increment_)

_expression_ A variable that represents a **[ShapeRange](Excel.shaperange.md)** object.


## Parameters

|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
| _Increment_|Required| **Single**|Specifies how far the shape object is to be moved vertically, in points. A positive value moves the shape down; a negative value moves it up.|

## Example

This example duplicates shape one on _myDocument_, sets the fill for the duplicate, moves it 70 points to the right and 50 points up, and rotates it 30 degrees clockwise.

```vb
Set myDocument = Worksheets(1) 
With myDocument.Shapes(1).Duplicate 
 .Fill.PresetTextured msoTextureGranite 
 .IncrementLeft 70 
 .IncrementTop -50 
 .IncrementRotation 30 
End With
```



[!include[Support and feedback](~/includes/feedback-boilerplate.md)]