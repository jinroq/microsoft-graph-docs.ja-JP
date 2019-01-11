---
title: " complianceInformation リソースの種類"
description: このリソースには、コンプライアンスが含まれているに関連付けられているデータは、スコアのコントロールをセキュリティで保護します。
localization_priority: Normal
ms.openlocfilehash: 7a3968e6e043d2019100870061c5e34b03b1b8bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820602"
---
#  <a name="complianceinformation-resource-type"></a>complianceInformation リソースの種類

コンプライアンスが含まれているに関連付けられているデータは、スコアのコントロールをセキュリティで保護します。

|プロパティ |種類 |説明 |
|:--|:--|:--|
|certificationName | 文字列 | コンプライアンスの証明書の名前 (たとえば、ISO 27018:2014、GDPR、FedRAMP、NIST 800-171) |
|certificationControls | [certificationControl](certificationcontrol.md)コレクション | 証明書に関連付けられている証明書のコントロールのコレクション |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.complianceInformation"
}-->

```json
{
  "certificationName": "String",
  "certificationControls": "Collection(microsoft.graph.complianceInformation)"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "complianceInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
