---
title: commsNotifications リソースの種類
description: 通信サーバーによって 1 つのバッチで複数の通知を送信するための通知の一覧です。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2d002b74bffe0911e2ba1fef4eed324b52ebcc49
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520593"
---
# <a name="commsnotifications-resource-type"></a>commsNotifications リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通信サーバーによって 1 つのバッチで複数の通知を送信するための通知の一覧です。

## <a name="properties"></a>プロパティ

| プロパティ       | 型                                                 | 説明                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| value          | [commsNotification](commsnotification.md)コレクション | リソースに変更を通知します。 |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [ { "@odata.type": "#microsoft.graph.commsNotification" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "commsNotifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/commsnotifications.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
