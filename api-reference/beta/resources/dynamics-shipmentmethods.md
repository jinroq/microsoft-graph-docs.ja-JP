---
title: shipmentMethods リソースの種類
description: Dynamics 365 Business Central の出荷方法。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: e8d25294b219815c8aa569c7a8c7fab7ec68830c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006613"
---
# <a name="shipmentmethods-resource-type"></a>shipmentMethods リソースの種類
UPS、Fedex、DHL など、Dynamics 365 Business Central の出荷方法を表します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[ShipmentMethods を取得する](../api/dynamics-shipmentmethods-get.md)|shipmentMethods|送付方法を取得します。|
|[Post shipmentMethods](../api/dynamics-create-shipmentmethods.md)|shipmentMethods|送付方法を作成します。|
|[Patch shipmentMethods](../api/dynamics-shipmentmethods-update.md)|shipmentMethods|送付方法を更新します。|
|[ShipmentMethods の削除](../api/dynamics-shipmentmethods-delete.md)|none|送付方法を削除します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|GUID|ShipmentMethod の一意の ID。 編集できません。|
|code|string|送付方法のコードを指定します。|
|displayName|string|送付方法の表示名を指定します。|
|lastModifiedDateTime|datetime|出荷方法が最後に変更された日付です。 読み取り専用。|  


## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

ShipmentMethod の JSON 表記を次に示します。

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```


