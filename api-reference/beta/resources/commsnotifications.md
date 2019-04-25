---
title: commsnotifications リソースの種類
description: 複数の通知を1つのバッチで送信するために通信サーバーによって使用される通知の一覧。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2d002b74bffe0911e2ba1fef4eed324b52ebcc49
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535517"
---
# <a name="commsnotifications-resource-type"></a>commsnotifications リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

複数の通知を1つのバッチで送信するために通信サーバーによって使用される通知の一覧。

## <a name="properties"></a>プロパティ

| プロパティ       | 型                                                 | 説明                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| value          | [commsnotification](commsnotification.md)コレクション | リソースの変更の通知。 |

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
