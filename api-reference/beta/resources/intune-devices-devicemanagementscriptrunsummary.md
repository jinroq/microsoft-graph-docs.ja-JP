---
title: deviceManagementScriptRunSummary リソースの種類
description: デバイス管理スクリプトの実行の概要のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b2109822ce081fc18286722cb48209a4349aa2b3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823542"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a>deviceManagementScriptRunSummary リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

デバイス管理スクリプトの実行の概要のプロパティが含まれています。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[DeviceManagementScriptRunSummary を取得します。](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|[DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)オブジェクトのプロパティと関係を参照してください。|
|[DeviceManagementScriptRunSummary を更新します。](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|[DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|デバイス管理スクリプトのキーは、エンティティの概要を実行します。|
|successDeviceCount|Int32|成功した場合のデバイスの数。|
|errorDeviceCount|Int32|デバイスのエラーの数です。|
|successUserCount|Int32|成功ユーザー カウントです。|
|errorUserCount|Int32|ユーザーのエラーの数です。|

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
  "successUserCount": 1024,
  "errorUserCount": 1024
}
```





