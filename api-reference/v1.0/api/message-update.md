---
title: メッセージを更新する
description: メッセージ オブジェクトのプロパティを更新します。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: c3564d5f48cb3b3e12e18a07d605fcd3eba01291
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922544"
---
# <a name="update-message"></a>メッセージを更新する

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
| 名前       | 種類 | 説明|
|:-----------|:------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |
| Content-Type | string  | エンティティ本文内のデータの性質です。必須。 |
## <a name="request-body"></a>要求本文
要求本文で、更新する関連フィールドの値を指定します。 要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。 最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。 次のプロパティを更新することができます。

| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|bccRecipients|Recipient|メッセージの BCC 受信者。 |
|body|ItemBody|メッセージの本文。 更新可能な場合にのみ isDraft = true です。|
|categories|String コレクション|メッセージに関連付けられたカテゴリ。|
|ccRecipients|Recipient collection|メッセージの CC 受信者。 |
|from|Recipient|メッセージのメールボックス所有者と送信者。 使用される実際のメールボックスに対応する必要があります。|
|importance|String|メッセージの重要性。 可能な値: `Low`、 `Normal`、 `High`。|
|inferenceClassification | String | 推論の妥当性や重要度、または明示的なオーバーライドに基づいて、ユーザーに対するメッセージの分類です。 可能な値:`focused`または`other`。 |
|internetMessageId |String |[RFC2822](https://www.ietf.org/rfc/rfc2822.txt) によって指定された形式のメッセージ ID。 更新可能な場合にのみ isDraft = true です。|
|isDeliveryReceiptRequested|ブール値|メッセージの開封応答が要求されているかどうかを示します。|
|isRead|ブール値|メッセージが開封されたかどうかを示します。|
|isReadReceiptRequested|ブール値|メッセージの開封確認メッセージが要求されているかどうかを示します。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection| 複数値のコレクションでは、メッセージに対して定義されたプロパティを拡張します。 Null 許容型。|
|replyTo|Recipient collection|返信時に使用される電子メール アドレス。 更新可能な場合にのみ isDraft = true です。|
|sender|Recipient|メッセージを生成するために実際に使用されるアカウント。 [共有されているメールボックス](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)、または[委任](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926)としてメッセージを送信するメッセージを送信するときに更新します。 いずれの場合も、値は、使用される実際のメールボックスに対応する必要があります。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection| 単一値のコレクションでは、メッセージに対して定義されたプロパティを拡張します。 Null 許容型。|
|subject|String|メッセージの件名。 更新可能な場合にのみ isDraft = true です。|
|toRecipients|Recipient collection|宛先] の受信者のメッセージです。|

**メッセージ** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`PATCH` 操作を使用して、既存の**メッセージ** インスタンスで拡張機能のカスタム プロパティにあるアプリ固有のデータを追加、更新、または削除することができます。

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [message](../resources/message.md) オブジェクトを返します。
## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "update_message"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/{id}
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
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
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
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
