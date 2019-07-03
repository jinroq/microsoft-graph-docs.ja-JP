---
title: signIns を一覧表示する
description: ディレクトリ (テナント) のアクティビティ (ベータ版) を監査するための、Microsoft Graph API (REST) の signIn リソース (エンティティ) を一覧表示する方法について説明します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7f40d1cd32a8156d88d80ed43b87f5d125a1a0ca
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457171"
---
# <a name="list-signins"></a>signIn を一覧表示する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

テナントの Azure AD ユーザーのサインインを取得します。 本来対話型のサイイン (ユーザー名とパスワードが認証トークンの一部として渡される場合) と、成功したフェデレーション サインインは、現在サインイン ログに含まれています。  最新の signIns が最初に返されます。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | AuditLog.Read.All |
|委任 (個人用 Microsoft アカウント) | サポートされていません   |
|アプリケーション | AuditLog.Read.All | 

また、アプリは Azure AD に[正しく登録されている](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)必要があります。

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```
## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための以下の OData クエリ パラメーターをサポートします。 これらのパラメーターを使用する方法の詳細については、[OData クエリ パラメーター](/graph/query_parameters)をご確認ください。

|Name     |説明                            |例|
|:--------------------|----------------|------------------------------------------------------------------------|
|[$filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)|結果 (行) をフィルターします。 |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter)|結果のページ サイズを設定します。|`/auditLogs/signIns?$top=1`|
|[$skiptoken](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter)|複数ページにわたる結果セットから、結果の次のページを取得します。|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a>$Filter パラメーターにサポートされる属性の一覧
|属性名 |サポートされる演算子|
|:----------------|:------|
|id|eq|
|userId|eq|
|appId|eq|
|createdDateTime| eq、le、ge|
|userDisplayName| eq、startswith|
|userPrincipalName| eq、startswith|
|appDisplayName| eq、startswith|
|ipAddress| eq、startswith|
|location/city| eq、startswith|
|location/state| eq、startswith|
|location/countryOrRegion| eq、startswith|
|status/errorCode|eq|
|initiatedBy/user/id|eq|
|initiatedBy/user/displayName| eq|
|initiatedBy/user/userPrincipalName| eq、startswith|
|clientAppUsed| eq|
|conditionalAccessStatus | eq|
|deviceDetail/browser| eq、startswith|
|deviceDetail/operatingSystem| eq、startswith|
|correlationId| eq|
|riskDetail| eq|
|riskLevelAggregated| eq|
|riskLevelDuringSignIn| eq|
|riskEventTypes| eq|
|riskState| eq|
|originalRequestId| eq|
|tokenIssuerName| eq|
|tokenIssuerType| eq|
|resourceDisplayName| eq|
|resourceId| eq|


## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードと、[signIn](../resources/signin.md) オブジェクトのコレクションを応答本文で返します。
## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signins"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signins-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signins-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signins-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>応答
以下は、応答の例です。 

>**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 264
```
```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
    "value": [{
        "id":"b01b1726-0147-425e-a7f7-21f252050400",
        "createdDateTime":"2018-11-06T18:48:33.8527147Z",
        "userDisplayName":"Jon Doe",
         "userPrincipalName":"admin@aad171.ccsctp.net",
         "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
        "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
         "appDisplayName":"Azure Portal",
         "ipAddress":"207.254.19.10",
         "clientAppUsed":"Browser",
        "mfaDetail":null,
         "correlationId":"65dd87ce-2183-419e-81a9-d6e20379bcc2",
         "conditionalAccessStatus":"notApplied",
        "originalRequestId":null,
        "isInteractive":true,
        "tokenIssuerName":null,
        "tokenIssuerType":"AzureAD",
        "processingTimeInMilliseconds":0,
        "riskDetail":"none",
        "riskLevelAggregated":"none",
        "riskLevelDuringSignIn":"none",
        "riskState":"none",
        "riskEventTypes":[

        ],
        "resourceDisplayName":"windows azure service management api",
        "resourceId":"797f4846-ba00-4fd7-ba43-dac1f8f63013",
        "authenticationMethodsUsed":[

        ],
        "status":{
            "errorCode":50140,
            "failureReason":"This error occurred due to 'Keep me signed in' interrupt when the user was signing-in.",
            "additionalDetails":null
        },
        "deviceDetail":{
            "deviceId":null,
            "displayName":null,
            "operatingSystem":"Windows 7",
            "browser":"Chrome 63.0.3239",
            "isCompliant":null,
            "isManaged":null,
            "trustType":null
        },
        "location":{
            "city":"Lithia Springs",
            "state":"Georgia",
            "countryOrRegion":"US",
            "geoCoordinates":{
                "altitude":null,
                "latitude":33.7930908203125,
                "longitude":-84.445358276367188
            }
        },
        "appliedConditionalAccessPolicies":[
            {
            "id":"6551c58c-e5da-4036-a6ea-c2c3fad264f1",
            "displayName":"New Name here4",
            "enforcedGrantControls":[
                "Mfa",
                "RequireCompliantDevice"
            ],
            "enforcedSessionControls":[

            ],
            "result":"notApplied"
            },
            {
            "id":"b645a140-20fe-4ce0-a724-18ab201e9026",
            "displayName":"PipelineTest4",
            "enforcedGrantControls":[

            ],
            "enforcedSessionControls":[

            ],
            "result":"notEnabled"
            }
        ],
        "authenticationProcessingDetails":[

        ],
        "networkLocationDetails":[

        ]
        }
    
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List signIns",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
