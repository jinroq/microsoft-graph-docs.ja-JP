---
title: 'directoryObject: validateProperties'
description: Office 365 のグループの表示名やメールのニックネームは、命名ポリシーに準拠している場合を検証します。  クライアントは、API を使用して場合は、表示名を確認または、Office 365 のグループ**を作成**する前に、メールのニックネームが無効です。 既存のグループのプロパティを検証するためには、グループの validateProperties 関数を使用します。
localization_priority: Normal
ms.openlocfilehash: 1f38a30d86cf5b28eea6b9891687c4dbca4b78fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879822"
---
# <a name="directoryobject-validateproperties"></a>directoryObject: validateProperties

Office 365 のグループの表示名やメールのニックネームは、命名ポリシーに準拠している場合を検証します。  クライアントは、API を使用して場合は、表示名を確認または、Office 365 のグループ**を作成**する前に、メールのニックネームが無効です。 既存のグループのプロパティを検証するためには、グループの[validateProperties 関数](group-validateproperties.md)を使用します。

表示名とメールのニックネームのプロパティには、次の検証が実行されます。 
1. プリフィックスおよびサフィックスの名前付けポリシーを検証します。
2. 禁止された単語をカスタム ポリシーを検証します。
3. 検証、メールのニックネームが一意では

この API は、最初のエラーが発生しましたを返します。 1 つまたは複数のプロパティには、複数の検証が失敗した場合、最初の検証エラーのプロパティだけが返されます。 ただし、メールのニックネームと表示名の両方を検証し、検証エラーのコレクションが表示される場合は、プレフィックスとサフィックスの名前付けポリシーを検証しているだけです。

## <a name="prerequisites"></a>必須条件

この API を実行するために次の**アクセス許可**が必要です: *Group.Read.All*

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a>要求ヘッダー

| 名前           | 説明      |
|:---------------|:-----------------|
| Authorization  | Bearer {code}    |
| Content-Type   | application/json |

## <a name="request-body"></a>要求本文
要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター    | Type   |説明|
|:---------------|:--------|:----------|
|entityType|String| `Group`唯一サポートされているエンティティの種類です。 |
|displayName|String| 検証グループの表示名。 プロパティは、個別に必要ではありません。 ただし、少なくとも 1 つのプロパティ (表示名または mailNickname) は、必要があります。 |
|mailNickname|String| 検証するためにグループのメール ニックネーム。 プロパティは、個別に必要ではありません。 ただし、少なくとも 1 つのプロパティ (表示名または mailNickname) は、必要があります。 |
|onBehalfOfUserId|Guid| API を呼び出すときに偽装するユーザーのオブジェクト ID です。 検証の結果は、onBehalfOfUserId の属性とロールのです。 |

## <a name="response"></a>応答

正常終了した場合、検証エラーは、メソッドを返します`204 No Content`応答コード。 応答本体には何もは返されません。

メソッドを返すかどうか、要求が有効でない`400 Bad Request`応答コード。 応答本体には、無効な要求に関する詳細情報をエラー メッセージが返されます。

メソッドを返すかどうかは検証エラーがある場合、`422 Unprocessable Entity`応答コード。 応答本体には、エラー メッセージとエラーの詳細情報のコレクションが返されます。

## <a name="examples"></a>例

これは、検証が成功した要求の例です。

### <a name="request"></a>要求
<!-- {
  "blockType": "request",
  "name": "directoryobject_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a>応答
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

これは、要求の妥当性確認エラーの例です。

### <a name="request"></a>要求
```http
POST https://graph.microsoft.com/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "test",
  "mailNickname": "test",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a>応答
```http
HTTP/1.1 422 
Content-Type: application/json

{
  "error": {
    "code": "Request_UnprocessableEntity",
    "message": "The values provided contain one or more validation errors.",
    "innerError": {
      "request-id": "request-id-value",
      "date": "date-value"
    },
    "details": [
      {
        "target": "displayName",
        "code": "MissingPrefixSuffix",
        "message": "Property mailNickname is missing a required prefix/suffix per your organization's Group naming requirements.",
        "prefix": "Myprefix_",
        "suffix": "_mysuffix"
      },
      {
        "target": "mailNickname",
        "code": "MissingPrefixSuffix",
        "message": "Property mailNickname is missing a required prefix/suffix per your organization's Group naming requirements.",
        "prefix": "Myprefix_",
        "suffix": "_mysuffix"
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: validateProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
