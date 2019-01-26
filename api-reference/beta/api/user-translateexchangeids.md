---
title: 'ユーザー: translateExchangeIds'
description: 形式との間、Outlook に関連するリソースの識別子を変換します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3b09ae9bf6a1cbf1967a900770b07d8c9750ba21
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571290"
---
# <a name="user-translateexchangeids"></a>ユーザー: translateExchangeIds

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

形式との間、Outlook に関連するリソースの識別子を変換します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類 | アクセス許可 (特権の小さいものから大きいものへ) |
|:----------------|:--------------------------------------------|
| 委任 (職場または学校のアカウント) | User.ReadBasic、User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All |
| 委任 (個人用 Microsoft アカウント) | User.ReadBasic、User.Read、User.ReadWrite |
| アプリケーション | User.Read.All、User.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a>要求ヘッダー

| 名前 | 値 |
|:-----|:------|
| Authorization | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文

| パラメーター | 型 | 説明 |
|:----------|:-----|:------------|
| inputIds | Edm.String コレクション | 変換識別子のコレクションです。 コレクション内のすべての識別子は、同じソース ID の種類を持つ必要があり、同じメールボックス内のアイテムにする必要があります。 このコレクションの最大サイズは、1000 の文字列です。 |
| sourceIdType | exchangeIdFormat | ID の種類の識別子の`InputIds`のパラメーターです。 |
| targetIdType | exchangeIdFormat | 要求された ID の種類に変換します。 |

### <a name="exchangeidformat-values"></a>exchangeIdFormat 値

| 値 | 説明 |
|:-------|:------------|
| エントリ Id | MAPI クライアントによって使用されるバイナリのエントリ ID の形式です。 |
| ewsId | Exchange Web サービス クライアントによって使用される ID 形式です。 |
| immutableEntryId | バイナリ MAPI と互換性のある変更不可能な ID 形式です。 |
| restId | Microsoft Graph で使用される既定の ID 形式です。 |
| restImmutableEntryId | Microsoft Graph で使用される ID の変更不可能な形式です。 |

バイナリ フォーマット (`entryId`と`immutableEntryId`) は、base64 でエンコードされた URL セーフであります。 URL safeness は、base64 エンコードのバイナリ データの次のように変更することによって実装されます。

- 交換`+`で`-`
- 交換`/`で`_`
- 末尾の埋め込み文字を削除する (`=`)
- 示す数のスペース文字は元の文字列の末尾に整数値を追加する (`0`、 `1`、または`2`)

## <a name="response"></a>応答

かどうかは成功すると、このメソッドを返します`200 OK`応答コードおよび応答の本文に[convertIdResult](../resources/convertidresult.md)のコレクションです。

## <a name="example"></a>例

次の使用例は、REST API の通常の形式から、複数の識別子を変換する方法を示しています (`restId`) に残りの部分の変更不可能な形式 (`restImmutableEntryId`)。

### <a name="request"></a>要求

要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "user_translateexchangeids"
}-->

```http
POST https://graph.microsoft.com/beta/me/translateExchangeIds
Content-Type: application/json

{
  "inputIds" : [
    "{rest-formatted-id-1}",
    "{rest-formatted-id-2}"
  ],
  "sourceIdType": "restId",
  "targetIdType": "restImmutableEntryId"
}
```

### <a name="response"></a>応答

応答の例を次のとおりです。
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.convertIdResult",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/testexchangebeta/$metadata#Collection(microsoft.graph.convertIdResult)",
  "value": [
    {
      "sourceId": "{rest-formatted-id-1}",
      "targetId": "{rest-immutable-formatted-id-1}"
    },
    {
      "sourceId": "{rest-formatted-id-2}",
      "targetId": "{rest-immutable-formatted-id-2}"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-translateexchangeids.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
