---
title: genericError リソースの種類
description: 汎用エラー。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 701a3b7ed0d7bad6e33f8ba41e77ec7340a57146
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973528"
---
# <a name="genericerror-resource-type"></a>genericError リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

汎用エラー。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------|:-----|:------------|
| メッセージ​​ | String | エラー メッセージ。 |
| code | String | エラーコード。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.genericError"
}-->

```json
{
  "message": "String",
  "code": "String"
}
```
