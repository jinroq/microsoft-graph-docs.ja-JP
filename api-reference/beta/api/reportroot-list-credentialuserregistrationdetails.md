---
title: CredentialUserRegistrationDetails を一覧表示する
description: 指定したテナントの credentialUserRegistrationDetails オブジェクトの一覧を取得します。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: e11e05c01ec84eda9ef4711e398c810fccfcdf36
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410958"
---
# <a name="list-credentialuserregistrationdetails"></a>CredentialUserRegistrationDetails を一覧表示する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定したテナントの[Credentialuserregistrationdetails](../resources/credentialuserregistrationdetails.md)オブジェクトの一覧を取得します。

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
GET /reports/credentialUserRegistrationDetails
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

この関数は、オプションの OData クエリパラメーター **$filter**をサポートします。 **$Filter**は、 [Credentialuserregistrationdetails](../resources/credentialuserregistrationdetails.md)リソースの次のプロパティの1つ以上に適用できます。

| プロパティ | 説明と例 |
| --------- | ----------------------- |
| userDisplayName | ユーザー名でフィルター処理します。 例: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`。 サポートされて`eq`いるフィルター `startswith()`演算子:、、。 大文字小文字の区別をサポートします。 |
| userPrincipalName | ユーザープリンシパル名でフィルター処理します。 例: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`。 サポートされて`eq`いる`startswith()`フィルター演算子: および。 大文字小文字の区別をサポートします。 |
| authMethods | 登録時に使用される認証方法でフィルター処理します。 例: `/reports/userCredentialUsageDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`。 サポートされて`eq`いるフィルター演算子:。 |
| isRegistered | セルフサービスによるパスワードのリセット (SSPR) に登録されているユーザーを抽出します。 例: `/reports/userCredentialUsageDetails?$filter=isRegistered eq true`。 サポートされて`eq`いるフィルター演算子:。 |
| isEnabled | SSPR に対して有効になっているユーザーを抽出します。 例: `/reports/userCredentialUsageDetails?$filter=isEnabled eq true`。 サポートされて`eq`いる filtter 演算子:。 |
| isCapable | パスワードのリセットまたは多要素認証 (MFA) を実行する準備ができているユーザーをフィルター処理します。 例: `/reports/userCredentialUsageDetails?$filter=isCapable eq true`。 サポートされているフィルター演算子:`eq` |
| isMfaRegistered | MFA に登録されているユーザーを抽出します。 例: `/reports/userCredentialUsageDetails?$filter=isMfaRegistered eq true`。 サポートされて`eq`いるフィルター演算子:。 |

## <a name="request-headers"></a>要求ヘッダー

| 名前      |説明|
|:----------|:----------|
| Authorization | ベアラー {トークン} |
| Content-Type | application/json |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Credentialuserregistrationdetails](../resources/credentialuserregistrationdetails.md)オブジェクトのコレクションを返します。

## <a name="examples"></a>例

次の例は、この API を呼び出す方法を示しています。

### <a name="request"></a>要求

要求の例を次に示します。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_credentialuserregistrationdetails"
}-->

```http
GET https://graph.microsoft.com/beta/reports/credentialUserRegistrationDetails
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-credentialuserregistrationdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-credentialuserregistrationdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-credentialuserregistrationdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>応答

応答の例を次に示します。

> **注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。 すべてのプロパティは、実際の呼び出しから返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.credentialUserRegistrationDetails",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.credentialUserRegistrationDetails)",
  "value":[
    {
      "id" : "id-value",
      "userPrincipalName":"userPrincipalName",
      "userDisplayName": "userDisplayName-value",
      "authMethods": ["email", "mobileSMS"],
      "isRegistered" : false,
      "isEnabled" : true,
      "isCapable" : false,
      "isMfaRegistered" : true
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List credentialUserRegistrationDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
