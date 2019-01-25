---
title: api リソースの種類
description: Web API アプリケーションの設定を指定します。
localization_priority: Normal
ms.openlocfilehash: 9d9259911464feb545b97a9eb8585723a9c3e20e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521447"
---
# <a name="api-resource-type"></a>api リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Web API アプリケーションの設定を指定します。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|requestedAccessTokenVersion|Int32| API の現在のリソースに許可されたアクセス トークンのバージョンを指定します。 使用可能な値は、1 または 2 です。  |
|oauth2PermissionScopes|[permissionScope](permissionscope.md)コレクション| Web アプリケーションの API (リソース) をクライアント アプリケーションに公開する OAuth 2.0 のアクセス許可のスコープのコレクション。 同意の中には、クライアント アプリケーションにこれらのアクセス許可のスコープを付与する可能性があります。 |

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
