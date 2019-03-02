---
title: agedaccountspayable リソースの種類
description: Dynamics 365 Business Central にある、期限切れのアカウントの債務オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 679c24b7ef32ef59b34a5885ea745d8c244376b2
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365907"
---
# <a name="agedaccountspayable-resource-type"></a>agedaccountspayable リソースの種類
Dynamics 365 Business Central の agedaccountspayable オブジェクトを表します。これは、ベンダーアカウントのエイジングを示しています。

## <a name="methods"></a>メソッド

| メソッド         | 戻り値の型  |説明|
|:---------------|:-------------|:----------|
|[agedaccountspayable を取得する](../api/dynamics-agedaccountspayable-get.md)|agedaccountspayable|agedaccountspayable オブジェクトを取得する|

## <a name="properties"></a>プロパティ
| プロパティ      | 型     |説明                                 |
|:--------------|:---------|:-------------------------------------------|
|vendorId       |GUID      |ベンダーの一意の ID。                    |
|vendorNumber   |string    |仕入先の番号を指定します。                  |
|name           |string    |ベンダーの名前を指定します。                    |
|currencyCode   |string    |通貨を指定します。                     |
|定率     |numeric   |仕入先による総残高を指定します。|
|currentamount  |numeric   |最初のエイジング期間より前の残高を指定します。|
|period1Amount  |numeric   |最初のエイジング期間で残高を指定します。|
|period2Amount  |numeric   |2番目のエイジング期間の残高を指定します。|
|period3Amount  |numeric   |3番目のエイジング期間の残高を指定します。|
|agedasofdate   |日付|エイジング期間の計算に使用される期間の開始日を指定します。|
|periodLengthFilter|string |期間の長さを指定します。 時間単位に使用できる値は、D、WD、W、M、Q、または .c で、日付に基づく現在の時間単位は、時間単位のプレフィックスとして指定できます。|


## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。


```json
{
    "vendorId": "GUID",
    "vendorNumber": "string",
    "name": "string",
    "currencyCode": "string",
    "balanceDue": "decimal",
    "currentAmount": "decimal",
    "period1Amount": "decimal",
    "period2Amount": "decimal",
    "period3Amount": "decimal",
    "agedAsOfDate": "date",
    "periodLengthFilter": "string"
}

```
