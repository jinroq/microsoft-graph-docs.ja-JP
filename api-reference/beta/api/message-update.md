---
title: メッセージを更新する
description: メッセージ オブジェクトのプロパティを更新します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: ac75c8fe517a7e3c13316f2d733ab2b35dece1fa
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879366"
---
# <a name="update-message"></a>メッセージを更新する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

メッセージ オブジェクトのプロパティを更新します。
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Mail.ReadWrite    |
|委任 (個人用 Microsoft アカウント) | Mail.ReadWrite    |
|アプリケーション | Mail.ReadWrite |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:-----------|:------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |
| Content-Type | string  | エンティティ本文内のデータの性質です。必須。 |
## <a name="request-body"></a>要求本文
要求本文で、更新する関連フィールドの値を指定します。 要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。 最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。 次のプロパティを更新できます。

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|bccRecipients|受信者|メッセージの BCC 受信者。 |
|body|ItemBody|メッセージの本文。 isDraft = true の場合にのみ更新可能です。|
|categories|String collection|メッセージに関連付けられたカテゴリ。|
|ccRecipients|受信者コレクション|メッセージの CC 受信者。 |
|flag|[followUpFlag](../resources/followupflag.md)|メッセージのステータス、開始日、期限、または完了日を示すフラグ値。|
|from|受信者|メッセージのメールボックス所有者と送信者。 実際に使用されているメールボックスに対応している必要があります。 |
|importance|String|メッセージの重要度です。可能な値は、`Low`、`Normal`、`High` です。|
|inferenceClassification | String | 推定される関連性や重要性、または明示的なオーバーライドに基づく、ユーザーのメッセージの分類です。使用可能な値: `focused` または `other`。 |
|internetMessageId |String |[RFC2822](https://www.ietf.org/rfc/rfc2822.txt) によって指定された形式のメッセージ ID。 isDraft = true の場合にのみ更新可能です。|
|isDeliveryReceiptRequested|Boolean|メッセージの開封応答が要求されているかどうかを示します。|
|isRead|Boolean|メッセージが開封されたかどうかを示します。|
|isReadReceiptRequested|Boolean|メッセージの開封確認メッセージが要求されているかどうかを示します。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) コレクション| メッセージに対して定義された、複数値の拡張プロパティのコレクション。 Null 許容型です。|
|replyTo|受信者コレクション|返信時に使用される電子メール アドレス。 isDraft = true の場合にのみ更新可能です。|
|sender|受信者|メッセージを生成するために実際に使用されるアカウント。 [共有メールボックス](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)からメッセージを送信するとき、またはメッセージを [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926) として送信するときに、更新可能です。 いずれの場合でも、この値は、実際に使用されているメールボックスに対応している必要があります。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) コレクション| メッセージに対して定義された、単一値の拡張プロパティのコレクションです。 Null 許容型です。|
|subject|String|メッセージの件名。 isDraft = true の場合にのみ更新可能です。|
|toRecipients|受信者コレクション|メッセージの宛先受信者。 |

**メッセージ** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`PATCH` 操作を使用して、既存の**メッセージ** インスタンスで拡張機能のカスタム プロパティにあるアプリ固有のデータを追加、更新、または削除することができます。

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [message](../resources/message.md) オブジェクトを返します。
## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_message"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "inferenceClassification": "other"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value",
  "inferenceClassification": "other"
}
```

## <a name="see-also"></a>関連項目

- [拡張機能を使用してカスタム データをリソースに追加する](/graph/extensibility-overview)
- [オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)](/graph/extensibility-open-users)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
