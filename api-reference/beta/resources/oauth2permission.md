---
title: oAuth2Permission リソースの種類
description: OAuth 2.0 委任されたアクセス許可スコープを表します。 指定した OAuth 2.0 委任されたアクセス許可スコープは、リソースアプリケーションを呼び出すときに (application オブジェクトの**Requiredresourceaccess**コレクションを通じて) クライアントアプリケーションによって要求されることがあります。 ServicePrincipal エンティティおよび application エンティティの**approles**プロパティは、 **oAuth2Permission**のコレクションです。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 16dfa93d13127d585cd5b56a56987bb22ab39d8f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009574"
---
# <a name="oauth2permission-resource-type"></a>oAuth2Permission リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

OAuth 2.0 委任されたアクセス許可スコープを表します。 指定した OAuth 2.0 委任されたアクセス許可スコープは、リソースアプリケーションを呼び出すときに ( [application](application.md)オブジェクトの**requiredresourceaccess**コレクションを通じて) クライアントアプリケーションによって要求されることがあります。 [Serviceprincipal](serviceprincipal.md)エンティティおよび[Application](application.md)エンティティの**Approles**プロパティは、 **oAuth2Permission**のコレクションです。


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2Permission"
}-->

```json
{
  "adminConsentDescription": "string",
  "adminConsentDisplayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "type": "string",
  "userConsentDescription": "string",
  "userConsentDisplayName": "string",
  "value": "string"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|Admincon/説明|String|管理者の同意とアプリの割り当てエクスペリエンスに表示されるアクセス許可ヘルプテキスト。|
|Admincon/表示 Displayname|String|管理者の同意とアプリの割り当てエクスペリエンスに表示されるアクセス許可の表示名。|
|id|Guid|Oauth2Permissions コレクション内の一意のスコープアクセス許可識別子。|
|isEnabled|Boolean|アクセス許可を作成または更新する場合は、このプロパティを**true**に設定する必要があります (これは既定値です)。 権限を削除するには、最初にこのプロパティを**false**に設定する必要があります。  その時点で、以降の呼び出しでは、アクセス許可が削除されることがあります。|
|type|String|この範囲のアクセス許可をエンドユーザーが同意することができるかどうか、または会社の管理者が同意する必要があるテナント全体のアクセス許可であるかどうかを指定します。  可能な値は、"User" または "Admin" です。|
|Usercondescription の説明|String|エンドユーザーの同意画面に表示されるアクセス許可ヘルプテキスト。|
|Usercon使い方 Displayname|String|エンドユーザーの同意画面に表示されるアクセス許可の表示名。|
|value|文字列型 (String)|OAuth 2.0 アクセストークンで想定されるリソースアプリケーションのスコープ要求の値。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
