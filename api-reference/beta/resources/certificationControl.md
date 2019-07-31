---
title: " certificationControl リソースの種類"
description: このリソースには、セキュリティで保護されたスコアコントロールに関連するコンプライアンス証明書データが含まれています。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 22dc12070a801988d814ba73c6bffe1414bb5218
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012997"
---
#  <a name="certificationcontrol-resource-type"></a>certificationControl リソースの種類

セキュリティで保護されたスコアコントロールに関連付けられたコンプライアンス証明書データを格納します。

|プロパティ |型 |説明 |
|:--|:--|:--|
|name | string | 証明書制御名 |
|url | string | Microsoft Service Trust Portal の URL |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificationControl"
}-->

```json
{
  "name": "String",
  "url": "Collection(microsoft.graph.certificationControl)"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "certificationControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
