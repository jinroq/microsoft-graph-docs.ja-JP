---
title: 組織を更新する
description: 現在認証されている組織のプロパティを更新します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 090be61f98ecd8f55a5e1a9edfe45bf7b39f23de
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526845"
---
# <a name="update-organization"></a>組織を更新する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

現在認証されている組織のプロパティを更新します。 この例では、 `organization` 、1 つのレコードの集合として定義されている要求の**ID**を指定する必要がありますので。  **ID**は、組織の**tenantId**とも呼ばれます。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類 | アクセス許可 (特権の小さいものから大きいものへ) |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.AccessAsUser.All |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}
```

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 型 | 説明|
|:-----------|:------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文

要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|marketingNotificationEmails|String コレクション|                                        **注**: Null は許容されません。            |
|privacyProfile|[privacyProfile](../resources/privacyprofile.md)|組織のプライバシー プロファイル (statementUrl と contactEmail を設定します)。            |
|securityComplianceNotificationMails|String collection||
|securityComplianceNotificationPhones|String コレクション||
|technicalNotificationMails|String コレクション|                                        **注**: Null は許容されません。            |

使用することが**組織**のリソースは、[拡張機能](/graph/extensibility-overview)をサポートするため、`PATCH`を追加、更新、または**組織**の既存のインスタンスで拡張機能のカスタム プロパティに独自のアプリケーション固有データを削除する操作です。

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/{id}
Content-type: application/json
Content-length: 411

{
  "marketingNotificationEmails" : ["marketing@contoso.com"],
  "privacyProfile" :
    {
      "contactEmail":"alice@contoso.com",
      "statementUrl":"https://contoso.com/privacyStatement"
    },
  "securityComplianceNotificationMails" : ["security@contoso.com"],
  "securityComplianceNotificationPhones" : ["(123) 456-7890"],
  "technicalNotificationMails" : ["tech@contoso.com"]
}
```

##### <a name="response"></a>応答

以下は、応答の例です。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a>関連項目

- [拡張機能を使用してカスタム データをリソースに追加する](/graph/extensibility-overview)
- [オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)](/graph/extensibility-open-users)

<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/organization-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
