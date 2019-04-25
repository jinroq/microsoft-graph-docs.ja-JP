---
title: 通貨リソースの種類
description: Dynamics 365 Business Central の currency オブジェクト
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: c0d15b8d20e99537cb2f567a9f8fe12b45dbd389
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543071"
---
# <a name="currencies-resource-type"></a>通貨リソースの種類
Dynamics 365 Business Central で使用されている通貨を表します。

## <a name="methods"></a>メソッド
| メソッド                                                  |戻り値の型|説明       |
|:--------------------------------------------------------|:----------|:-----------------|
|[通貨を取得する](../api/dynamics-currencies-get.md)      |外貨 |通貨を取得します。   |
|[通貨の転記](../api/dynamics-create-currencies.md)  |外貨 |通貨を作成します。|
|[パッチ通貨](../api/dynamics-currencies-update.md) |外貨 |通貨を更新します。|
|[通貨を削除する](../api/dynamics-currencies-delete.md)|なし       |通貨を削除します。|

## <a name="properties"></a>プロパティ
| プロパティ              | 型   |説明                                                   |
|:----------------------|:-------|:-------------------------------------------------------------|
|id                     |GUID    |通貨の一意の ID です。 編集できません。                  |
|code                   |string  |通貨コードを指定します。                                  |
|displayName            |string  |通貨の表示名を指定します。                          |
|疑問符                 |string  |小切手に表示されるこの通貨の記号を指定します。|
|amountDecimalPlaces    |string  |この通貨の金額で、システムが表示される小数点以下の桁数を指定します。|
|amountRoundingPrecision|decimal |この通貨の金額を丸めるときに使用する間隔のサイズを指定します。|
|lastModifiedDateTime   |datetime|通貨が最後に変更された datetime。 読み取り専用。       |  


## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

以下は、通貨の JSON 表記です。


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "symbol": "string",
  "amountDecimalPlaces": "string",
  "amountRoundingPrecision": "decimal",
  "lastModifiedDateTime": "datetime"
}

```

