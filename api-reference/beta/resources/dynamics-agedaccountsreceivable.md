---
title: agedAccountsReceivable リソースの種類
description: Dynamics 365 Business Central の期限切れの売掛金勘定オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: ce5d010c08f956468398082821040e30b4ef2ace
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365578"
---
# <a name="agedaccountsreceivable-resource-type"></a>agedAccountsReceivable リソースの種類
Dynamics 365 Business Central の agedAccountsReceivable オブジェクトを表します。これは、顧客アカウントのエージングを示します。

## <a name="methods"></a>メソッド

| メソッド         | 戻り値の型  |説明|
|:---------------|:-------------|:----------|
|[agedAccountsReceivable を取得する](../api/dynamics-agedaccountsreceivable-get.md)|agedAccountsReceivable|agedAccountsReceivable オブジェクトを取得する|

## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明                                  |
|:---------------|:--------|:--------------------------------------------|
|customerId      |GUID     |顧客の一意の ID。                   |
|顧客番号  |string   |顧客の番号を指定します。                 |
|name            |string   |顧客の名前を指定します。                   |
|currencyCode    |string   |通貨を指定します。                      |
|定率      |numeric  |顧客の総残高を指定します。      |
|currentamount   |numeric  |現在のエイジング期間の残高を指定します。|
|period1Amount   |numeric  |最初のエイジング期間で残高を指定します。 |
|period2Amount   |numeric  |2番目のエイジング期間の残高を指定します。|
|period3Amount   |numeric  |3番目のエイジング期間の残高を指定します。 |
|agedasofdate    |日付     |エイジング期間の計算に使用される期間の開始日を指定します。|
|periodLengthFilter|string |期間の長さを指定します。 使用可能な時間の単位は、D、WD、W、M、Q、および Y で、日付に基づく現在の時間単位は、時間単位のプレフィックスとして指定できます。|


## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。


```json
{
    "customerId": "GUID",
    "customerNumber": "string",
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


