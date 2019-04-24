---
title: customerPaymentJournals リソースの種類
description: Dynamics 365 Business Central の顧客支払仕訳帳。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: a8b01124db732866e1a7b971af57d7e0a2b692e1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507253"
---
# <a name="customerpaymentsjournals-resource-type"></a>customerPaymentsJournals リソースの種類
Dynamics 365 Business Central の顧客支払仕訳帳を表します。

## <a name="methods"></a>メソッド

| メソッド               | 戻り値の型             |説明                      |
|:---------------------|:------------------------|:--------------------------------|
|[customerPaymentJournals を取得する](../api/dynamics-customerpaymentsjournal-get.md)      |customerPaymentJournals|顧客支払仕訳帳を取得します。   |
|[Post customerPaymentJournals](../api/dynamics-create-customerpaymentsjournal.md)  |customerPaymentJournals|顧客支払仕訳帳を作成します。|
|[Patch customerPaymentJournals](../api/dynamics-customerpaymentsjournal-update.md) |customerPaymentJournals|顧客支払仕訳帳を更新します。|
|[customerPaymentJournals の削除](../api/dynamics-customerpaymentsjournal-delete.md)|なし                     |顧客支払仕訳帳を削除します。|

## <a name="properties"></a>プロパティ
| プロパティ           | 型                  |説明                                                             |
|:-------------------|:----------------------|:-----------------------------------------------------------------------|
|id                  |GUID                   |顧客支払仕訳帳の一意の ID。 編集できません。           |
|code                |文字列、最大サイズ10| 顧客支払仕訳帳のコード。                             |
|displayName         |文字列、最大サイズ50| 顧客支払仕訳帳の表示名。                     |
|lastModifiedDateTime|datetime               |顧客支払仕訳帳が最後に変更された日時。 読み取り専用。|

## <a name="relationships"></a>リレーションシップ

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。


```json
{
  "id": "GUID",
  "code": "String",
  "displayName": "String",
  "lastModifiedDateTime": "datetime"
}
```

