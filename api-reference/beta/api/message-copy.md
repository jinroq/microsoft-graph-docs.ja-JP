---
title: 'メッセージ: copy'
description: メッセージをフォルダーにコピーします。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a5dfd92c6478414c8890b6c411b5a9385a992198
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540593"
---
# <a name="message-copy"></a>メッセージ: copy

メッセージをフォルダーにコピーします。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類 | アクセス許可 (特権の小さいものから大きいものへ) |
|:----------------|:--------------------------------------------|
|委任 (職場または学校のアカウント) | Mail.ReadWrite    |
|委任 (個人用 Microsoft アカウント) | Mail.ReadWrite    |
|アプリケーション | Mail.ReadWrite |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a>要求ヘッダー

| ヘッダー | 値 |
|:-------|:------|
| Authorization | `Bearer {token}`. 必須。 |
| Content-Type | `application/json`. 必須です。 |

## <a name="request-body"></a>要求本文

要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター | 型 | 説明 |
|:----------|:-----|:------------|
|destinationId|String|宛先フォルダーの ID、または既知のフォルダー名。 サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。|

## <a name="response"></a>応答

成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[メッセージ](../resources/message.md)リソースを返します。

## <a name="example"></a>例

以下は、この API を呼び出す方法の例です。

##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "message_copy"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a>応答

以下は、応答の例です。

> **注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。 実際の呼び出しではすべてのプロパティが返されます。
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
  "bodyPreview": "bodyPreview-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
