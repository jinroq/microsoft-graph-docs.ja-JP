---
title: agedAccountsPayable リソースの種類
description: Dynamics 365 Business Central にある、期限切れのアカウントの債務オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: a135627804e2d6c5be4203c0ee0c229642c70c65
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973745"
---
# <a name="agedaccountspayable-resource-type"></a>agedAccountsPayable リソースの種類
Dynamics 365 Business Central の agedAccountsPayable オブジェクトを表します。これは、ベンダーアカウントのエイジングを示しています。

## <a name="methods"></a>メソッド

| メソッド         | 戻り値の型  |説明|
|:---------------|:-------------|:----------|
|[AgedAccountsPayable を取得する](../api/dynamics-agedaccountspayable-get.md)|agedAccountsPayable|AgedAccountsPayable オブジェクトを取得する|

## <a name="properties"></a>プロパティ
| プロパティ      | 型     |説明                                 |
|:--------------|:---------|:-------------------------------------------|
|vendorId       |GUID      |ベンダーの一意の ID。                    |
|vendorNumber   |string    |仕入先の番号を指定します。                  |
|name           |string    |ベンダーの名前を指定します。                    |
|currencyCode   |string    |通貨を指定します。                     |
|定率     |数値   |仕入先による総残高を指定します。|
|currentAmount  |数値   |最初のエイジング期間より前の残高を指定します。|
|period1Amount  |数値   |最初のエイジング期間で残高を指定します。|
|period2Amount  |数値   |2番目のエイジング期間の残高を指定します。|
|period3Amount  |数値   |3番目のエイジング期間の残高を指定します。|
|agedAsOfDate   |date|エイジング期間の計算に使用される期間の開始日を指定します。|
|periodLengthFilter|string |期間の長さを指定します。 時間単位に使用できる値は、D、WD、W、M、Q、または .C で、日付に基づく現在の時間単位は、時間単位のプレフィックスとして指定できます。|


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
