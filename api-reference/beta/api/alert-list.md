---
title: アラートを一覧表示する
description: アラート オブジェクトのリストを取得します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: e71b22ae1e60aa2f70bafd4dcd54805e46efdddf
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636556"
---
# <a name="list-alerts"></a>アラートを一覧表示する

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[アラート](../resources/alert.md) オブジェクトのリストを取得します。

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
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドは、応答をカスタマイズするために次の[OData クエリ パラメーター](/graph/query-parameters)をサポートします:

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- `$top` は、各セキュリティ API プロバイダーから集計された上位の結果を返します。

別のプロパティ セットを返すには、OData `$select` クエリ パラメーターを使用し、目的の**アラート**のプロパティのセットを指定します。  例えば、**assignedTo**、**カテゴリ**、**重要度** プロパティを返すには、次をクエリに追加します: `$select=assignedTo,category,severity`。

> **注:** `$top` には1000件のアラートという上限があり、`$top`  +  `$skip` の組み合わせは6000件のアラートを超えることはできません。 例えば、`/security/alerts?$top=10&$skip=5990` では `200 OK` 応答コードを返しますが、`/security/alerts?$top=10&$skip=5991` では `400 Bad Request` 応答コードを返します。  詳細については、[Microsoft グラフ セキュリティ API のエラー応答](../resources/security-error-codes.md)を参照してください。

## <a name="request-headers"></a>要求ヘッダー

| 名前      |説明|
|:----------|:----------|
| Authorization  | ベアラー {code}。 必須です。|

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。 要求本文は無視されます。

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、**アラート** オブジェクトのコレクションを応答本文で返します。 プロバイダーから 2xx または 404 以外の状態コードが返されるか、プロバイダーがタイムアウトした場合、応答は、警告ヘッダー内のプロバイダーの応答と共に`206 Partial Content` 状態コードになります。 詳細については、[Microsoft グラフ セキュリティ API のエラー応答](../resources/security-error-codes.md)を参照してください。

## <a name="example"></a>例

### <a name="request"></a>要求

要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/beta/security/alerts
```

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
#### <a name="sdk-sample-code"></a>SDK サンプルコード
# <a name="ctabcs"></a>[Visual](#tab/cs)
[!INCLUDE [sample-code](../includes/get_alerts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Java](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_alerts-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List alerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/alert-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/alert-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
