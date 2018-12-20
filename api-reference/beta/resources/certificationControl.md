---
title: " certificationControl リソースの種類"
description: このリソースには、コンプライアンスが含まれている証明書のデータに関連付けられているスコアのコントロールをセキュリティで保護します。
ms.openlocfilehash: 62b6627a9bb1a012d6d7e542d87abbaddb0e279a
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380946"
---
#  <a name="certificationcontrol-resource-type"></a>certificationControl リソースの種類

コンプライアンスを含む証明書のデータに関連付けられているスコアのコントロールをセキュリティで保護します。

|プロパティ |型 |説明 |
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
