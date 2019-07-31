---
title: trialBalance リソースの種類
description: Dynamics 365 Business Central の試算表オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 02e4f039411c992cd1d7335fc2463d660b8ff181
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972874"
---
# <a name="trialbalance-resource-type"></a>trialBalance リソースの種類
Dynamics 365 Business Central の試算表を表します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[TrialBalance の取得](../api/dynamics-trialbalance-get.md)|trialBalance|試算表オブジェクトを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|番号|string|TrialBalance アイテムの G/L アカウント番号|
|accountId|GUID|レコードの G/L アカウントの一意識別子。|
|accountType|string|レコードの G/L アカウントのアカウントの種類。|
|ディスプレイ|string|TrialBalance アイテムの G/L アカウント名。|
|totalDebit|string|G/L アカウントの借方金額の合計を表します。|
|totalCredit|string|G/L アカウントの合計クレジット金額を表します。|
|定率|string|G/L アカウントの日付の金額での正の残高を表します。|
|balanceAtDateCredit|string|G/L アカウントの日付の金額での負の残高を表します。|
|dateFilter|date|TrialBalance のアイテムを計算するために使用される日付フィルター。|


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

