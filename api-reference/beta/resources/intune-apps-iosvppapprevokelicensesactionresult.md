---
title: iosVppAppRevokeLicensesActionResult リソースの種類
description: IOS Vpp アプリでのアクションの結果を定義します。 ActionResult の継承されたプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d9fce6d4a2a37aa5421fa7e0e173b9447db4be93
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34975967"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a>iosVppAppRevokeLicensesActionResult リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

IOS Vpp アプリでのアクションの結果を定義します。 ActionResult の継承されたプロパティが含まれています。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|userId|String|アクションに関連付けられている UserId。|
|managedDeviceId|String|アクションに関連付けられている DeviceId。|
|合計の合計数|Int32|取り消しが試行されたライセンスの数。|
|failedLicensesCount|Int32|失効に失敗したライセンスの数。|
|actionFailureReason|[vppTokenActionFailureReason](../resources/intune-shared-vpptokenactionfailurereason.md)|失効ライセンスの処理の失敗の理由。 可能な値は、`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate` です。|
|actionName|文字列型 (String)|アクション名|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|アクションの状態。 可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。|
|startDateTime|DateTimeOffset|アクションが開始された時刻|
|lastUpdatedDateTime|DateTimeOffset|アクション状態の最終更新時刻|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppRevokeLicensesActionResult",
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





