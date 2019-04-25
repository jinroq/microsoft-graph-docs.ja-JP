---
title: settingtemplatevalue リソースの種類
description: 設定がインスタンス化されていない場合に、設定の既定値を含む、個々のテンプレート設定の定義を表します。
localization_priority: Normal
ms.openlocfilehash: 0cb3376177e3a4efcae54a591a083914db6b56d7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549693"
---
# <a name="settingtemplatevalue-resource-type"></a>settingtemplatevalue リソースの種類

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
