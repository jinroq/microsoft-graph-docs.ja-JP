---
title: " certificationControl リソースの種類"
description: このリソースには、コンプライアンスが含まれている証明書のデータに関連付けられているスコアのコントロールをセキュリティで保護します。
localization_priority: Normal
ms.openlocfilehash: 6f8269a85a8d3cb032f3e58457df95f4dd432c11
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810389"
---
#  <a name="certificationcontrol-resource-type"></a>certificationControl リソースの種類

コンプライアンスを含む証明書のデータに関連付けられているスコアのコントロールをセキュリティで保護します。

|プロパティ |種類 |説明 |
|:--|:--|:--|
|name | 文字列 | コントロールの名前を証明 |
|url | 文字列 | Microsoft サービスの URL は、ポータルを信頼します。 |

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
