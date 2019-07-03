---
title: statusDetails リソースの種類
description: プロビジョニングイベントとそれに関連するエラーの状態について説明します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 88880fbe88c0bd702eefeac5bed9668aac12a356
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455183"
---
# <a name="statusdetails-resource-type"></a>statusDetails リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

プロビジョニングイベントとそれに関連するエラーの状態について説明します。 [Statusbase](/graph/api/resources/statusbase?view=graph-rest-beta)から継承され、状態が "失敗" に設定されている場合にのみ使用されます。  

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|status|String|使用可能な値: `success`、`failure`、`skipped`、`unknownFutureValue`。 StatusBase から継承されます。|
|additionalDetails|String|エラーが発生した場合の追加情報。|
|errorCategory|String|エラーコードを分類します。|
|errorCode|String|エラーが発生した場合は、一意のエラーコード。|
|したがっ|String|状態の概要と、状態が発生した理由を説明します。|
|recommendedAction|String|対応するエラーの解決方法を示します。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.statusDetails",
  "baseType": "microsoft.graph.statusBase"
}-->

```json
{
  "status": "failure",
  "additionalDetails": "String",
  "errorCategory": "String",
  "errorCode": "String",
  "reason": "String",
  "recommendedAction": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "statusDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
