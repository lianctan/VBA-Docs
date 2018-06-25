---
title: Pages.CalloutRelationshipAdded Event (Visio)
keywords: vis_sdr.chm11062075
f1_keywords:
- vis_sdr.chm11062075
ms.prod: visio
api_name:
- Visio.Pages.CalloutRelationshipAdded
ms.assetid: 45f350ca-05ed-b775-d5da-b0d9c8a5c885
ms.date: 06/08/2017
---


# Pages.CalloutRelationshipAdded Event (Visio)

Occurs when a new callout relationship is added to a page.


## Syntax

Private Sub  _expression_ _'CalloutRelationshipAdded'( **_By Val ShapePair As RelatedShapePairEvent_** )

 _expression_ A variable that represents a '[Pages](Visio.Pages.md)' object.


### Parameters



|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
| _ShapePair_|Required| **[RelatedShapePairEvent](relatedshapepairVisio.Event.md)**|An object that represents the new callout shape-pair relationship.|

## Remarks

The  **RelatedShapePairEvent** object that this event returns contains two shapes: the container and the member, represented by the **[RelatedShapePairEvent.FromShapeID](Visio.RelatedShapePairEvent.FromShapeID.md)** and the **[RelatedShapePairEvent.ToShapeID](Visio.RelatedShapePairEvent.ToShapeID.md)** properties respectively.

If you are using Microsoft Visual Basic or Visual Basic for Applications (VBA), the syntax in this topic describes a common, efficient way to handle events.

If you want to create your own  **[Event](Visio.Event.md)** objects, use the **[EventList.Add](Visio.EventList.Add.md)** or **[EventList.AddAdvise](Visio.EventList.AddAdvise.md)** method. To create an **Event** object that runs an add-on, use the **EventList.Add** method. To create an **Event** object that receives notification, use the **EventList.AddAdvise** method. To find an event code for the event that you want to create, see[Event Codes](http://msdn.microsoft.com/library/de8f5c7a-421d-ebcf-22b6-4310a202ef64%28Office.15%29.aspx).

