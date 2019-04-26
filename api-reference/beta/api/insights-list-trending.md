---
title: 人気上昇中を一覧表示する
description: ユーザーの周囲のアイテムのリストを返す、計算された洞察。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 49f777e77663a4c055e186860f791459db57ca9c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33323697"
---
# <a name="list-trending"></a>人気上昇中を一覧表示する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザーの周囲のアイテムのリストを返す、計算された洞察。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。


|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Sites.Read.All、Sites.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Sites.Read.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求
```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。

クエリパラメーターを使用`$filter`して、傾向分析項目をフィルター処理できます。 たとえば、Type に基づいています。

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

またはコンテナーの種類に基づきます。

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

利用可能なコンテナーの種類と種類を表示します。これは、 [resourcevisualization](../resources/insights-resourcevisualization.md)でフィルター処理できます。


## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       |  値|
|:-------------|:------|
| Authorization  | ベアラー {トークン}。必須。|
| 承諾  | application/json|

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[傾向](../resources/insights-trending.md)項目のリストを返します。 各アイテムには、アイテムを表示するための視覚エフェクトプロパティが含まれています。

## <a name="example"></a>例
#### <a name="request"></a>要求
以下は、要求の例です。
```http
GET https://graph.microsoft.com/beta/me/insights/trending
```
#### <a name="response"></a>応答
以下は、応答の例です。 注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。 実際の呼び出しではすべてのプロパティが返されます。 ページの下部にある、切り捨てられていない応答の例を参照してください。
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 801

{
    "value": [
        {
            "id": "id-value",
            "weight": "weight-value",
            "resourceVisualization": {
                "title": "title-value",
                "type": "type-value",
                "mediaType": "mediaType-value",
                "previewImageUrl": "previewImageUrl-value",
                "previewText": "previewText-value",
                "containerWebUrl": "containerWebUrl-value",
                "containerDisplayName": "containerDisplayName-value",
                "containerType": "containerType-value"
            },
            "resourceReference": {
                "webUrl": "webUrl-value",
                "id": "id-value",
                "type": "type-value"
            }
        }
    ]
}
```

### <a name="expanding-resource"></a>リソースの展開
傾向分析によって参照されているリソースを展開できます。
```http
GET https://graph.microsoft.com/beta/me/insights/trending/{id}/resource
```
