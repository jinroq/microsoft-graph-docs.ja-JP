---
title: 同期エラーリソースの種類
description: 同期処理中に発生したエラーを表します。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2be415a127f7bcef030407be737bb9b48c8a116f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964670"
---
# <a name="synchronizationerror-resource-type"></a>同期エラーリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

同期処理中に発生したエラーを表します。

## <a name="properties"></a>プロパティ

<!-- Add descriptions for the properties. -->
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|code|String||
|message|String||
|tenantActionable 可能|Boolean||

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationError"
}-->

```json
{
  "code": "String",
  "message": "String",
  "tenantActionable": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
