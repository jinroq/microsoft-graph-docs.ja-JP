---
title: settingTemplateValue リソースの種類
description: 設定がインスタンス化されていない場合に、設定の既定値を含む、個々のテンプレート設定の定義を表します。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f4ac39001e260d7f65b3a593d90976f94acd4693
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034392"
---
# <a name="settingtemplatevalue-resource-type"></a>settingTemplateValue リソースの種類

設定がインスタンス化されていない場合に、設定の既定値を含む、個々のテンプレート設定の定義を表します。

### <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|defaultValue|String| 設定の既定値。 |
|description|String| 設定の説明。 |
|name|String| 設定の名前。 |
|type|String| 設定の種類。 |

### <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "String",
  "description": "String",
  "name": "String",
  "type": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
