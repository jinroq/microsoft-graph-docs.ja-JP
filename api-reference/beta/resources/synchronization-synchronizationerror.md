---
title: 同期エラーリソースの種類
description: 同期処理中に発生したエラーを表します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b48f1f47f343995b5cb7dc9ab3de4210a5249124
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620753"
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
