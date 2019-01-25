---
title: アプリケーションを更新します。
description: アプリケーション オブジェクトのプロパティを更新します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 335281a0ac37ae3b966f731112223f019a67437d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525949"
---
# <a name="update-application"></a>アプリケーションを更新します。

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

アプリケーション オブジェクトのプロパティを更新します。
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
|allowPublicClient|ブール値| アプリケーションは、パブリック クライアントとして動作できるかどうかを指定します。 たとえば、モバイル デバイスで実行されているインストール済みのアプリケーションです。 既定値は *false* です。 |
|API|API| API アプリケーションの設定を指定します。 |
|appRoles|[エンティティ](../resources/approle.md)のコレクション|アプリケーションが宣言されているアプリケーション ロールのコレクションです。 これらのロールは、ユーザー、グループ、またはサービス ・ プリンシパルを指定できます。 null 許容ではありません。|
|applicationAliases|String コレクション| アプリケーションを識別する Uri。 詳細情報は、「[アプリケーションのオブジェクトおよびオブジェクトのサービス プリンシパル](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/)です。 複数値プロパティのフィルター式には *any* 演算子が必要です。 null 許容ではありません。 |
|createdDateTime|DateTimeOffset| 日付と時刻、アプリケーションが登録されています。 |
|deletedDateTime|DateTimeOffset| 日付と時刻、アプリケーションが削除されました。 |
|displayName|String|アプリケーションの表示名です。 |
|id|String|アプリケーションの一意の識別子です。 [directoryObject](../resources/directoryobject.md) から継承されます。 キー。 null 許容ではありません。 読み取り専用です。 |
|Info|[informationalUrl](../resources/informationalurl.md)| アプリケーションの基本的なプロファイル情報です。 | デスクトップやモバイル デバイスなどのインストールされているクライアントの設定を指定します。 |
|keyCredentials|[keyCredential](../resources/keycredential.md)コレクション|しないアプリケーションに関連付けられているキーの資格情報のコレクション null 許容型です。 |
|logo|Stream|アプリケーションのメインのロゴです。 null 許容ではありません。 |
|orgRestrictions|String コレクション| 組織 tenantIds をアプリケーションに制限されます。  コレクションが空の場合は、アプリケーションは、マルチ テナント型 (制限されていないです)。 コレクションには、tenantIds が含まれている、アプリケーションは、コレクション内の組織の tenantIds に制限されます。 他のテナントがアプリケーションが登録されている tenantId ではありませんを指定すると、アプリケーションの tenantId が間接的に含まれていることを意味します。 |
|passwordCredentials|[passwordCredential](../resources/passwordcredential.md)コレクション|アプリケーションに関連付けられているパスワード資格情報のコレクションです。 null 許容ではありません。|
|preAuthorizedApplications|[preAuthorizedApplication](../resources/preauthorizedapplication.md)コレクション| アプリケーションと暗黙的な同意を要求されたアクセス許可の一覧です。 管理者がアプリケーションに同意を提供する必要があります。 preAuthorizedApplications では、ユーザーが要求されたアクセス許可に同意するものは必要ありません。 PreAuthorizedApplications に記載されているアクセス許可では、ユーザーの同意は必要ありません。 ただし、preAuthorizedApplications に記載されていない追加の要求されたアクセス許可は、ユーザーの同意を必要とします。 |
|requiredResourceAccess|[requiredResourceAccess](../resources/requiredresourceaccess.md)コレクション|このアプリケーションへのアクセスと、OAuth アクセス許可のスコープおよび各リソースの下に必要なアプリケーション ロールのセットを必要とするリソースを指定します。 必要なリソースへのアクセスのこの前の構成では、同意の経験をドライブします。 null 許容ではありません。|
|タグの前に追加されるマークアップ|String コレクション| 分類し、アプリケーションの識別に使用できるカスタム文字列。 |
|web|Web| Web アプリケーションの設定を指定します。 |

## <a name="response"></a>応答

かどうかは成功すると、このメソッドが返されます、`204 No Content`応答コードは、戻り値も、応答の本体で、です。
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
    "Error: /api-reference/beta/api/application-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
