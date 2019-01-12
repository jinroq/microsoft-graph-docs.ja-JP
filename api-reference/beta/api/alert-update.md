---
title: 警告の更新
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 8b8e21334d9a94d6a41c1e283959bd6473c11e1a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990621"
---
# <a name="update-alert"></a>警告の更新

 > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

アラートの状態および割り当ての同期を保つソリューション全体に統合されたソリューション内で、編集可能な**アラート**のプロパティを更新します。 このメソッドは、id。 参照されているアラートのレコードがどのようなソリューションを更新します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) |   SecurityEvents.ReadWrite.All  |
|委任 (個人用 Microsoft アカウント) |  サポートされていません。  |
|アプリケーション | SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

> **注:** パラメーターおよび vendorInformation が含まれていると**警告**の ID を含める必要があります、`provider`と`vendor`このメソッドを使用します。
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 説明|
|:-----------|:-----------|
| Authorization  | Bearer {code}。必須。|
|Prefer | 返す = 表現 |

## <a name="request-body"></a>要求本文

要求の本文には、更新される関連フィールドの値の JSON の形式を指定します。 含まれている**必要があります**本体、`vendorInformation`プロパティに有効な`provider`と`vendor`のフィールドです。 次の表では、アラートの更新可能なフィールドを示します。 要求の本文に含まれていない既存のプロパティの値は変更されません。 最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。

| プロパティ   | 型 |説明|
|:---------------|:--------|:----------|
|担当者|String|アナリスト、警告の名前は、選別、調査、または修復用に割り当てられます。|
|closedDateTime|DateTimeOffset|時間のアラートが閉じられました。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|comments|String コレクション|(顧客の警告管理) の警告のアナリストのコメントです。|
|feedback|alertFeedback 列挙型|アナリストのフィードバック通知をします。 可能な値は、`unknown`、`truePositive`、`falsePositive`、`benignPositive` です。|
|status|alertStatus 列挙型|アラートのライフ サイクルのステータス (ステージ)。 可能な値は、`unknown`、`newAlert`、`inProgress`、`resolved` です。|
|タグの前に追加されるマークアップ|String コレクション|アラートに適用することができますし、フィルターの条件 (たとえば、"HVA"、"されていた) として使用できるユーザー定義のラベル。|
|vendorInformation |[securityVendorInformation](../resources/securityvendorinformation.md)|セキュリティ製品やサービスの仕入先、プロバイダー、および subprovider の詳細を含む複合型 (仕入先など = Microsoft; プロバイダー = Windows Defender の ATP は subProvider AppLocker を =)。 **プロバイダーおよび仕入先のフィールドは、必要があります。**|

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。

省略可能な要求ヘッダーが使用され、メソッドが返されます、`200 OK`応答コードおよび応答の本体で更新された[アラート](../resources/alert.md)オブジェクトです。

## <a name="example-1"></a>例 1

### <a name="request"></a>要求

要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/alerts/{alert_id}
Content-type: application/json

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```

### <a name="response"></a>応答

次は、正常な応答の例です。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="example-2"></a>例 2

### <a name="request"></a>要求

次の例では、要求を含む、`Prefer`要求ヘッダー。

<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/alerts/{alert_id}
Content-type: application/json
Prefer: return=representation

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```

### <a name="response"></a>応答

次の応答の例ではときに、省略可能な`Prefer: return=representation`要求ヘッダーを使用します。

>**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "activityGroupName": "activityGroupName-value",
  "assignedTo": "assignedTo-value",
  "azureSubscriptionId": "azureSubscriptionId-value",
  "azureTenantId": "azureTenantId-value",
  "category": "category-value",
  "closedDateTime": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update alert",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
