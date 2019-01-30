---
title: Serviceprincipal を更新します。
description: Serviceprincipal オブジェクトのプロパティを更新します。
localization_priority: Normal
ms.openlocfilehash: a562bca03881923cfc21d32eadee2a7f7053fa9b
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641177"
---
# <a name="update-serviceprincipal"></a>Serviceprincipal を更新します。

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Serviceprincipal オブジェクトのプロパティを更新します。
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.AccessAsUser.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Application.ReadWrite.OwnedBy、Application.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:-----------|:------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|accountEnabled|Boolean|                サービス プリンシパルのアカウントが有効な場合は **true**。それ以外の場合は **false**。            |
|appDisplayName|String|関連付けられているアプリケーションによって公開される表示名。|
|appId|String|関連付けられたアプリケーションの一意の識別子 (その **appId** プロパティ)。|
|appRoleAssignmentRequired|Boolean|Azure AD からアプリケーションにユーザー トークンまたはアクセス トークンが発行される前に、ユーザーまたはグループに対する **appRoleAssignment** が必要かどうかを指定します。                            **メモ**: バージョン 1.5 が必要ですか、null を許容しません。            |
|appRoles|エンティティ|関連付けられているアプリケーションによって公開されるアプリケーション ロール。 詳細についてはアプリケーション エンティティ**のノート**で**appRoles**プロパティの定義を参照してください: バージョン 1.5 が必要ですか、null を許容しません。            |
|displayName|String|サービス プリンシパルの表示名。|
|errorUrl|String|            |
|HomePage|String|関連付けられたアプリケーションのホーム ページの URL です。|
|keyCredentials|keyCredential|サービス プリンシパルに関連付けられているキー資格情報のコレクションです。null 許容型ではありません。                            **注**: Null は許容されません。            |
|logoutUrl|String| Microsoft の承認サービスで、[フロント チャネル](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[バック チャネル](https://openid.net/specs/openid-connect-backchannel-1_0.html)または SAML ログアウト プロトコルを使ってユーザーのログアウトするのに使う URL を指定します。 |
|oauth2Permissions|oAuth2Permission|関連付けられているアプリケーションによって公開される OAuth 2.0 のアクセス許可。 さらに詳しい情報については、アプリケーション エンティティの **oauth2Permissions** プロパティの定義を参照してください。                            **メモ**: バージョン 1.5 が必要ですか、null を許容しません。            |
|passwordCredentials|passwordCredential|サービス プリンシパルに関連付けられているパスワード資格情報のコレクションです。null 許容型ではありません。                            **注**: Null は許容されません。            |
|preferredTokenSigningKeyThumbprint|String|内部使用専用に予約済みです。 このプロパティに書き込みしたり、依存したりしないでください。 将来のバージョンで削除される可能性があります。                            **メモ**: バージョン 1.5 以降が必要です。            |
|publisherName|String|関連付けられたアプリケーションが指定されているテナントの表示名。|
|replyUrls|String|関連付けられたアプリケーションにサインインするためにユーザー トークンが送信される URL、または関連付けられたアプリケーションに対して OAuth 2.0 認証コードとアクセス トークンが送信されるリダイレクト URI。                            **注**: Null は許容されません。            |
|samlMetadataUrl|String|            |
|servicePrincipalNames|String|関連するアプリケーションを識別する URI です。 詳細については、「[Azure Active Directory のアプリケーション オブジェクトとサービス プリンシパル オブジェクト](https://msdn.microsoft.com/library/azure/dn132633.aspx)」を参照してください。                            **メモ**: null を許容しない、 **any**演算子は、複数値を持つプロパティのフィルター式に必要な詳細については、[サポートされているクエリ、フィルター、およびページングのオプション](https://msdn.microsoft.com/library/azure/dn727074.aspx)を参照してください。            |
|tags|String|                                        **注**: Null は許容されません。            |

## <a name="response"></a>応答

かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の更新された[servicePrincipal](../resources/serviceprincipal.md)オブジェクトです。
## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}-->
```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/{id}
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```
##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceprincipal"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update serviceprincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
