---
title: settingtemplatevalue リソースの種類
description: 設定がインスタンス化されていない場合に、設定の既定値を含む、個々のテンプレート設定の定義を表します。
localization_priority: Normal
ms.openlocfilehash: 2277f4b7bb66839164a1b09011d20886baf2bd1f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343186"
---
# <a name="settingtemplatevalue-resource-type"></a>settingtemplatevalue リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

設定がインスタンス化されていない場合に、設定の既定値を含む、個々のテンプレート設定の定義を表します。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|defaultValue|string|設定の既定値。 読み取り専用です。|
|説明|string|設定の説明。 読み取り専用。|
|name|string|設定の名前。 値の取得のみ可能です。|
|type|string|設定の種類。 読み取り専用です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "string",
  "description": "string",
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
