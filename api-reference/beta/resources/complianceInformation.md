---
title: " complianceInformation リソースの種類"
description: このリソースには、コンプライアンスが含まれているに関連付けられているデータは、スコアのコントロールをセキュリティで保護します。
ms.openlocfilehash: a32670c6d11d391834358b769ae938a67b3d8aad
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380960"
---
#  <a name="complianceinformation-resource-type"></a>complianceInformation リソースの種類

コンプライアンスが含まれているに関連付けられているデータは、スコアのコントロールをセキュリティで保護します。

|プロパティ |型 |説明 |
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
