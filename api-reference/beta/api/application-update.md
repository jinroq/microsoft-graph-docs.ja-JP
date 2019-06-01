---
title: アプリケーションを更新する
description: Application オブジェクトのプロパティを更新します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c5ab3871c1101c170deb500e516ff179dec6929f
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655174"
---
# <a name="update-application"></a>アプリケーションを更新する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Application オブジェクトのプロパティを更新します。
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。


|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) |  Directory.AccessAsUser.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Application.ReadWrite.OwnedBy、Application.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
PATCH /applications/{id}
```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:-----------|:------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。  |

## <a name="request-body"></a>要求本文
要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|allowPublicClient|Boolean| アプリケーションがパブリッククライアントとして動作するかどうかを指定します。 たとえば、モバイルデバイスで実行中のアプリケーションがインストールされている場合です。 既定値は *false* です。 |
|api|[apiApplication](../resources/apiapplication.md)| API アプリケーションの設定を指定します。 |
|appRoles|[appRole](../resources/approle.md) コレクション|アプリケーションで宣言できるアプリケーション ロールのコレクションです。 これらのロールは、ユーザー、グループ、サービス プリンシパルなどに割り当てることができます。 null 許容ではありません。|
|applicationAliases|String コレクション| アプリケーションを識別する URI です。 詳細については、「[Azure Active Directory のアプリケーション オブジェクトとサービス プリンシパル オブジェクト](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/)」を参照してください。 複数値プロパティのフィルター式には *any* 演算子が必要です。 null 許容ではありません。 |
|createdDateTime|DateTimeOffset| アプリケーションが登録された日付と時刻です。 |
|deletedDateTime|DateTimeOffset| アプリケーションが削除された日付と時刻です。 |
|displayName|String|アプリケーションの表示名。 |
|id|String|アプリケーションの一意の識別子です。 [directoryObject](../resources/directoryobject.md) から継承されます。 キー。 null 許容ではありません。 読み取り専用です。 |
|info|[informationalUrl](../resources/informationalurl.md)| アプリケーションの基本的なプロファイル情報です。 | デスクトップやモバイル デバイスなど、インストールされているクライアントの設定を指定します。 |
|keyCredentials|[keyCredential](../resources/keycredential.md) コレクション|アプリケーションに関連付けられているキー資格情報のコレクションです。null 許容型ではありません。 |
|logo|Stream|アプリケーションのメイン ロゴです。 null 許容ではありません。 |
|orgRestrictions|String コレクション| アプリケーションが制限されている組織の整理された Ds。  コレクションが空の場合、アプリケーションはマルチテナント (制限なし) です。 コレクションに保持されている Ds がある場合、アプリケーションはコレクション内の整理された Ds に制限されます。 アプリケーションが登録されている tenantId を指定せずに他のテナントを指定すると、アプリケーション自体の tenantId が間接的に含まれていることを意味します。 |
|passwordCredentials|[passwordCredential](../resources/passwordcredential.md) コレクション|アプリケーションに関連付けられているパスワード資格情報のコレクションです。 null 許容型ではありません。|
|preAuthorizedApplications|[Preauthorizedapplication](../resources/preauthorizedapplication.md)コレクション| アプリケーションおよび暗黙的同意の要求されたアクセス許可を一覧表示します。 管理者はアプリケーションに同意を得る必要があります。 preAuthorizedApplications では、ユーザーが要求されたアクセス許可に同意する必要はありません。 PreAuthorizedApplications にリストされているアクセス許可は、ユーザーの同意を必要としません。 ただし、preAuthorizedApplications に表示されていない追加の要求されたアクセス許可には、ユーザーの同意が必要です。 |
|requiredResourceAccess|[requiredResourceAccess](../resources/requiredresourceaccess.md) コレクション|このアプリケーションがアクセスする必要があるリソース、およびそのリソースで必要な OAuth アクセス許可の範囲とアプリケーション ロールのセットを指定します。 必要なリソースへのアクセスに対するこの事前構成によって、同意エクスペリエンスが促進されます。 null 許容型ではありません。|
|tags|String コレクション| アプリケーションを分類および識別するために使用できるカスタム文字列です。 |
|Web|[webApplication](../resources/webapplication.md)| Web アプリケーションの設定を指定します。 |

## <a name="response"></a>応答

成功した場合、このメソッド`204 No Content`は応答コードを返し、応答本文では何も返しません。
## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "update_application"
}-->
```http
PATCH https://graph.microsoft.com/beta/applications/{id}
Content-type: application/json
Content-length: 72

{
  "allowPublicClient": false,
  "displayName": "New display name"
}
```
##### <a name="response"></a>応答
注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a>SDK サンプル コード
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/update_application-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_application-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/application-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/application-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
