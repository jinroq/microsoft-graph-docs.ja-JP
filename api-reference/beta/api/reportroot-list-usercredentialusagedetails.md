---
title: Usercredentialの詳細を一覧表示する
description: 指定したテナントの Usercredentialの詳細オブジェクトの一覧を取得します。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 1ea46387a4d4f4c0920a94a2d082a20090fe0bb0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871232"
---
# <a name="list-usercredentialusagedetails"></a>Usercredentialの詳細を一覧表示する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定したテナントの[Usercredentialの詳細](../resources/usercredentialusagedetails.md)オブジェクトの一覧を取得します。 詳細には、ユーザー情報、リセットの状態、およびエラーの理由が含まれます。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ) |
|:---------------------------------------|:--------------------------------------------|
| 委任 (職場または学校アカウント)     | Reports.Read.All |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。 |
| アプリケーション                            | Reports.Read.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET /reports/userCredentialUsageDetails
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

この関数は、オプションの OData クエリパラメーター **$filter**をサポートします。 [Usercredentialの詳細](../resources/usercredentialusagedetails.md)リソースの次のプロパティの1つ以上に **$filter**を適用できます。

| プロパティ | 説明と例 |
|:--------- |:----------- |
| 特徴 | 必要な利用状況データの種類 (登録とリセット) によってフィルター処理します。 例: `/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`。 サポートされているフィルター演算子:`eq` |
| userDisplayName | ユーザーの表示名でフィルター処理します。 例: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`。 サポートされて`eq`いる`startswith()`フィルター演算子: および。 大文字小文字の区別をサポートします。 |
| userPrincipalName  | ユーザープリンシパル名でフィルター処理します。 例: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`。    サポートされて`eq`いる`startswith()`フィルター演算子: および。 大文字小文字の区別をサポートします。 |
| この | アクティビティの状態によってフィルター処理します。 例: `/reports/userCredentialUsageDetails?$filter=isSuccess eq true`。 サポートされて`eq`いる`orderby`フィルター演算子: および。 |
| authMethod  | 登録時にを使用して、認証方法によってフィルター処理を行います。 例: `/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`。 サポートされて`eq`いるフィルター演算子:。 |
| failureReason | 失敗の理由 (アクティビティが失敗した場合) でフィルター処理します。 例: `/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`。 サポートされて`eq`いる`startswith()`フィルター演算子: および。 大文字小文字の区別をサポートします。 |


## <a name="request-headers"></a>要求ヘッダー

| 名前      |説明|
|:----------|:----------|
| Authorization | ベアラー {トークン} |
| Content-Type | application/json |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Usercredentialの details](../resources/usercredentialusagedetails.md)オブジェクトのコレクションを返します。

## <a name="examples"></a>例

次の例は、この API を呼び出す方法を示しています。

### <a name="request"></a>要求

要求の例を次に示します。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_usercredentialusagedetails"
}-->

```http
GET https://graph.microsoft.com/beta/reports/userCredentialUsageDetails
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-usercredentialusagedetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-usercredentialusagedetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-usercredentialusagedetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-usercredentialusagedetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>応答

応答の例を次に示します。

> **注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。 すべてのプロパティは、実際の呼び出しから返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userCredentialUsageDetails",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 258

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.getUserCredentialUsageDetails)",
  "value":[
    {
      "id" : "id-value",
      "feature":"registration",
      "userPrincipalName":"userPrincipalName-value",
      "userDisplayName": "userDisplayName-value",
      "isSuccess" : true,
      "authMethod": "email",
      "failureReason": "User contacted an admin after trying the email verification option",
      "eventDateTime" : "2019-04-01T00:00:00Z"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List userCredentialUsageDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
