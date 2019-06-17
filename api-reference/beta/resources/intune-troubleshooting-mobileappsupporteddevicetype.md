---
title: mobileAppSupportedDeviceType リソースの種類
description: デバイスのプロパティ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6e757596be1ffbcb93c48f0a3d450e57c94641dd
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34988133"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a>mobileAppSupportedDeviceType リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスのプロパティ

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|type|[deviceType](../resources/intune-shared-devicetype.md)|デバイスの種類。 可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.|
|minimumOperatingSystemVersion|String|最小 OS バージョン|
|最大化 Umoper/Systemversion|String|最大 OS バージョン|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppSupportedDeviceType",
  "type": "String",
  "minimumOperatingSystemVersion": "String",
  "maximumOperatingSystemVersion": "String"
}
```





