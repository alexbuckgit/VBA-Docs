---
title: Application.DDEPoke method (Excel)
keywords: vbaxl10.chm132091
f1_keywords:
- vbaxl10.chm132091
api_name:
- Excel.Application.DDEPoke
ms.assetid: 5d00e0da-e041-7a9e-3b55-f5edd3f2a4a0
ms.date: 04/04/2019
ms.localizationpriority: medium
---


# Application.DDEPoke method (Excel)

Sends data to an application.


## Syntax

_expression_.**DDEPoke** (_Channel_, _Item_, _Data_)

_expression_ A variable that represents an **[Application](Excel.Application(object).md)** object.


## Parameters

|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
| _Channel_|Required| **Long**|The channel number returned by the **[DDEInitiate](Excel.Application.DDEInitiate.md)** method.|
| _Item_|Required| **Variant**|The item to which the data is to be sent.|
| _Data_|Required| **Variant**|The data to be sent to the application.|

## Remarks

An error occurs if the method call doesn't succeed.


## Example

This example opens a channel to Word, opens the Word document Sales.doc, and then inserts the contents of cell A1 (on Sheet1) at the beginning of the document.

```vb
channelNumber = Application.DDEInitiate( _ 
 app:="WinWord", _ 
 topic:="C:\WINWORD\SALES.DOC") 
Set rangeToPoke = Worksheets("Sheet1").Range("A1") 
Application.DDEPoke channelNumber, "\StartOfDoc", rangeToPoke 
Application.DDETerminate channelNumber
```




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]