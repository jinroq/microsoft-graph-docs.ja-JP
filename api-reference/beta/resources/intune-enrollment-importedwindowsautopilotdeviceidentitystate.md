---
title: importedWindowsAutopilotDeviceIdentityState リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4f392f011f4bfcc615f88b6ea965fbc2b47899c9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941536"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a>importedWindowsAutopilotDeviceIdentityState リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|deviceImportStatus|[importedWindowsAutopilotDeviceIdentityImportStatus](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|Device Directory Service (DDS) から報告されたデバイスの状態です。 可能な値は、`unknown`、`pending`、`partial`、`complete`、`error` です。|
|deviceRegistrationId|String|正常に追加されたと Devce Directory Service (DDS) から報告されたデバイスの Devce Registration ID です。|
|deviceErrorCode|Int32|Device Directory Service (DDS) から報告されたデバイス エラー コードです。|
|deviceErrorName|String|Device Directory Service (DDS) から報告されたデバイス エラー名です。|

## <a name="relationships"></a>関係
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




