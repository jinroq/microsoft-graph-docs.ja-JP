---
title: 'ユーザー: translateExchangeIds'
description: Outlook 関連リソースの ID の形式を変換します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1015ae12f5ecfd63b29efe38f7172321b06386ec
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33961230"
---
# <a name="user-translateexchangeids"></a>ユーザー: translateExchangeIds

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Outlook 関連リソースの ID の形式を変換します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類 | アクセス許可 (特権の小さいものから大きいものへ) |
|:----------------|:--------------------------------------------|
| 委任 (職場または学校のアカウント) | ユーザー. ReadBasic、user. 読み取り、ユーザー. 読み取り/書き込み。すべてのユーザー。すべてのユーザーに対して。 |
| 委任 (個人用 Microsoft アカウント) | ユーザー. ReadBasic、User. 読み取り/書き込み |
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
| inputIds | String collection | 変換する識別子のコレクション。 コレクション内のすべての識別子のソース ID の種類は同じである必要があり、同じメールボックス内のアイテムである必要があります。 このコレクションの最大サイズは1000文字列です。 |
| sourceIdType | exchangeIdFormat | `InputIds`パラメーターの識別子の id の種類。 |
| targetIdType | exchangeIdFormat | 変換先となる要求された ID の種類。 |

### <a name="exchangeidformat-values"></a>exchangeIdFormat の値

| 値 | 説明 |
|:-------|:------------|
| entryId | MAPI クライアントによって使用されるバイナリエントリ ID 形式。 |
| ewsId | Exchange Web サービスクライアントによって使用される ID 形式。 |
| immutableEntryId | バイナリ MAPI 互換の不変 ID 形式。 |
| restId | Microsoft Graph で使用される既定の ID 形式。 |
| restImmutableEntryId | Microsoft Graph で使用される不変の ID 形式。 |

バイナリ形式 (`entryId`および`immutableEntryId`) は、URL セーフな base64 でエンコードされます。 URL-safeness は、バイナリデータの base64 エンコードを次のように変更することによって実装されます。

- 置換`+`後`-`
- 置換`/`後`_`
- 末尾のパディング文字を削除`=`する ()
- 文字列の末尾に、元の文字の数 (`0`、 `1`、、または`2`) を示す整数を追加します。

## <a name="response"></a>応答

成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[convertIdResult](../resources/convertidresult.md)コレクションを返します。

## <a name="example"></a>例

次の例は、複数の識別子を標準の REST API 形式 (`restId`) から不変形式 (`restImmutableEntryId`) に変換する方法を示しています。

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

応答の例を次に示します。
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
#### <a name="sdk-sample-code"></a>SDK サンプル コード
# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_translateexchangeids-Javascript-snippets.md)]

# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/user_translateexchangeids-Cs-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-translateexchangeids.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-translateexchangeids.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
