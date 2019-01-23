---
title: macOsVppAppRevokeLicensesActionResult リソースの種類
description: ActionResult の継承されたプロパティが含まれています、MacOS Vpp のアプリケーションでの操作の結果を定義します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f90bd55476bbbb48ab3a4904886a67b217ab67b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430282"
---
# <a name="macosvppapprevokelicensesactionresult-resource-type"></a>macOsVppAppRevokeLicensesActionResult リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ActionResult の継承されたプロパティが含まれています、MacOS Vpp のアプリケーションでの操作の結果を定義します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|userId|String|アクションに関連付けられているユーザーの Id。|
|managedDeviceId|String|DeviceId はアクションに関連付けられています。|
|totalLicensesCount|Int32|取り消しが実行しようとするライセンス数のカウントです。|
|failedLicensesCount|Int32|失敗する revoke のライセンス数のカウントです。|
|actionFailureReason|[vppTokenActionFailureReason](../resources/intune-shared-vpptokenactionfailurereason.md)|取り消しライセンス操作が失敗した理由です。 可能な値は、`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate` です。|
|actionName|文字列型 (String)|アクション名|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|アクションの状態です。 可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。|
|startDateTime|DateTimeOffset|アクションが開始された時刻|
|lastUpdatedDateTime|DateTimeOffset|アクション状態の最終更新時刻|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppRevokeLicensesActionResult",
  "userId": "String",
  "managedDeviceId": "String",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024,
  "actionFailureReason": "String",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```




