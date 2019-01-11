---
title: permissionScope リソースの種類
description: OAuth 2.0 を表しますは、アクセス許可のスコープを委任します。 (Application オブジェクトの**requiredResourceAccess**コレクション) をクライアント アプリケーションで、委任されたアクセス許可のスコープを要求することが指定された OAuth 2.0 リソース アプリケーションを呼び出すときにします。 ServicePrincipal エンティティおよびアプリケーション エンティティの**oauth2Permissions**プロパティは、 **OAuth2Permission**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: a294316f5c6255d0873ce0dbe809c33dad89ae08
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818152"
---
# <a name="permissionscope-resource-type"></a>permissionScope リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

OAuth 2.0 を表しますは、アクセス許可のスコープを委任します。 ( [Application](application.md)オブジェクトの**requiredResourceAccess**コレクション) をクライアント アプリケーションで、委任されたアクセス許可のスコープを要求することが指定された OAuth 2.0 リソース アプリケーションを呼び出すときにします。 [ServicePrincipal](serviceprincipal.md)エンティティおよび[アプリケーション](application.md)エンティティの**oauth2Permissions**プロパティは、 **OAuth2Permission**のコレクションです。

## <a name="properties"></a>プロパティ

| プロパティ | 種類 | 説明 |
|:---------------|:--------|:----------|
|adminConsentDescription|String| 管理者同意し、アプリケーションの割り当てのエクスペリエンスに表示されるアクセス許可のヘルプ テキストです。 |
|adminConsentDisplayName|String| 管理者同意し、アプリケーションの割り当ての経験で表示されるアクセス許可の名前を表示します。 |
|ID|Guid| Oauth2Permissions コレクション内の一意のスコープ権限識別子です。 |
|isEnabled|Boolean| を作成またはアクセス許可を更新するとき、このプロパティは**true** (既定値) に設定する必要があります。 アクセス許可を削除するには、このプロパティを**false**に設定最初する必要があります。 その時点で、後続の呼び出しでアクセス許可が削除されます。 |
|原点|String| 内部で使用します。 |
|type|String| 、エンドユーザーがこのスコープの権限に同意するかどうか、または企業の管理者によって、に同意する必要があります、テナント全体のアクセス許可があるかどうかを指定します。 使用可能な値は、*ユーザー*または*管理者*です。 |
|userConsentDescription|String| エンドユーザーの同意に表示されるアクセス許可のヘルプ テキストです。 |
|userConsentDisplayName|String| エンドユーザーの同意で表示されるアクセス許可の名前を表示します。 |
|value|文字列| スコープの値は、OAuth 2.0 のアクセス トークンにリソース アプリケーションが予想されることを要求します。 |

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.permissionScope"
}-->

```json
{
  "adminConsentDescription": "String",
  "adminConsentDisplayName": "String",
  "id": "Guid",
  "isEnabled": true,
  "origin": "String",
  "type": "String",
  "userConsentDescription": "String",
  "userConsentDisplayName": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "permissionScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
