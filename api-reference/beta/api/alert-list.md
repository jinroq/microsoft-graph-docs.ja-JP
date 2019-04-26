---
title: アラートを一覧表示する
description: alert オブジェクトの一覧を取得します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: ab9ec3c42b0a46279e43660e241fb3cde52e83a9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322695"
---
# <a name="list-alerts"></a>アラートを一覧表示する

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[alert](../resources/alert.md)オブジェクトの一覧を取得します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) |  securityevents. all、securityevents、ReadWrite  |
|委任 (個人用 Microsoft アカウント) |  サポートされていません。  |
|アプリケーション | securityevents. all、securityevents、ReadWrite |

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

このメソッドは、応答をカスタマイズするために、次の[OData クエリパラメーター](/graph/query-parameters)をサポートしています。

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- `$top`は、各セキュリティ API プロバイダーから集約された上位の結果を返します。

代替プロパティセットを返すには、OData `$select`クエリパラメーターを使用して、必要な**警告**プロパティのセットを指定します。  たとえば、**担当者**、**カテゴリ**、および**重要度**のプロパティを取得するには、クエリ`$select=assignedTo,category,severity`に以下を追加します。

> **注:**`$top`には1000警告の制限があり、の`$top`  +  `$skip`組み合わせは6000通知を超えることはできません。 たとえば、 `/security/alerts?$top=10&$skip=5990`は`200 OK`応答コード`/security/alerts?$top=10&$skip=5991`を返しますが、応答コードを`400 Bad Request`返します。  詳細については、「 [Microsoft Graph セキュリティ API のエラー応答](../resources/security-error-codes.md)」を参照してください。

## <a name="request-headers"></a>要求ヘッダー

| 名前      |説明|
|:----------|:----------|
| Authorization  | ベアラー {code}。 必須です。|

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。 要求本文は無視されます。

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**alert**オブジェクトのコレクションを返します。 2xx または404以外の状態コードがプロバイダーから返された場合、またはプロバイダーがタイムアウトになった場合は`206 Partial Content` 、応答は、警告ヘッダー内のプロバイダーの応答と共に状態コードになります。 詳細については、「 [Microsoft Graph セキュリティ API のエラー応答](../resources/security-error-codes.md)」を参照してください。

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
<!--
{
  "type": "#page.annotation",
  "description": "List alerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
