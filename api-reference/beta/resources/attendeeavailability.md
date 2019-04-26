---
title: attendeeAvailability リソースの種類
description: 出席者の空き時間。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 95896808f1a58eb77cafb8003ca5c7848d50bc08
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339022"
---
# <a name="attendeeavailability-resource-type"></a>attendeeAvailability リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

出席者の空き時間。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailability"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeBase"},
  "availability": "String"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|attendee|[attendeeBase](attendeebase.md)|出席者の電子メールアドレスと種類。個人またはリソースのいずれかを指定します。また、必要かどうかは、ユーザーの場合はオプションです。|
|availability|freeBusyStatus| 出席者の空き時間の状態。使用可能な値: `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
