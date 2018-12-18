---
title: educationOrganization リソースの種類
description: 教育セクター内の別の組織の種類との間の共通性をモデル化するために使用する抽象エンティティです。
author: mmast-msft
ms.openlocfilehash: e4c0f69d63108cc88b88f530e99cbd55b23f49ed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326146"
---
# <a name="educationorganization-resource-type"></a>educationOrganization リソースの種類

教育セクター内の別の組織の種類との間の共通性をモデル化するために使用する抽象エンティティです。

## <a name="properties"></a>Properties
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|説明|String| 組織の説明です。|
|displayName|String| 組織の表示名です。|
|externalSource|educationExternalSource| この組織が作成されたソースです。 可能な値: `sis`、 `manual`、 `unknownFutureValue`。|

## <a name="relationships"></a>リレーションシップ
なし。


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->