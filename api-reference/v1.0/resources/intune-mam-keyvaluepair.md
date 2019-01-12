---
title: keyValuePair リソースの種類
description: カスタム設定の保存用のキーと値のペア
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: db3e24c1c14cb208be66b7a2b0364ad12b162956
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926443"
---
# <a name="keyvaluepair-resource-type"></a>keyValuePair リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

カスタム設定の保存用のキーと値のペア
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
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



