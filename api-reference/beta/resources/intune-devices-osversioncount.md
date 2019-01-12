---
title: osVersionCount リソースの種類
description: 各オペレーティング システムのバージョンのマルウェアとデバイスの数
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: de841e679ede22492d26f2a1587e775179c45761
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911841"
---
# <a name="osversioncount-resource-type"></a>osVersionCount リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

各オペレーティング システムのバージョンのマルウェアとデバイスの数
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|osVersion|String|OS のバージョン|
|deviceCount|Int32|OS のバージョンのマルウェアとデバイスの数|
|lastUpdateDateTime|DateTimeOffset|デバイスの最後の更新のタイムスタンプは UTC でカウントします。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.osVersionCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.osVersionCount",
  "osVersion": "String",
  "deviceCount": 1024,
  "lastUpdateDateTime": "String (timestamp)"
}
```





