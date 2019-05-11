---
title: managedDeviceCleanupSettings リソースの種類
description: 管理者がデバイスをクリーンアップする必要がある場合は、ルールを定義します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5070de01324b25332d42b63a4d1d787989b86c4f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941962"
---
# <a name="manageddevicecleanupsettings-resource-type"></a>managedDeviceCleanupSettings リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

管理者がデバイスをクリーンアップする必要がある場合は、ルールを定義します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|deviceInactivityBeforeRetirementInDays|String|デバイスが Intune に接続していない場合の日数。|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceCleanupSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceCleanupSettings",
  "deviceInactivityBeforeRetirementInDays": "String"
}
```




