---
title: アラートを更新する
description: ソリューション間でアラートの状態と割り当てを同期させるために、任意の統合ソリューション内の編集可能な**警告**プロパティを更新します。 このメソッドは、参照される警告 ID のレコードを持つソリューションを更新します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 42bc945dde726466439802350796d628ee438e22
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551511"
---
# <a name="update-alert"></a>アラートを更新する

ソリューション間でアラートの状態と割り当てを同期させるために、任意の統合ソリューション内の編集可能な**警告**プロパティを更新します。 このメソッドは、参照される警告 ID のレコードを持つソリューションを更新します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ) |
|:---------------------------------------|:------------------------------------|
| 委任 (職場または学校のアカウント)     | SecurityEvents.ReadWrite.All        |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。                      |
| アプリケーション                            | SecurityEvents.ReadWrite.All        |

## <a name="http-request"></a>HTTP 要求

> **注:** このメソッドを使用**** して、 `provider`および`vendor`を含む vendorInformation というパラメーターとして、警告 ID を含める必要があります。

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a>要求ヘッダー

| 名前          | 説明              |
|:--------------|:-------------------------|
| Authorization | ベアラー {code}。 必須。 |
| Prefer        | 戻り値 = 表現    |

## <a name="request-body"></a>要求本文

要求本文で、更新する必要のある関連フィールドの値の JSON 表記を指定します。 本文には、有効`vendorInformation`な`provider` `vendor`フィールドとフィールドのプロパティが含まれて**いる必要があり**ます。 次の表に、通知に対して更新できるフィールドを示します。 要求本文に含まれていない既存のプロパティの値は変更されません。 最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。

| プロパティ          | 型                                                                   | 説明 |
|:------------------|:-----------------------------------------------------------------------|:--|
| assignedTo        | String                                                                 | トリアージ、調査、または修復のためにアラートが割り当てられたアナリストの名前。 |
| closeddatetime    | DateTimeOffset                                                         | 通知が終了した時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` |
| コメント          | String collection                                                      | アラートに関するアナリストのコメント (顧客の警告管理)。 |
| feedback          | alertFeedback                                                          | アラートに関するアナリストのフィードバック。 可能な値は、`unknown`、`truePositive`、`falsePositive`、`benignPositive` です。 |
| status            | alertStatus                                                            | アラートライフサイクルの状態 (ステージ)。 可能な値は、`unknown`、`newAlert`、`inProgress`、`resolved` です。 |
| tags              | String コレクション                                                      | 通知に適用することができ、フィルター条件として機能することができる、ユーザー定義のラベル (たとえば、"hva"、"のこぎり" など)。 |
| vendorInformation | [securityVendorInformation](../resources/securityvendorinformation.md) | セキュリティ製品/サービスのベンダー、プロバイダ、およびサブプロバイダに関する詳細を含む複合型 (たとえば、vendor = Microsoft; provider = Windows Defender ATP; subprovider = AppLocker)。 **プロバイダーおよびベンダーフィールドは必須です。** |

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。

オプションの要求ヘッダーが使用されている場合、 `200 OK`メソッドは応答コードと、応答本文で更新された[alert](../resources/alert.md)オブジェクトを返します。

## <a name="examples"></a>例

### <a name="example-1-request-without-prefer-header"></a>例 1: 希望するヘッダーのない要求

#### <a name="request"></a>要求

要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
Content-type: application/json

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": [
    "String"
  ],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": [
    "String"
  ],
  "vendorInformation": {
    "provider": "String",
    "vendor": "String"
  }
}
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a>応答

成功応答の例を次に示します。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a>例 2: 要求ヘッダーを使用した要求

#### <a name="request"></a>要求

次の例は、 `Prefer`要求ヘッダーを含む要求を示しています。

<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
Content-type: application/json
Prefer: return=representation

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": [
    "String"
  ],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": [
    "String"
  ],
  "vendorInformation": {
    "provider": "String",
    "vendor": "String"
  }
}
```

#### <a name="response"></a>応答

オプション`Prefer: return=representation`の要求ヘッダーを使用する場合の応答の例を次に示します。

> **注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。

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
