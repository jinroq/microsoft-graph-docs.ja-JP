---
title: keyValuePair リソースの種類
description: カスタム設定の保存用のキーと値のペア
ms.openlocfilehash: 803dd9e347ef06bc9d4a9fce13d2265c4fc969a3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023388"
---
# <a name="keyvaluepair-resource-type"></a>keyValuePair リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

カスタム設定の保存用のキーと値のペア
## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|名前|文字列|キーと値のペアの名前|
|value|文字列|キーと値のペアの値|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValuePair",
  "name": "String",
  "value": "String"
}
```



