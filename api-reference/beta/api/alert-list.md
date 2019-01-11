---
title: 警告の一覧表示
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: 6036514c2aeabe287fd019ce69157d4b7897af60
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860208"
---
# <a name="list-alerts"></a>警告の一覧表示

 > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

オブジェクトの[アラート](../resources/alert.md)の一覧を取得します。

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

このメソッドは、応答をカスタマイズするために次の[OData クエリ パラメーター](/graph/query-parameters)をサポートします。

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- `$top`セキュリティ API の各プロバイダーから集計の上位の結果を返します。  

OData を使用する別のプロパティ セットを返すには、`$select`する**警告**のプロパティのセットを指定するパラメーター クエリを実行します。  たとえば、**担当者**、**カテゴリ**、および**重要度**のプロパティを返す、クエリに次を追加: `$select=assignedTo,category,severity`。

> **注:**`$top` 1000 の警告との組み合わせの制限が`$top`  +  `$skip` 6000 のアラートを超えることはできません。 などの`/security/alerts?$top=10&$skip=5990`を返します、`200 OK`応答コードの場合が、`/security/alerts?$top=10&$skip=5991`を返します、`400 Bad Request`応答コード。  詳細については、 [Microsoft グラフ セキュリティ API のエラー応答](../resources/security-error-codes.md)を参照してください。

## <a name="request-headers"></a>要求ヘッダー

| 名前      |説明|
|:----------|:----------|
| Authorization  | Bearer {code}。必須。|

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。 要求の本体は無視されます。

## <a name="response"></a>応答

かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の**通知**オブジェクトのコレクションです。 2 xx または 404 以外のステータス コードは、プロバイダーから返された場合、またはプロバイダーがタイムアウトすると、応答がある場合、`206 Partial Content`警告ヘッダー内のプロバイダーの応答のステータス コード。 詳細については、 [Microsoft グラフ セキュリティ API のエラー応答](../resources/security-error-codes.md)を参照してください。

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List alerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
