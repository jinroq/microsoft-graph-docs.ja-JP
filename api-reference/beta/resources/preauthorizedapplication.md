---
title: preauthorizedapplication リソースの種類
description: アプリケーションと、暗黙的同意の要求されたアクセス許可を表します。 管理者はアプリケーションに同意を得る必要があります。 preauthorizedapplications では、ユーザーが要求されたアクセス許可に同意する必要はありません。 preauthorizedapplications にリストされているアクセス許可は、ユーザーの同意を必要としません。 ただし、preauthorizedapplications に表示されていない追加の要求されたアクセス許可には、ユーザーの同意が必要です。
localization_priority: Normal
ms.openlocfilehash: f74ac0883c883bfbb2cb93c2da58e9fd8419dadd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344230"
---
# <a name="preauthorizedapplication-resource-type"></a>preauthorizedapplication リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

アプリケーションと、暗黙的同意の要求されたアクセス許可を表します。 管理者はアプリケーションに同意を得る必要があります。 preauthorizedapplications では、ユーザーが要求されたアクセス許可に同意する必要はありません。 preauthorizedapplications にリストされているアクセス許可は、ユーザーの同意を必要としません。 ただし、preauthorizedapplications に表示されていない追加の要求されたアクセス許可には、ユーザーの同意が必要です。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|appId|String| アプリケーションの一意の識別子です。 |
|permissionids|String collection| アプリケーションが必要とする[publishedpermissionscope](permissionscope.md)または[approle](approle.md)の一意の識別子。 |

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.preAuthorizedApplication"
}-->

```json
{
  "appId": "String",
  "permissionIds": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "preAuthorizedApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
