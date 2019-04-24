---
title: 使用するリスト
description: ユーザーが使用するファイルの一覧を返す、計算された洞察。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 2341e41701a2b7306b9e0f1cb89a6b5df76b55ed
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32500854"
---
# <a name="list-used"></a>使用するリスト

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザーが使用するファイルの一覧を返す、計算された洞察。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Sites.Read.All、Sites.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Sites.Read.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求
```http
GET /me/insights/used
```
他のユーザーの使用ドキュメントを要求すると、結果は ' lastModifiedDateTime ' で並べ替えられ、' lastAccessedDateTime ' は ' lastModifiedDateTime ' に設定されます。
```http
GET /users/{id | userPrincipalName}/insights/used
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。

クエリパラメーターを使用`$filter`して、使用されているアイテムをフィルター処理できます。 たとえば、Type に基づいています。

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

またはコンテナーの種類に基づきます。

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

利用可能なコンテナーの種類と種類を表示します。これは、 [resourcevisualization](../resources/insights-resourcevisualization.md)でフィルター処理できます。


## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       |  値|
|:-------------|:------|
| Authorization  | ベアラー {トークン}。必須。|
| 承諾  | application/json|

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[使用され](../resources/insights-used.md)ている項目のリストを返します。
## <a name="example"></a>例

##### <a name="request"></a>要求

以下は、要求の例です。
```http
GET https://graph.microsoft.com/beta/me/insights/used
```

##### <a name="response"></a>応答

以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。 
```http
{
    "value": [
        {   
            "id": "id-value",
            "lastused" : { 
                "lastAccessedDateTime" : "lastAccessedDateTime-value", 
                "lastModifiedDateTime": "lastModifiedDateTime-value" 
            },
            "resourceVisualization": { 
                "title" : "title-value, 
                "type"  : "type-value",
                "mediaType" : "mediaType-value",
                "previewImageUrl" : previewImageUrl-value, 
                "previewText" : "previewText-value", 
                "containerWebUrl" : "containerWebUrl-value", 
                "containerDisplayName" : "containerDisplayName-value", 
                "containerType" : "containerType-value" 
            }, 
            "resourceReference" : { 
                "webUrl" : "webUrl-value", 
                "id": "id-value", 
                "type: "type-value" 
            }
        }
    ]
}
```

### <a name="expanding-resource"></a>リソースの展開
使用されている洞察で参照されているリソースを展開できます。
```http
GET https://graph.microsoft.com/beta/me/insights/used/{id}/resource
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/insights-list-used.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
