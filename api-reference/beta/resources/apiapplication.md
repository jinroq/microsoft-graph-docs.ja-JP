---
title: api リソースの種類
description: Web API アプリケーションの設定を指定します。
localization_priority: Normal
ms.openlocfilehash: f26a568d05c85059e914b355d971755f19627cac
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348404"
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
  "@odata.type": "microsoft.graph.apiApplication"
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
  "suppressions": []
}
-->
