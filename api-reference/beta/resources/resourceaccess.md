---
title: resourceAccess リソースの種類
description: OAuth 2.0 のためのアクセス許可のスコープまたはアプリケーションを必要とするアプリケーションの役割を指定します。 RequiredResourceAccess 型の**resourceAccess**プロパティは、 **ResourceAccess**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: f5389915897c3aab8b8277a45b54042bc861b290
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862336"
---
# <a name="resourceaccess-resource-type"></a>resourceAccess リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

OAuth 2.0 のためのアクセス許可のスコープまたはアプリケーションを必要とするアプリケーションの役割を指定します。 [RequiredResourceAccess](requiredresourceaccess.md)型の**resourceAccess**プロパティは、 **ResourceAccess**のコレクションです。


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resourceAccess"
}-->

```json
{
  "id": "guid",
  "type": "string"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|ID|Guid|リソースのアプリケーションを公開する[oAuth2Permission](oauth2permission.md)または[エンティティ](approle.md)のインスタンスの 1 つの一意の識別子です。|
|type|String|[OAuth2Permission](oauth2permission.md)または[エンティティ](approle.md)の**id**プロパティを参照するかどうかを指定します。 使用可能な値は、「スコープ」または「ロール」です。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
