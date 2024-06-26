---
title: LeaderLines property (Excel Graph)
keywords: vbagr10.chm5207592
f1_keywords:
- vbagr10.chm5207592
api_name:
- Excel.LeaderLines
ms.assetid: ddd9ab86-d135-73de-b888-3ba43c39ece8
ms.date: 04/11/2019
ms.localizationpriority: medium
---


# LeaderLines property (Excel Graph)

Returns a **LeaderLines** object that represents the leader lines for the specified series. Read-only.

## Syntax

_expression_.**LeaderLines**

_expression_ Required. An expression that returns a **[LeaderLines](excel.leaderlines-graph-object.md)** object.

## Example

This example adds data labels and blue leader lines to series one on the pie chart.

```vb
With myChart.SeriesCollection(1) 
 .HasDataLabels = True 
 .DataLabels.Position = xlLabelPositionBestFit 
 .HasLeaderLines = True 
 .LeaderLines.Border.ColorIndex = 5 
End With
```

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]