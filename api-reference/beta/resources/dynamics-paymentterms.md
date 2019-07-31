---
title: paymentTerms リソースの種類
description: Dynamics 365 Business Central の支払い用語オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: d367314d5546c59dd251b30e952aa17b9d60ce10
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006599"
---
# <a name="paymentterms-resource-type"></a>paymentTerms リソースの種類
Dynamics 365 Business Central の支払い条件を表します。

## <a name="methods"></a>メソッド

| メソッド                                                      | 戻り値の型|説明            |
|:------------------------------------------------------------|:-----------|:----------------------|
|[PaymentTerms を取得する](../api/dynamics-paymentterms-get.md)      |paymentTerms|支払い用語オブジェクトを取得します。   |
|[Post paymentTerms](../api/dynamics-create-paymentterms.md)  |paymentTerms|支払い用語オブジェクトを作成します。|
|[Patch paymentTerms](../api/dynamics-paymentterms-update.md) |paymentTerms|支払い用語オブジェクトを更新します。|
|[PaymentTerms の削除](../api/dynamics-paymentterms-delete.md)|none        |支払い用語オブジェクトを削除します。|

## <a name="properties"></a>プロパティ
| プロパティ                     | 型     |説明                                                |
|:-----------------------------|:-------|:----------------------------------------------------------|
|id                            |GUID    |PaymentTerms の一意の ID。 編集できません。           |
|code                          |string  |支払い条件コードを指定します。                           |
|displayName                   |string  |支払用語の表示名を指定します。                   |
|dueDateCalculation            |string  |支払いが行われる日付の計算に使用される式を指定します。|
|discountDateCalculation       |string  |値引きを取得するために支払いを行う必要がある日付の計算に使用される式を指定します。|
|discountPercent               |decimal |請求金額の早期支払いに適用される割引率を指定します。|
|calculateDiscountOnCreditMemos|ブール値 |クレジットメモに割引を適用する必要があるかどうかを指定します。 **True**は割引が提供されることを示し、 **false**は割引が与えられないことを示します。|
|lastModifiedDateTime          |datetime|PaymentTerms が最後に変更された日時。 読み取り専用。|  


## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

PaymentTerms の JSON 表記を次に示します。


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
