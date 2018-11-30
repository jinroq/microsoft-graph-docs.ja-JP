---
title: 'グループ: validateProperties'
description: Office 365 のグループの表示名やメールのニックネームは、命名ポリシーに準拠している場合を検証します。 クライアントは、API を使用して場合は、表示名を確認または、Office 365 のグループ**を更新**する前に、メールのニックネームが無効です。 プロパティを検証グループを作成する前に、ディレクトリ オブジェクトの validateProperties 関数を使用します。
ms.openlocfilehash: d7f2767908e6cbf9116bec769a1abc32731e4758
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067279"
---
# <a name="group-validateproperties"></a>グループ: validateProperties

Office 365 のグループの表示名やメールのニックネームは、命名ポリシーに準拠している場合を検証します。 クライアントは、API を使用して場合は、表示名を確認または、Office 365 のグループ**を更新**する前に、メールのニックネームが無効です。 プロパティを検証グループを作成する前に、ディレクトリ オブジェクトの[validateProperties 関数](directoryobject-validateproperties.md)を使用します。

表示名とメールのニックネームのプロパティには、次の検証が実行されます。 
1. プリフィックスおよびサフィックスの名前付けポリシーを検証します。
2. 禁止された単語をカスタム ポリシーを検証します。

この API は、最初のエラーが発生しましたを返します。 1 つまたは複数のプロパティには、複数の検証が失敗した場合、最初の検証エラーのプロパティだけが返されます。 ただし、メールのニックネームと表示名の両方を検証し、検証エラーのコレクションが表示される場合は、プレフィックスとサフィックスの名前付けポリシーを検証しているだけです。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Group.Read.All、Group.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Group.Read.All、Group.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/<id>/validateProperties
```

## <a name="request-headers"></a>要求ヘッダー

| 名前           | 説明      |
|:---------------|:-----------------|
| Authorization  | Bearer {code}    |
| Content-Type   | application/json |

## <a name="request-body"></a>要求本文

要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター    | 型   |説明|
|:---------------|:--------|:----------|
|displayName|String| 検証グループの表示名。 プロパティは、個別に必要ではありません。 ただし、少なくとも 1 つのプロパティ (表示名または mailNickname) は、必要があります。 |
|mailNickname|String| 検証するためにグループのメール ニックネーム。 プロパティは、個別に必要ではありません。 ただし、少なくとも 1 つのプロパティ (表示名または mailNickname) は、必要があります。 |
|onBehalfOfUserId|Guid| API を呼び出すときに偽装するユーザーのオブジェクト ID です。 検証の結果は、onBehalfOfUserId の属性とロールのです。 |

## <a name="response"></a>応答
正常終了した場合、検証エラーは、メソッドを返します`204 No Content`応答コード。 応答本体には何もは返されません。

メソッドを返すかどうか、要求が有効でない`400 Bad Request`応答コード。 応答本体には、無効な要求に関する詳細情報をエラー メッセージが返されます。

検証エラーがある場合。 メソッドが返す`422 Unprocessable Entity`応答コード。 応答本体には、エラー メッセージとエラーの詳細情報のコレクションが返されます。

## <a name="examples"></a>例

これは、検証が成功した要求の例です。

### <a name="request"></a>要求
<!-- {
  "blockType": "request",
  "name": "group_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 132

{
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a>応答
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

これは、要求の妥当性確認エラーの例です。

### <a name="request"></a>要求
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

### <a name="response"></a>応答
```http
HTTP/1.1 422
Content-type: application/json
Content-length: 223

{
  "error": {
    "code": "Request_UnprocessableEntity",
    "message": "The values provided contain one or more validation errors.",
    "innerError": {
      "request-id": "id-value",
      "date": "date-value"
    },
    "details": [
      {
        "target": "mailNickname",
        "code": "PropertyConflict",
        "message": "Another object with the same value for property mailNickname already exists."
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: validateProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
