---
title: osVersionCount リソースの種類
description: 各オペレーティング システムのバージョンのマルウェアとデバイスの数
author: tfitzmac
ms.openlocfilehash: ccc031c6060604b36166b4869d02f08854dfdd2c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331998"
---
# <a name="osversioncount-resource-type"></a>osVersionCount リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

各オペレーティング システムのバージョンのマルウェアとデバイスの数
## <a name="properties"></a>Properties
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





