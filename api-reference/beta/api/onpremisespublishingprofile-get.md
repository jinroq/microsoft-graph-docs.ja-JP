---
title: OnPremisesPublishingProfile を取得する
description: '[OnPremisesPublishingProfile](../resources/onpremisespublishingprofile.md)オブジェクトのプロパティとリレーションシップを取得します。'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 92e2800d03cb2e9aab59c119b7a9b7e9f09682d7
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841074"
---
# <a name="get-onpremisespublishingprofile"></a>OnPremisesPublishingProfile を取得する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[OnPremisesPublishingProfile](../resources/onpremisespublishingprofile.md)オブジェクトのプロパティとリレーションシップを取得します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ) |
|:--------------------------------------|:---------------------------------------------------------|
| 委任 (職場または学校のアカウント)     | OnPremisesPublishingProfiles |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。 |
| アプリケーション                            | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。

## <a name="request-headers"></a>要求ヘッダー

| 名前      |説明|
|:----------|:----------|
| Authorization | ベアラー {トークン} |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md)オブジェクトを返します。

## <a name="examples"></a>例

### <a name="request"></a>要求

要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "get_onpremisespublishingprofile"
}-->

```http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning?$expand=publishedResources,agents,agentGroups
```

### <a name="response"></a>応答

応答の例を次に示します。

> **注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```json
HTTP/1.1 200 OK

{
    "publishedResources": [
        {
            "publishingType": "provisioning",
            "displayName": "Demo Provisioning",
            "id": "aed0b780-965f-4149-85c5-a8c73e58b67d",
            "resourceName": "domain1.contoso.com",
            "agentGroups": [
                {
                    "id": "2d55ed41-1619-4848-92bb-0576d3038682",
                    "displayName": "Group 1"
                }
            ]
        }
    ],
    "agents": [
        {
            "id": "1234b780-965f-4149-85c5-a8c73e58b67d",
            "status": "Active",
            "machineName": "server 1",
            "externalIp": "1.0.0.127",
            "agentGroups": [
                 {
                    "id": "2d55ed41-1619-4848-92bb-0576d3038682",
                    "displayName": "Group 1"
                 }
            ]
        }
    ],
    "agentGroups": [
        {
            "id": "2d55ed41-1619-4848-92bb-0576d3038682",
            "displayName": "Group 1",
            "publishingType": "provisioning",
            "isDefault": false,
            "agents": [
                 {
                    "id": "1234b780-965f-4149-85c5-a8c73e58b67d",
                    "status": "Active"
                 }
            ],
            "publishedResources": [
                {
                    "displayName": "Demo Provisioning",
                    "id": "aed0b780-965f-4149-85c5-a8c73e58b67d",
                    "resourceName": "domain1.contoso.com"
                }
            ]
        }
    ],
  "hybridAgentUpdaterConfiguration": {
       "deferUpdateDateTime" : "2018-08-12T12:00",
       "updateWindow" :
          {
            "updateWindowStartTime" : "0:00:00",
            "updateWindowEndTime" : "23:59:00.0000000"
          },
       "allowUpdateConfigurationOverride" : false
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get onPremisesPublishingProfile",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
