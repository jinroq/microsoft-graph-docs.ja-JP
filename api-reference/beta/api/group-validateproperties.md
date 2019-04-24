---
title: 'グループ: validateproperties'
description: Office 365 グループの表示名またはメールニックネームが名前付けポリシーに準拠しているかどうかを検証します。 クライアントは API を使用して、Office 365 グループの**更新**を試行する前に、表示名またはメールニックネームが有効かどうかを判断します。 グループを作成する前にプロパティを検証するには、ディレクトリオブジェクトに対して validateproperties 関数を使用します。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 5361e05d2a58e2d4c27bd662f158d4f185c447fe
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32501939"
---
# <a name="group-validateproperties"></a>グループ: validateproperties

Office 365 グループの表示名またはメールニックネームが名前付けポリシーに準拠しているかどうかを検証します。 クライアントは API を使用して、Office 365 グループの**更新**を試行する前に、表示名またはメールニックネームが有効かどうかを判断します。 グループを作成する前にプロパティを検証するには、ディレクトリオブジェクトに対して[validateproperties 関数](directoryobject-validateproperties.md)を使用します。

[表示名] および [メールニックネーム] プロパティに対して、次の検証が実行されます。 
1. プレフィックスとサフィックスの名前付けポリシーを検証する
2. カスタムの禁止単語のポリシーを検証する

この API は、最初のエラーが発生したことを返します。 1つ以上のプロパティが複数の検証に失敗した場合、最初の検証に失敗したプロパティのみが返されます。 ただし、プレフィックスとサフィックスの名前付けポリシーのみを検証する場合は、メールニックネームと表示名の両方を検証し、検証エラーのコレクションを受信することができます。

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
|displayName|String| 検証するグループの表示名。 プロパティが個別に必要ではありません。 ただし、少なくとも1つのプロパティ (displayName または mailNickname) が必要です。 |
|mailNickname|String| 検証するグループのメールニックネーム。 プロパティが個別に必要ではありません。 ただし、少なくとも1つのプロパティ (displayName または mailNickname) が必要です。 |
|onBehalfOfUserId|Guid| API を呼び出すときに偽装するユーザーのオブジェクト ID。 検証結果は、onBehalfOfUserId の属性とロールに対して行われます。 |

## <a name="response"></a>応答
成功した場合、検証エラーがない場合、メソッド`204 No Content`は応答コードを返します。 応答本文には何も返されません。

要求が無効である場合、メソッドは`400 Bad Request`応答コードを返します。 無効な要求に関する詳細を含むエラーメッセージが応答本文で返されます。

検証エラーが発生した場合。 メソッドは応答`422 Unprocessable Entity`コードを返します。 エラーメッセージとエラーの詳細のコレクションが応答本文で返されます。

## <a name="examples"></a>例

これは、正常な検証要求の例です。

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

これは、検証エラーが発生した要求の例です。

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
