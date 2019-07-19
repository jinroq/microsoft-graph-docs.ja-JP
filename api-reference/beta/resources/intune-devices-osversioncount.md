---
title: osVersionCount リソースの種類
description: 各 OS バージョンのマルウェアがあるデバイスの数
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d4b8987017012d4db0756fc3d8a78efe99319d68
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963913"
---
# <a name="osversioncount-resource-type"></a>osVersionCount リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

各 OS バージョンのマルウェアがあるデバイスの数

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|osVersion|String|OS のバージョン|
|deviceCount|Int32|OS バージョン用のマルウェアがあるデバイスの数|
|lastUpdateDateTime|DateTimeOffset|デバイス数の最終更新のタイムスタンプ (UTC)|

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





