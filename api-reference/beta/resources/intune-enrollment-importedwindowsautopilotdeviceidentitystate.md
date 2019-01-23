---
title: importedWindowsAutopilotDeviceIdentityState リソースの種類
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0f4e76b23d4d970a9fb873326dc84f278aa2ed2b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410967"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a>importedWindowsAutopilotDeviceIdentityState リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|deviceImportStatus|[importedWindowsAutopilotDeviceIdentityImportStatus](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|Device Directory Service (DDS) から報告されたデバイスの状態です。 可能な値は、`unknown`、`pending`、`partial`、`complete`、`error` です。|
|deviceRegistrationId|String|正常に追加されたと Devce Directory Service (DDS) から報告されたデバイスの Devce Registration ID です。|
|deviceErrorCode|Int32|Device Directory Service (DDS) から報告されたデバイス エラー コードです。|
|deviceErrorName|String|Device Directory Service (DDS) から報告されたデバイス エラー名です。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
  "deviceImportStatus": "String",
  "deviceRegistrationId": "String",
  "deviceErrorCode": 1024,
  "deviceErrorName": "String"
}
```




