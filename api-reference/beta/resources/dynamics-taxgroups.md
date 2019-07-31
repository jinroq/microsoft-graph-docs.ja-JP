---
title: taxGroups リソースの種類
description: Dynamics 365 Business Central の税グループオブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 378d8c1d773eacb3339eba35d5d60cc7ef5f2400
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006606"
---
# <a name="taxgroups-resource-type"></a>taxGroups リソースの種類
Dynamics 365 Business Central の taxGroups リソースの種類を表します。

## <a name="methods"></a>メソッド
| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[TaxGroups を取得する](../api/dynamics-taxgroups-get.md)|taxGroups|税グループオブジェクトを取得します。|
|[Post taxGroups](../api/dynamics-create-taxgroups.md)|taxGroups|税グループオブジェクトを作成します。|
|[Patch taxGroups](../api/dynamics-taxgroups-update.md)|taxGroups|税グループオブジェクトを更新します。|
|[TaxGroups の削除](../api/dynamics-taxgroups-delete.md)|none|税グループオブジェクトを削除します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|GUID|TaxGroup の一意の ID。 読み取り専用です。|
|code|string|税グループを指定します。|
|displayName|string|税グループの表示名を指定します。|
|taxType|string|グループの税の種類を指定します。|
|lastModifiedDateTime|datetime|税グループが最後に変更された日付です。 読み取り専用。|  


## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

TaxGroup の JSON 表記を次に示します。

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "taxType": "string",
  "lastModifiedDateTime": "datetime"
}

```


