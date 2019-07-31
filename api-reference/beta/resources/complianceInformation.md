---
title: " complianceInformation リソースの種類"
description: このリソースには、セキュリティで保護されたスコアコントロールに関連するコンプライアンスデータが含まれています。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: b93e01bf6274591282fd5e486bebb878672d8cc3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973231"
---
#  <a name="complianceinformation-resource-type"></a>complianceInformation リソースの種類

セキュリティで保護されたスコアコントロールに関連するコンプライアンスデータが保存されています。

|プロパティ |型 |説明 |
|:--|:--|:--|
|certificationName | string | コンプライアンス証明書の名前 (たとえば、ISO 27018:2014、GDPR、FedRAMP、NIST 800-171) |
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
