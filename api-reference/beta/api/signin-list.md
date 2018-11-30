---
title: リスト signIns
description: テナントの Azure AD ユーザーのサインインを取得します。 インタラクティブ (ユーザー名とパスワードは認証トークンの一部として渡す) 性質およびフェデレーション サインインが成功には、サインインの問題は現在、サインインがログに含まれます。  最新の signIns が最初に返されます。
ms.openlocfilehash: 3abca59187dcc9667789e33bcefc1bcc51d5ab10
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068090"
---
# <a name="list-signins"></a>リスト signIns

テナントの Azure AD ユーザーのサインインを取得します。 インタラクティブ (ユーザー名とパスワードは認証トークンの一部として渡す) 性質およびフェデレーション サインインが成功には、サインインの問題は現在、サインインがログに含まれます。  最新の signIns が最初に返されます。


## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | AuditLog.Read.All |
|委任 (個人用 Microsoft アカウント) | サポートされていません   |
|アプリケーション | AuditLog.Read.All | 

さらに、アプリケーションでは、Azure AD に[適切に登録](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)をする必要があります。

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```
## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための以下の OData クエリ パラメーターをサポートします。 これらのパラメーターを使用する方法については、 [OData クエリのパラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)を確認してください。

|名前     |説明                            |例|
|:--------------------|----------------|------------------------------------------------------------------------|
|[$filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)|結果 (行) をフィルターします。 |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter)|結果のページ サイズを設定します。|`/auditLogs/signIns?$top=1`|
|[$skiptoken](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter)|取得の結果からの結果の次のページを設定するは、複数ページに します。|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a>$Filter パラメーターでサポートされている属性の一覧
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
|場所と市区町村| eq、startswith|
|場所と状態| eq、startswith|
|場所/countryOrRegion| eq、startswith|
|ステータスまたはエラー コード|eq|
|initiatedBy、構造体、id のユーザー|eq|
|initiatedBy、構造体、displayName ユーザー| eq|
|userPrincipalName/initiatedBy/ユーザー| eq、startswith|
|clientAppUsed| eq|
|conditionalAccessStatus | eq|
|deviceDetail/ブラウザー| eq、startswith|
|deviceDetail/ル| eq、startswith|
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
かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本体での[サインイン](../resources/signin.md)のオブジェクトのコレクションです。
## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "get_signins"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
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
  "tocPath": ""
}-->
