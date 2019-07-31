---
title: permissionScope リソースの種類
description: OAuth 2.0 委任されたアクセス許可スコープを表します。 指定した OAuth 2.0 委任されたアクセス許可スコープは、リソースアプリケーションを呼び出すときに (Application オブジェクトの**Requiredresourceaccess**コレクションを通じて) クライアントアプリケーションによって要求されることがあります。 ServicePrincipal エンティティおよび Application エンティティの**oauth2Permissions**プロパティは、 **OAuth2Permission**のコレクションです。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 59770460b8fbc3c0a8946eeed94adfbe027f20cc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966168"
---
# <a name="permissionscope-resource-type"></a>permissionScope リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

OAuth 2.0 委任されたアクセス許可スコープを表します。 指定した OAuth 2.0 委任されたアクセス許可スコープは、リソースアプリケーションを呼び出すときに ( [application](application.md)オブジェクトの**requiredresourceaccess**コレクションを通じて) クライアントアプリケーションによって要求されることがあります。 [Serviceprincipal](serviceprincipal.md)エンティティおよび[Application](application.md)エンティティの**oauth2Permissions**プロパティは、 **OAuth2Permission**のコレクションです。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|Admincon/説明|String| 管理者の同意とアプリの割り当てエクスペリエンスに表示されるアクセス許可ヘルプテキスト。 |
|Admincon/表示 Displayname|String| 管理者の同意とアプリの割り当てエクスペリエンスに表示されるアクセス許可の表示名。 |
|id|Guid| Oauth2Permissions コレクション内の一意のスコープアクセス許可識別子。 |
|isEnabled|Boolean| アクセス許可を作成または更新する場合は、このプロパティを**true**に設定する必要があります (これは既定値です)。 権限を削除するには、最初にこのプロパティを**false**に設定する必要があります。 その時点で、以降の呼び出しでは、アクセス許可が削除されることがあります。 |
|戻す|String| 内部使用用。 |
|type|String| この範囲のアクセス許可をエンドユーザーが同意することができるかどうか、または会社の管理者が同意する必要があるテナント全体のアクセス許可であるかどうかを指定します。 使用可能な値は、*ユーザー*または*管理者*です。 |
|Usercondescription の説明|String| エンドユーザーの同意に表示されるアクセス許可ヘルプテキスト。 |
|Usercon使い方 Displayname|String| エンドユーザーの同意に表示されるアクセス許可の表示名。 |
|value|文字列型 (String)| OAuth 2.0 アクセストークンで想定されるリソースアプリケーションのスコープ要求の値。 |

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
<!--
{
  "type": "#page.annotation",
  "description": "permissionScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
