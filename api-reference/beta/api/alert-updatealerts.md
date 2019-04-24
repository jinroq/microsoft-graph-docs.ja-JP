---
title: '通知: updatealerts'
description: 複数の要求ではなく1つの要求で複数の通知を更新します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 5be6374d70baaf4205d5fc1e431111844ce34313
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459316"
---
# <a name="alert-updatealerts"></a>通知: updatealerts

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

複数の要求ではなく1つの要求で複数の通知を更新します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ) |
|:---------------------------------------|:--------------------------------------------|
|委任 (職場または学校のアカウント) |   SecurityEvents.ReadWrite.All  |
|委任 (個人用 Microsoft アカウント) |  サポートされていません。  |
|アプリケーション | SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /security/alerts/updateAlerts
```

## <a name="request-headers"></a>要求ヘッダー

| 名前          | 説明   |
|:--------------|:--------------|
| Authorization | Bearer {code} |

## <a name="request-body"></a>要求本文

要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。 各エンティティには、 **id**プロパティと**vendorInformation**プロパティが必要です。 更新できるプロパティの詳細については、「 [update alert](alert-update.md)」を参照してください。

| パラメーター    | 型        | 説明 |
|:-------------|:------------|:------------|
|value|[alert](../resources/alert.md)コレクション| 更新する通知のコレクション。 各エンティティには、更新する**id**、 **vendorInformation**、およびその他の編集可能なプロパティが必要です。|

## <a name="response"></a>応答

成功した場合、この`200, OK`メソッドは応答コードと、応答本文で[通知](../resources/alert.md)コレクションオブジェクトを返します。

## <a name="examples"></a>例

次の例は、この API を呼び出す方法を示しています。

### <a name="request"></a>要求

要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "alert_updatealerts"
}-->

```http
POST https://graph.microsoft.com/beta/security/alerts/updateAlerts
Content-type: application/json

{
  "value": [
    {
      "assignedTo": "String",
      "closedDateTime": "String (timestamp)",
      "comments": ["String"],
      "feedback": "@odata.type: microsoft.graph.alertFeedback",
      "id": "String (identifier)",
      "status": "@odata.type: microsoft.graph.alertStatus",
      "tags": ["String"],
      "vendorInformation":
        {
          "provider": "String",
          "vendor": "String"
        }
    }
  ]
}
```

### <a name="response"></a>応答

応答の例を次に示します。

> [!NOTE]
> ここに示す response オブジェクトは読みやすいように短縮される場合があります。 実際の呼び出しではすべてのプロパティが返されます。

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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alert: updateAlerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
