---
title: deviceManagementScriptRunSummary リソースの種類
description: デバイス管理スクリプトの実行の概要のプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e9d2b0b92287a045607c02e271155e2e74a2fa90
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370026"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a>deviceManagementScriptRunSummary リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイス管理スクリプトの実行の概要のプロパティが含まれています。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[DeviceManagementScriptRunSummary を取得する](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|[DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[DeviceManagementScriptRunSummary の更新](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|[DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|デバイス管理スクリプト実行の概要エンティティのキー。|
|successDeviceCount|Int32|成功したデバイス数。|
|errorDeviceCount|Int32|エラーデバイス数。|
|compliantDeviceCount|Int32|準拠しているデバイスの数。|
|notCompliantDeviceCount|Int32|準拠していないデバイス数。|
|pendingDeviceCount|Int32|保留中のデバイス数。|
|successUserCount|Int32|成功したユーザー数。|
|errorUserCount|Int32|エラーユーザー数。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "id": "String (identifier)",
  "successDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "notCompliantDeviceCount": 1024,
  "pendingDeviceCount": 1024,
  "successUserCount": 1024,
  "errorUserCount": 1024
}
```



