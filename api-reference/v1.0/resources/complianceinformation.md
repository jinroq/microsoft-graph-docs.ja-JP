---
title: complianceInformation リソースの種類
description: このリソースには、セキュリティで保護されたスコアコントロールに関連するコンプライアンスデータが含まれています。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9fc47940b8a9f249e66092ee016453a9eb5152ca
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032859"
---
#  <a name="complianceinformation-resource-type"></a>complianceInformation リソースの種類

セキュリティで保護されたスコアコントロールに関連するコンプライアンスデータが保存されています。

## <a name="properties"></a>プロパティ

|プロパティ |型 |説明 |
|:--|:--|:--|
|certificationName|String| コンプライアンス証明書の名前 (たとえば、ISO 27018:2014、GDPR、FedRAMP、NIST 800-171) |
|certificationControls|[certificationControl](certificationcontrol.md)コレクション|証明書に関連付けられている証明書コントロールのコレクション|

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
  "certificationControls": [{"@odata.type": "microsoft.graph.certificationControl"}]
}

```


<!-- {
  "type": "#page.annotation",
  "description": "complianceInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
