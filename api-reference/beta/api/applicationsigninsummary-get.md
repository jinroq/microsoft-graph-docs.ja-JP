---
title: ApplicationSignInSummary を取得する
description: '**ApplicationSigninSummary**オブジェクトのプロパティとリレーションシップを取得します。'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 408a148973d37297f2bbd0bf48a0eee64a914d0f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439554"
---
# <a name="get-applicationsigninsummary"></a>ApplicationSignInSummary を取得する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[ApplicationSigninSummary](../resources/applicationsigninsummary.md)オブジェクトのプロパティとリレーションシップを取得します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference.md)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | すべてのレポートを取得します。 |
|委任 (個人用 Microsoft アカウント) | サポートされていません   |
|アプリケーション | すべてのレポートを取得します。 | 

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
``` http
GET reports/getAzureADApplicationSignInSummary(period='{period}')
```

## <a name="function-parameters"></a>関数パラメーター

| パラメーター | 説明 |
|:----------|:----------|
| period | いずれ`D7`か (過去7日間) `D30`または (過去30日間)。他の値を指定すると、エラーが発生します。 |

## <a name="request-headers"></a>要求ヘッダー
| 名前      |説明|
|:----------|:----------|
| Authorization | Bearer {code} |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答
成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[applicationSignInSummary](../resources/applicationsigninsummary.md)オブジェクトを返します。

## <a name="example"></a>例

##### <a name="request"></a>要求
要求の例を次に示します。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationsigninsummary"
}-->
```http
GET https://graph.microsoft.com/beta/reports/getAzureADApplicationSignInSummary(period='D7')
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationsigninsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationsigninsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationsigninsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>応答
応答の例を次に示します。 

>**注:** ここに示す response オブジェクトは読みやすくするために短縮されている場合があります。 実際の呼び出しではすべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationSignInSummary"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "appId": "appId-value",
  "appDisplayName": "appDisplayName-value",
  "successfulSignInCount": 99,
  "failedSignInCount": 99,
  "successPercentage": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationSignInSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
