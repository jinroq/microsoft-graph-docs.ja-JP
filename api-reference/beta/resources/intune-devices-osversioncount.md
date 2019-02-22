---
title: osversioncount リソースの種類
description: 各 OS バージョンのマルウェアがあるデバイスの数
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 12ee68855f45ed6827f84a64084118c24081d266
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142750"
---
# <a name="osversioncount-resource-type"></a>osversioncount リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

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




