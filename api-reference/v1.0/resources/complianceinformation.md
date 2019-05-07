---
title: complianceInformation リソースの種類
description: このリソースには、セキュリティで保護されたスコアコントロールに関連するコンプライアンスデータが含まれています。
localization_priority: Normal
author: preetikr
ms.openlocfilehash: 85fef478a8dcc0f3196355d89f0a20ef0cd7a5b4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629307"
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
