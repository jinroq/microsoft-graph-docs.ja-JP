---
title: subscribedSku リソースの種類
description: " create、update、および delete はサポートされていません。 クエリのフィルター式はサポートされていません。 directoryObject から継承します。"
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4096860b3c45f525a57d208c6f70f1f1087d552d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345733"
---
# <a name="subscribedsku-resource-type"></a>subscribedSku リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

購読している SKU では読み取り操作のみがサポートされ、作成、更新、削除はサポートされません。クエリのフィルター式はサポートされていません。[directoryObject](directoryobject.md) から継承します。


## <a name="methods"></a>メソッド
| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[subscribedSku を取得する](../api/subscribedsku-get.md) | [subscribedSku](subscribedsku.md) |subscribedSku オブジェクトのプロパティとリレーションシップを読み取ります。|
|[リスト subscribedsku](../api/subscribedsku-list.md) | [subscribedSku](subscribedsku.md) コレクション |組織で取得した商用サブスクリプションの一覧を取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|appliesTo|String| "User" や "Company" など。 |
|capabilityStatus|String| たとえば、"有効" です。 |
|consumedUnits|Int32| 割り当てられたライセンスの数。 |
|id|String| 購読している SKU オブジェクトの一意識別子。 キー。 null 許容ではありません。 |
|prepaidUnits|[licenseUnitsDetail](licenseunitsdetail.md)| プリペイド ライセンスの数と状態に関する情報。 |
|serviceplans|[servicePlanInfo](serviceplaninfo.md) コレクション| SKU と併用できるサービス プランに関する情報。 null 許容ではない |
|skuId|Guid| サービス SKU の一意識別子 (GUID)。 |
|skupartnumber|String| SKU 部品番号。"AAD_PREMIUM" や "RMSBASIC" など。 |

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.subscribedSku"
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
<!--
{
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
