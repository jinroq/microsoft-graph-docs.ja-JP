---
title: teamstabconfiguration リソースの種類 (オープンタイプ)
description: タブの内容を決定する設定。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9873d9e03fec5d7751270b963015aed9eeb0ab48
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456982"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a>teamstabconfiguration リソースの種類 (オープンタイプ)

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[タブ](teamstab.md)の内容を決定する設定。タブが対話的に構成されている場合、この情報はタブプロバイダーアプリケーションによって設定されます。
次のプロパティに加えて、一部のタブプロバイダーアプリケーションは、追加のカスタムプロパティを指定します。

## <a name="properties"></a>プロパティ

|プロパティ|型|説明|
|-|-|-|
|  entityId   |   string |  タブプロバイダによってホストされているエンティティの識別子。     |
|  contentUrl |   string |  Teams でのタブのコンテンツのレンダリングに使用される Url。 必須です。    |
|  removeUrl  |   string |  teams クライアントを使用してタブを削除したときに teams クライアントによって呼び出される Url。     |
|  websiteUrl |   string |  Teams の外部にタブのコンテンツを表示するための Url。     |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTabConfiguration"
}-->

```json
{
   "entityId": "string",
   "contentUrl": "string (HTTPS Url)",
   "websiteUrl": "string (HTTPS Url)",
   "removeUrl": "string (HTTPS Url)"  
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsTabConfiguration complex type (Open Type)",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamstabconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
