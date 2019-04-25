---
title: teamguestsettings リソースの種類
description: ゲストがチームでチャネルを作成、更新、削除できるかどうかを構成する設定。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: cb6e83093945a96784bfb91a76bc343a8c13d0ac
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548454"
---
# <a name="teamguestsettings-resource-type"></a>teamguestsettings リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ゲストが[チーム](team.md)内でチャネルを作成、更新、または削除できるかどうかを構成するための設定。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|allowCreateUpdateChannels|ブール値|true に設定すると、ゲストはチャネルを追加および更新できるようになります。|
|allowDeleteChannels|ブール値|true に設定されている場合、ゲストはチャネルを削除できます。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamGuestSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamguestsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
