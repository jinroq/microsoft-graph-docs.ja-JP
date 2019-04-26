---
title: permissionscope リソースの種類
description: OAuth 2.0 委任されたアクセス許可スコープを表します。 指定した OAuth 2.0 委任されたアクセス許可スコープは、リソースアプリケーションを呼び出すときに (Application オブジェクトの**requiredresourceaccess**コレクションを通じて) クライアントアプリケーションによって要求されることがあります。 serviceprincipal エンティティおよび Application エンティティの**oauth2Permissions**プロパティは、 **OAuth2Permission**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: 00629a6e123ef19290d3c1bd4797e4bab3ce95c0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568181"
---
# <a name="permissionscope-resource-type"></a>permissionscope リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

OAuth 2.0 委任されたアクセス許可スコープを表します。 指定した OAuth 2.0 委任されたアクセス許可スコープは、リソースアプリケーションを呼び出すときに ( [Application](application.md)オブジェクトの**requiredresourceaccess**コレクションを通じて) クライアントアプリケーションによって要求されることがあります。 [serviceprincipal](serviceprincipal.md)エンティティおよび[Application](application.md)エンティティの**oauth2Permissions**プロパティは、 **OAuth2Permission**のコレクションです。

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
  "suppressions": [
    "Error: /api-reference/beta/resources/permissionscope.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
