---
title: userIdentity リソースの種類
description: Azure AD 監査ログのコンテキストでは、これは監査アクティビティの開始または影響を受けたユーザー情報を表します。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0e72f5338f7281188b7023aed342dd34ee57595e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033503"
---
# <a name="useridentity-resource-type"></a>userIdentity リソースの種類

Azure AD 監査ログのコンテキストでは、これは監査アクティビティの開始または影響を受けたユーザー情報を表します。

## <a name="properties"></a>プロパティ

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| displayName | String | Id の表示名。 これは、常に有効であったり、最新ではない場合があることに注意してください。    |
| id          | 文字列 | ID の一意識別子。  |
| ipAddress   | String| ユーザーがアクティビティを実行するときに使用するクライアント IP アドレスを示します (監査ログのみ)。|
| userPrincipalName | String  | ユーザーの userPrincipalName 属性。 |

>**注:** 場合によっては、一意の識別子を使用できないことがあります。 その場合、ID の **displayName** プロパティが返されますが、**id** プロパティはリソースから失われます。

## <a name="json-representation"></a>JSON 表記

この型の JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
"displayName", "thumbnails"
  ],
  "@odata.type": "microsoft.graph.userIdentity"
}-->

```json
{
  "displayName": "string",
  "id": "string",
  "ipAddress": "string",
  "userPrincipalName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/useridentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
