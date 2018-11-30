---
title: resourceAccess リソースの種類
description: OAuth 2.0 のためのアクセス許可のスコープまたはアプリケーションを必要とするアプリケーションの役割を指定します。 RequiredResourceAccess 型の**resourceAccess**プロパティは、 **ResourceAccess**のコレクションです。
ms.openlocfilehash: 56e9b2b006d63d2a9abebc9e9585744b08438800
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071867"
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
| プロパティ     | 型   |説明|
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
