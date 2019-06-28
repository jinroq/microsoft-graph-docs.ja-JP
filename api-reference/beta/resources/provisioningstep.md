---
title: プロビジョニングステップリソースの種類
description: 'アクションを実行するために実行される手順について説明します。 '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1658114615c4532f0a7f9b9f5ad3c3a25deff81b
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349413"
---
# <a name="provisioningstep-resource-type"></a>プロビジョニングステップリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

アクションを実行するために実行される手順について説明します。

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|description|String|手順中に発生した処理の概要。|
|詳細|[詳細情報](detailsinfo.md)|手順中に発生した処理の詳細。|
|name|文字列|手順の名前を指定します。|
|/プロビジョニングの種類|String| 手順の種類。 可能な値は、`import`、`scoping`、`matching`、`processing`、`referenceResolution`、`export`、`unknownFutureValue` です。|
|status|String| 手順の状態。 使用可能な値は、`success`、`failure`、`skipped`、`unknownFutureValue` です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningStep",
  "baseType": null
}-->

```json
{
  "description": "String",
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "name": "String",
  "provisioningStepType": "String",
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningStep resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
