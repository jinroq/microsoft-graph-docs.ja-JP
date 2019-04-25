---
title: " complianceInformation リソースの種類"
description: このリソースには、セキュリティで保護されたスコアコントロールに関連するコンプライアンスデータが含まれています。
localization_priority: Normal
ms.openlocfilehash: 7a3968e6e043d2019100870061c5e34b03b1b8bd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543365"
---
#  <a name="complianceinformation-resource-type"></a>complianceInformation リソースの種類

セキュリティで保護されたスコアコントロールに関連するコンプライアンスデータが保存されています。

|プロパティ |型 |説明 |
|:--|:--|:--|
|certificationName | string | コンプライアンス証明書の名前 (たとえば、ISO 27018:2014、GDPR、fedramp、NIST 800-171) |
|certificationControls | [certificationControl](certificationcontrol.md)コレクション | 証明書に関連付けられている証明書コントロールのコレクション |

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
