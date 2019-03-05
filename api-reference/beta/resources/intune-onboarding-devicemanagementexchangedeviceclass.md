---
title: devicemanagementexchangedeviceclass リソースの種類
description: Exchange のデバイスクラス。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ffa5f9c9f54722711a2e38116c2f2a3e03a3171e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149568"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a>devicemanagementexchangedeviceclass リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Exchange のデバイスクラス。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|name|String|このルールの影響を受けるデバイスクラスの名前。|
|type|[devicemanagementexchangeaccessruletype](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|このルールの影響を受けるデバイスの種類 (例: Model, Family)。 可能な値: `family`、`model`。|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeDeviceClass",
  "name": "String",
  "type": "String"
}
```




