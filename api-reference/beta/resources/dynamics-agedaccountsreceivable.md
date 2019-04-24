---
title: agedAccountsReceivable リソースの種類
description: Dynamics 365 Business Central の期限切れの売掛金勘定オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: ce5d010c08f956468398082821040e30b4ef2ace
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507617"
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
|id      |GUID     |顧客の一意の ID。                   |
|顧客番号  |string   |顧客の番号を指定します。                 |
|name            |string   |顧客の名前を指定します。                   |
|currencyCode    |string   |通貨を指定します。                      |
|定率      |数値  |顧客の総残高を指定します。      |
|currentamount   |数値  |現在のエイジング期間の残高を指定します。|
|period1Amount   |数値  |最初のエイジング期間で残高を指定します。 |
|period2Amount   |数値  |2番目のエイジング期間の残高を指定します。|
|period3Amount   |数値  |3番目のエイジング期間の残高を指定します。 |
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


