---
title: アラートを一覧表示する
description: alert オブジェクトのリストを取得する。
author: preetikr
localization_priority: Priority
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 41f5badd0e4a9ef7ae0580a5c231dae7500b020c
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726607"
---
# <a name="list-alerts"></a>アラートを一覧表示する

[alert](../resources/alert.md) オブジェクトのリストを取得する。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) |  SecurityEvents.Read.All、SecurityEvents.ReadWrite.All  |
|委任 (個人用 Microsoft アカウント) |  サポートされていません。  |
|アプリケーション | SecurityEvents.Read.All、SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}' and {property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドは、応答をカスタマイズするために次の [OData クエリ パラメーター](/graph/query-parameters)をサポートします:

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- `$top` は、各セキュリティ API プロバイダーから集計された上位の結果を返します。  

別のプロパティ セットを返すには、OData `$select` クエリ パラメーターを使用し、目的の **alert** プロパティのセットを指定します。  例えば、**assignedTo**、**category**、および **severity** プロパティを返すには、以下をクエリに追加します: `$select=assignedTo,category,severity`。

> **注:** `$top` ではアラート数が 1000件に制限され、`$top`  +  `$skip` の組み合わせでのアラート数は 6000 件に制限されます。 例えば、`/security/alerts?$top=10&$skip=5990` は応答コード `200 OK` を返しますが、`/security/alerts?$top=10&$skip=5991` は応答コード `400 Bad Request` を返します。  詳細については、「[Microsoft グラフ セキュリティ API のエラー応答](../resources/security-error-codes.md)」を参照してください。

## <a name="request-headers"></a>要求ヘッダー

| 名前      |説明|
|:----------|:----------|
| Authorization  | ベアラー {code}。 必須です。|

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。 要求本文は無視されます。

## <a name="response"></a>応答

成功した場合、このメソッドは応答コード `200 OK` と **alert** オブジェクトのコレクションを応答本文で返します。 プロバイダーから 2xx または 404 以外の状態コードが返されるか、プロバイダーがタイムアウトした場合、応答は、警告ヘッダー内のプロバイダーの応答と共に状態コード `206 Partial Content` になります。 詳細については、「[Microsoft グラフ セキュリティ API のエラー応答](../resources/security-error-codes.md)」を参照してください。

## <a name="example"></a>例

### <a name="request"></a>要求

要求の例を次に示します。

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/security/alerts
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-alerts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-alerts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-alerts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-alerts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>応答

応答の例を次に示します。

>**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "activityGroupName": "activityGroupName-value",
      "assignedTo": "assignedTo-value",
      "azureSubscriptionId": "azureSubscriptionId-value",
      "azureTenantId": "azureTenantId-value",
      "category": "category-value",
      "closedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List alerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
