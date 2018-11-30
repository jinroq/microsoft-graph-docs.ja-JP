---
title: rgbColor リソースの種類
description: RGB 色。
ms.openlocfilehash: 5b3ef1f7b26925721098f82ec2bf54c614ce399b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024168"
---
# <a name="rgbcolor-resource-type"></a>rgbColor リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

RGB 色。
## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|r|バイト型 (Byte)|赤の値|
|g|バイト型 (Byte)|緑の値|
|b|バイト型 (Byte)|青の値|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rgbColor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rgbColor",
  "r": 1024,
  "g": 1024,
  "b": 1024
}
```



