---
title: api リソースの種類
description: Web API アプリケーションの設定を指定します。
localization_priority: Normal
ms.openlocfilehash: 9d9259911464feb545b97a9eb8585723a9c3e20e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535692"
---
# <a name="api-resource-type"></a>api リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Web API アプリケーションの設定を指定します。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|requestedAccessTokenVersion|Int32| 現在の API リソースに対して承認されたアクセストークンのバージョンを指定します。 可能な値は1または2です。  |
|oauth2PermissionScopes|[permissionscope](permissionscope.md)コレクション| web API (リソース) アプリケーションがクライアントアプリケーションに公開する OAuth 2.0 アクセス許可スコープのコレクション。 これらのアクセス許可スコープは、同意時にクライアントアプリケーションに付与されることがあります。 |

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.api"
}-->

```json
{
  "requestedAccessTokenVersion": 1,
  "oauth2PermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "api resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/api.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
