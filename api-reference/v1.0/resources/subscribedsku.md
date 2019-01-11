---
title: subscribedSku リソースの種類
description: 会社が購読しているサービス SKU に関する情報が含まれています。
localization_priority: Normal
ms.openlocfilehash: 17290890ff27fded1aaf5d7fdb2c0cdacee09b0c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873718"
---
# <a name="subscribedsku-resource-type"></a>subscribedSku リソースの種類

会社が購読しているサービス SKU に関する情報が含まれています。

購読している SKU では読み取り操作のみがサポートされ、作成、更新、削除はサポートされません。クエリのフィルター式はサポートされていません。[directoryObject](directoryobject.md) から継承します。

## <a name="methods"></a>メソッド
| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[subscribedSku を取得する](../api/subscribedsku-get.md) | [subscribedSku](subscribedsku.md) |subscribedSku オブジェクトのプロパティとリレーションシップを読み取ります。|
|[リスト subscribedsku](../api/subscribedsku-list.md) | [subscribedSku](subscribedsku.md) コレクション |組織で取得した商用サブスクリプションの一覧を取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|appliesTo|String| "User" や "Company" など。 |
|capabilityStatus|String| 「有効」など。 |
|consumedUnits|Int32| 割り当てられたライセンスの数。 |
|id|String| 購読している SKU オブジェクトの一意識別子。キーであり、null 許容ではありません。 |
|prepaidUnits|[licenseUnitsDetail](licenseunitsdetail.md)| プリペイド ライセンスの数と状態に関する情報。 |
|servicePlans|[servicePlanInfo](serviceplaninfo.md) コレクション| SKU と併用できるサービス プランに関する情報。null 許容ではありません |
|skuId|Guid| サービス SKU の一意識別子 (GUID)。 |
|skuPartNumber|String| SKU 部品番号。"AAD_PREMIUM" や "RMSBASIC" など。 |

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.subscribedSku",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "toppable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
  "appliesTo": "string",
  "capabilityStatus": "string",
  "consumedUnits": 1024,
  "id": "string (identifier)",
  "prepaidUnits": {"@odata.type": "microsoft.graph.licenseUnitsDetail"},
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "guid",
  "skuPartNumber": "string"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
