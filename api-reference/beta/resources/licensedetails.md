---
title: licensedetails リソースの種類
description: ユーザーに割り当てられているライセンスに関する情報が含まれています。
localization_priority: Normal
ms.openlocfilehash: 6b977dcff67ac9dc03890a4f2182d8b1d974f314
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345304"
---
# <a name="licensedetails-resource-type"></a>licensedetails リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザーに割り当てられているライセンスに関する情報が含まれています。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[licenseDetails を一覧表示する](../api/user-list-licensedetails.md) | licenseDetails コレクション |ユーザーの licensedetails オブジェクトの一覧を取得します。|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| ライセンス詳細オブジェクトの一意識別子。 読み取り専用、キー、null 許容ではない |
|serviceplans|[servicePlanInfo](serviceplaninfo.md) コレクション| ライセンスで割り当てられているサービスプランに関する情報。 読み取り専用で、null 許容ではない |
|skuId|Guid| サービス SKU の一意識別子 (GUID)。 関連する[SubscribedSku](subscribedsku.md)オブジェクトの skuId プロパティと同じです。 読み取り専用 |
|skupartnumber|String| 一意の SKU 表示名。 関連する[SubscribedSku](subscribedsku.md)オブジェクトの skupartnumber と等しい。例: "AAD_Premium"。 読み取り専用 |

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseDetails"
}-->

```json
{
  "id": "String (identifier)",
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "Guid",
  "skuPartNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
