---
title: permissionscope リソースの種類
description: OAuth 2.0 委任されたアクセス許可スコープを表します。 指定した OAuth 2.0 委任されたアクセス許可スコープは、リソースアプリケーションを呼び出すときに (Application オブジェクトの**requiredresourceaccess**コレクションを通じて) クライアントアプリケーションによって要求されることがあります。 serviceprincipal エンティティおよび Application エンティティの**oauth2Permissions**プロパティは、 **OAuth2Permission**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: 6f45d2eb0645991eb55db8ef3338e3b6fcf300a7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344995"
---
# <a name="permissionscope-resource-type"></a>permissionscope リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

OAuth 2.0 委任されたアクセス許可スコープを表します。 指定した OAuth 2.0 委任されたアクセス許可スコープは、リソースアプリケーションを呼び出すときに ( [application](application.md)オブジェクトの**requiredresourceaccess**コレクションを通じて) クライアントアプリケーションによって要求されることがあります。 [serviceprincipal](serviceprincipal.md)エンティティおよび[Application](application.md)エンティティの**oauth2Permissions**プロパティは、 **OAuth2Permission**のコレクションです。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|admincon/説明|String| 管理者の同意とアプリの割り当てエクスペリエンスに表示されるアクセス許可ヘルプテキスト。 |
|admincon/表示 displayname|String| 管理者の同意とアプリの割り当てエクスペリエンスに表示されるアクセス許可の表示名。 |
|id|Guid| oauth2Permissions コレクション内の一意のスコープアクセス許可識別子。 |
|isEnabled|Boolean| アクセス許可を作成または更新する場合は、このプロパティを**true**に設定する必要があります (これは既定値です)。 権限を削除するには、最初にこのプロパティを**false**に設定する必要があります。 その時点で、以降の呼び出しでは、アクセス許可が削除されることがあります。 |
|戻す|String| 内部使用用。 |
|type|String| この範囲のアクセス許可をエンドユーザーが同意することができるかどうか、または会社の管理者が同意する必要があるテナント全体のアクセス許可であるかどうかを指定します。 使用可能な値は、*ユーザー*または*管理者*です。 |
|usercondescription の説明|String| エンドユーザーの同意に表示されるアクセス許可ヘルプテキスト。 |
|usercon使い方 displayname|String| エンドユーザーの同意に表示されるアクセス許可の表示名。 |
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
