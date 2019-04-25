---
title: trialbalance リソースの種類
description: Dynamics 365 Business Central の試算表オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1a7e906e50ddf39e4c9e2d3d9dde11226c7ec662
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534851"
---
# <a name="trialbalance-resource-type"></a>trialbalance リソースの種類
Dynamics 365 Business Central の試算表を表します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[trialbalance の取得](../api/dynamics-trialbalance-get.md)|trialbalance|試算表オブジェクトを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|番号|string|trialbalance アイテムの G/L アカウント番号|
|accountId|GUID|レコードの G/L アカウントの一意識別子。|
|accountType|string|レコードの G/L アカウントのアカウントの種類。|
|ディスプレイ|string|trialbalance アイテムの G/L アカウント名。|
|totaldebit|string|G/L アカウントの借方金額の合計を表します。|
|totalcredit|string|G/L アカウントの合計クレジット金額を表します。|
|定率|string|G/L アカウントの日付の金額での正の残高を表します。|
|balanceAtDateCredit|string|G/L アカウントの日付の金額での負の残高を表します。|
|datefilter|日付|trialbalance のアイテムを計算するために使用される日付フィルター。|


## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。


```json
{
    "number": "string",
    "accountId": "GUID",
    "accountType": "string",
    "display": "string",
    "totalDebit": "string",
    "totalCredit": "string",
    "balanceAtDateDebit": "string",
    "balanceAtDateCredit": "string",
    "dateFilter": "date"
}

```

