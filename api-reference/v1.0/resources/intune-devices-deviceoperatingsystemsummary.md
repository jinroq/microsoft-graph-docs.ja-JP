---
title: deviceOperatingSystemSummary リソースの種類
description: デバイスのオペレーティング システムの概要。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 53c806e250d6b201e6dfe49d90685c4144913182
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574076"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a>deviceOperatingSystemSummary リソースの種類

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスのオペレーティング システムの要約です。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|androidCount|Int32|Android デバイスの数です。|
|iosCount|Int32|iOS デバイスの数です。|
|macOSCount|Int32|Mac OS X デバイスの数です。|
|windowsMobileCount|Int32|Windows Mobile デバイスの数です。|
|windowsCount|Int32|Windows デバイスの数です。|
|unknownCount|Int32|不明なデバイスの数です。|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
  "androidCount": 1024,
  "iosCount": 1024,
  "macOSCount": 1024,
  "windowsMobileCount": 1024,
  "windowsCount": 1024,
  "unknownCount": 1024
}
```



