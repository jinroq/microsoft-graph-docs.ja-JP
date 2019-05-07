---
title: certificationControl リソースの種類
description: このリソースには、セキュリティで保護されたスコアコントロールに関連するコンプライアンス証明書データが含まれています。
localization_priority: Normal
author: preetikr
ms.openlocfilehash: c92d129b6849898abe7202b9c2f539f26d2e1ebe
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629314"
---
#  <a name="certificationcontrol-resource-type"></a>certificationControl リソースの種類

セキュリティで保護されたスコアコントロールに関連付けられたコンプライアンス証明書データを格納します。

## <a name="properties"></a>プロパティ

|プロパティ |型 |説明 |
|:--|:--|:--|
|name|String|証明書制御名 |
|url|String|Microsoft Service Trust Portal の URL |

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
  "url": "String"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "certificationControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
