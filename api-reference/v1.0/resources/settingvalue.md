---
title: settingValue リソースの種類
description: 名前と値の組で表される設定。
ms.openlocfilehash: b47c5c746117390cfd59db71d832928e482403b9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024285"
---
# <a name="settingvalue-resource-type"></a>settingValue リソースの種類

名前と値の組で表される設定。

### <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|名前|文字列| 設定の名前 ([groupSettingTemplate](groupsettingtemplate.md) によって定義されている)。 |
|値|文字列| 設定の値です。 |

### <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->