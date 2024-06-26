---
title: Adjustments.Item property (Excel)
keywords: vbaxl10.chm103003
f1_keywords:
- vbaxl10.chm103003
api_name:
- Excel.Adjustments.Item
ms.assetid: b3f3a20c-3ef0-48be-411a-dfb08758684d
ms.date: 04/04/2019
ms.localizationpriority: medium
---


# Adjustments.Item property (Excel)

Returns or sets the adjustment value specified by the _Index_ argument. Read/write **Single**.


## Syntax

_expression_.**Item** (_Index_)

_expression_ A variable that represents an **[Adjustments](Excel.Adjustments.md)** object.


## Parameters

|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
| _Index_|Required| **[INT]**| **Long**. The index number of the adjustment.|

## Remarks

AutoShapes, connectors, and WordArt objects can have up to eight adjustments.

For linear adjustments, an adjustment value of 0.0 generally corresponds to the left or top edge of the shape, and a value of 1.0 generally corresponds to the right or bottom edge of the shape. However, adjustments can pass beyond shape boundaries for some shapes. 

For radial adjustments, an adjustment value of 1.0 corresponds to the width of the shape. 

For angular adjustments, the adjustment value is specified in degrees. The **Item** property applies only to shapes that have adjustments.




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]