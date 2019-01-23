---
title: deviceManagementExchangeAccessRule リソースの種類
description: Exchange でのデバイス アクセス ルールです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c46bff30bf5f88723a789bb13160bf5aedb1ef2a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409441"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a>deviceManagementExchangeAccessRule リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Exchange でのデバイス アクセス ルールです。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|deviceClass|[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|デバイス クラスはこの規則の影響を受けます。|
|accessLevel|[deviceManagementExchangeAccessLevel](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|この規則によって付与された Exchange のアクセス レベルです。 可能な値は、`none`、`allow`、`block`、`quarantine` です。|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeAccessRule",
  "deviceClass": {
    "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
    "name": "String",
    "type": "String"
  },
  "accessLevel": "String"
}
```




