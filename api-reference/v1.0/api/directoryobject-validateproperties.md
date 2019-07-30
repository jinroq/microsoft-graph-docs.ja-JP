---
title: 'directoryObject: validateProperties'
description: Office 365 グループの表示名またはメールニックネームが名前付けポリシーに準拠していることを確認します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f26857514ec180dbbc50c73eeb8eccc4b30185ed
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932215"
---
# <a name="directoryobject-validateproperties"></a>directoryObject: validateProperties

Office 365 グループの表示名またはメールニックネームが名前付けポリシーに準拠していることを確認します。  クライアントは、この API を使用して、Office 365 グループを[作成](group-post-groups.md)する前に、表示名またはメールニックネームが有効かどうかを判断します。 既存のグループのプロパティを検証するには、 [group: validateProperties](group-validateproperties.md)関数を使用します。

[表示名] および [メールニックネーム] プロパティに対して、次のポリシー検証が実行されます。 
1. プレフィックスとサフィックスの名前付けポリシーを検証する
2. カスタムの禁止単語のポリシーを検証する
3. メールニックネームが一意であることを確認する

この API は、検出された最初の検証エラーのみを返します。 プロパティが複数の検証に失敗した場合は、最初の検証エラーのみが返されます。 ただし、プレフィックスとサフィックスの名前付けポリシーのみを検証する場合は、メールニックネームと表示名の両方を検証し、検証エラーのコレクションを受信することができます。 名前付けポリシーの構成の詳細については、「 [Configure ネーミング policy](https://docs.microsoft.com/en-us/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell)」を参照してください。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a>要求ヘッダー

| 名前           | 説明      |
|:---------------|:-----------------|
| Authorization  | ベアラー {トークン}。必須。    |
| Content-Type   | application/json |

## <a name="request-body"></a>要求本文
要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター    | 型   |説明|
|:---------------|:--------|:----------|
|entityType|String| Group は、サポートされている唯一のエンティティの種類です。 |
|displayName|文字列| 検証するグループの表示名。 プロパティが個別に必要ではありません。 ただし、少なくとも1つのプロパティ (**displayName**または**mailNickname**) が必要です。 |
|mailNickname|String| 検証するグループのメールニックネーム。 プロパティが個別に必要ではありません。 ただし、少なくとも1つのプロパティ (**displayName**または**mailNickname**) が必要です。 |
|onBehalfOfUserId|Guid| API を呼び出すときに偽装するユーザーの ID。 検証結果は、 **onBehalfOfUserId の**属性とロールに対して行われます。 |

## <a name="response"></a>応答

成功した場合、検証エラーがない場合、メソッド`204 No Content`は応答コードを返します。 応答本文には何も返されません。

要求が無効である場合、メソッドは`400 Bad Request`応答コードを返します。 無効な要求に関する詳細を含むエラーメッセージが応答本文で返されます。

検証エラーが発生した場合、メソッドは`422 Unprocessable Entity`応答コードを返します。 エラーメッセージとエラーの詳細のコレクションが応答本文で返されます。

## <a name="examples"></a>例

### <a name="example-1-successful-validation-request"></a>例 1: 正常な検証要求
これは、正常な検証要求の例です。

#### <a name="request"></a>要求

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/v1.0/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>応答
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```


### <a name="example-2-request-with-validation-errors"></a>例 2: 検証エラーがある要求
これは、検証エラーが発生した要求の例です。

#### <a name="request"></a>要求
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "test",
  "mailNickname": "test",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

#### <a name="response"></a>応答
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
