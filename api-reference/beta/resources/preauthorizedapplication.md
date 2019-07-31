---
title: preAuthorizedApplication リソースの種類
description: アプリケーションと、暗黙的同意の要求されたアクセス許可を表します。 管理者はアプリケーションに同意を得る必要があります。 preAuthorizedApplications では、ユーザーが要求されたアクセス許可に同意する必要はありません。 PreAuthorizedApplications にリストされているアクセス許可は、ユーザーの同意を必要としません。 ただし、preAuthorizedApplications に表示されていない追加の要求されたアクセス許可には、ユーザーの同意が必要です。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7adaf4fe960b762b12f6b2cc8607e64c9813712e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965818"
---
# <a name="preauthorizedapplication-resource-type"></a>preAuthorizedApplication リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

アプリケーションと、暗黙的同意の要求されたアクセス許可を表します。 管理者はアプリケーションに同意を得る必要があります。 preAuthorizedApplications では、ユーザーが要求されたアクセス許可に同意する必要はありません。 PreAuthorizedApplications にリストされているアクセス許可は、ユーザーの同意を必要としません。 ただし、preAuthorizedApplications に表示されていない追加の要求されたアクセス許可には、ユーザーの同意が必要です。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|appId|String| アプリケーションの一意の識別子です。 |
|permissionIds|文字列コレクション| アプリケーションが必要とする[Publishedpermissionscope](permissionscope.md)または[approle](approle.md)の一意の識別子。 |

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
