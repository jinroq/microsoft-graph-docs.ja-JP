---
title: paymentMethods リソースの種類
description: Dynamics 365 Business Central の支払い方法オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 08cfc864ee670a799a5f1672fa96cf8167ef1423
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006585"
---
# <a name="paymentmethods-resource-type"></a>paymentMethods リソースの種類
は、PayPal、クレジットカード、銀行口座など、Dynamics 365 Business Central の支払方法を表します。

## <a name="methods"></a>メソッド

| メソッド                                                          | 戻り値の型  |説明             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[PaymentMethods を取得する](../api/dynamics-paymentmethods-get.md)      |paymentMethods|支払い方法オブジェクトを取得します。   |
|[Post paymentMethods](../api/dynamics-create-paymentmethods.md)  |paymentMethods|支払い方法オブジェクトを作成します。|
|[Patch paymentMethods](../api/dynamics-paymentmethods-update.md) |paymentMethods|支払い方法オブジェクトを更新します。|
|[PaymentMethods の削除](../api/dynamics-paymentmethods-delete.md)|none          |支払い方法オブジェクトを削除します。|

## <a name="properties"></a>プロパティ
| プロパティ           | 型   |説明                                                  |
|:-------------------|:-------|:------------------------------------------------------------|
|id                  |GUID    |PaymentMethods の一意の ID。 編集できません。           |
|code                |string  |支払い方法のコードを指定します。                           |
|displayName         |string  |支払い方法の表示名を指定します。                   |
|lastModifiedDateTime|datetime|支払い方法が最後に変更された datetime。 読み取り専用。|  


## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

PaymentMethods の JSON 表記を次に示します。


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```
