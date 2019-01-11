---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: 間隔によって項目のアクティビティの統計 (stats) を取得します。
localization_priority: Normal
ms.openlocfilehash: 7ca0e4e4767073d37ebeabbab10e1f50ce323599
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826867"
---
# <a name="get-item-activity-stats-by-interval"></a>間隔によって項目のアクティビティの統計 (stats) を取得します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

このリソース内の指定した時間間隔で行われた活動の[itemActivityStats][]を取得します。

>**注:****ItemAnalytics**リソースはまだすべての[国内展開](/graph/deployments)で使用可能ではありません。

分析の集計は、すべてのアクション タイプにできない可能性があります。

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

| Parameter      | Type               | 説明
|:---------------|:-------------------|:---------------------------------------
| startDateTime  | 文字列 (タイムスタンプ) | 集計の活動に使用される開始時刻。
| endDateTime    | 文字列 (タイムスタンプ) | 集計の活動に使用される終了時間です。
| interval       | 文字列             | 集計間隔です。

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get activities by interval"
} -->
