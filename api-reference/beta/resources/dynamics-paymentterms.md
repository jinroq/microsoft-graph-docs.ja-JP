---
title: paymentTerms リソースの種類
description: Dynamics 365 Business Central の支払い用語オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4ed1f3791474cf6e29038e75fcd3625e4da300a0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507330"
---
# <a name="paymentterms-resource-type"></a>paymentTerms リソースの種類
Dynamics 365 Business Central の支払い条件を表します。

## <a name="methods"></a>メソッド

| メソッド                                                      | 戻り値の型|説明            |
|:------------------------------------------------------------|:-----------|:----------------------|
|[paymentTerms を取得する](../api/dynamics-paymentterms-get.md)      |paymentTerms|支払い用語オブジェクトを取得します。   |
|[Post paymentTerms](../api/dynamics-create-paymentterms.md)  |paymentTerms|支払い用語オブジェクトを作成します。|
|[Patch paymentTerms](../api/dynamics-paymentterms-update.md) |paymentTerms|支払い用語オブジェクトを更新します。|
|[paymentTerms の削除](../api/dynamics-paymentterms-delete.md)|なし        |支払い用語オブジェクトを削除します。|

## <a name="properties"></a>プロパティ
| プロパティ                     | 型     |説明                                                |
|:-----------------------------|:-------|:----------------------------------------------------------|
|id                            |GUID    |paymentTerms の一意の ID。 編集できません。           |
|code                          |string  |支払い条件コードを指定します。                           |
|displayName                   |string  |支払用語の表示名を指定します。                   |
|dueDateCalculation            |string  |支払いが行われる日付の計算に使用される式を指定します。|
|discountDateCalculation       |string  |値引きを取得するために支払いを行う必要がある日付の計算に使用される式を指定します。|
|discountpercent               |decimal |請求金額の早期支払いに適用される割引率を指定します。|
|calculateDiscountOnCreditMemos|ブール値 |クレジットメモに割引を適用する必要があるかどうかを指定します。 **True**は割引が提供されることを示し、 **false**は割引が与えられないことを示します。|
|lastModifiedDateTime          |datetime|paymentTerms が最後に変更された日時。 読み取り専用。|  


## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

paymentTerms の JSON 表記を次に示します。


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "dueDateCalculation": "string",
  "discountDateCalculation": "string",
  "discountPercent": "decimal",
  "calculateDiscountOnCreditMemos": "boolean",
  "lastModifiedDateTime": "datetime"
}

```
