---
author: daspek
description: このリソースの下で、指定された期間内に行われたアクティビティの itemActivityStats を取得します。
ms.date: 10/06/2017
title: 間隔ごとにアイテムアクティビティの統計情報を取得する
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 6d1f7a3b4e6a326f107a0d0ff33db59ed73f2794
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979107"
---
# <a name="get-item-activity-stats-by-interval"></a>間隔ごとにアイテムアクティビティの統計情報を取得する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

このリソースの下で、指定された期間内に行われたアクティビティの[Itemactivitystats][]を取得します。

>**注:****Itemanalytics**リソースは、すべての[国内展開](/graph/deployments)でまだ使用できません。

分析集約は、すべてのアクションの種類では使用できない場合があります。

[itemActivityStats]: ../resources/itemactivitystat.md

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)
|:--------------------------------------|:-------------------------------------
|委任 (職場または学校のアカウント)     | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All
|委任 (個人用 Microsoft アカウント) | サポートされていません。
|アプリケーション                            | Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016',endDateTime='2017',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a>関数パラメーター

| パラメーター      | 型               | 説明
|:---------------|:-------------------|:---------------------------------------
| startDateTime  | string (タイムスタンプ) | アクティビティを集計する開始時刻。
| endDateTime    | string (タイムスタンプ) | アクティビティを集約する終了時刻。
| interval       | string             | 集約間隔。

## <a name="example"></a>例

#### <a name="request"></a>要求

<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```

#### <a name="response"></a>応答

<!-- { "blockType": "response", "@type": "Collection(microsoft.graph.itemActivityStat)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "startDateTime": "2017-01-01T00:00:00.000Z",
            "endDateTime": "2017-01-02T00:00:00.000Z",
            "delete": {
                "actionCount": 1,
                "actorCount": 1
            },
            "access": {
                "actionCount": 5,
                "actorCount": 3
            }
        },
        {
            "startDateTime": "2017-01-02T00:00:00.000Z",
            "endDateTime": "2017-01-03T00:00:00.000Z",
            "edit": {
                "actionCount": 3,
                "actorCount": 1
            },
            "access": {
                "actionCount": 7,
                "actorCount": 6
            }
        }
    ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get activities by interval",
  "suppressions": []
}
-->
