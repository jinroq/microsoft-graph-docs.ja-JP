---
title: webApplication リソースの種類
description: Web アプリケーションの設定を指定します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: e57744c3825a669a9008cd05d649be0ec51b71ac
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964152"
---
# <a name="webapplication-resource-type"></a>webApplication リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Web アプリケーションの設定を指定します。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------|:-----|:------------|
|implicitGrantSettings|[implicitGrantSettings](implicitgrantsettings.md)| この web アプリケーションが OAuth 2.0 暗黙的フローを使用してトークンを要求できるかどうかを指定します。|
|logoutUrl|String| Microsoft の承認サービスで、[フロント チャネル](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[バック チャネル](https://openid.net/specs/openid-connect-backchannel-1_0.html)または SAML ログアウト プロトコルを使ってユーザーのログアウトするのに使う URL を指定します。 |
|oauth2AllowImplicitFlow|Boolean| 現在は廃止されています。 使用しないでください。 | 
|redirectUris|文字列コレクション| サインインのためにユーザートークンが送信される Url、または OAuth 2.0 認証コードとアクセストークンがに送信されるリダイレクト Uri を指定します。 |

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.webApplication"
}-->

```json
{
  "implicitGrantSettings": {"@odata.type": "microsoft.graph.implicitGrantSettings"},
  "logoutUrl": "String",
  "oauth2AllowImplicitFlow": false,
  "redirectUris": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "webApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
