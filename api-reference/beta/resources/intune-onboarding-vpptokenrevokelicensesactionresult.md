---
title: vppTokenRevokeLicensesActionResult リソースの種類
description: 取り消しライセンスのステータスは、Apple ボリューム購入プログラムのトークンで実行されます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 75c75c6b8bcdc06ede0f71b19956155becc4d478
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418226"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a>vppTokenRevokeLicensesActionResult リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

取り消しライセンスのステータスは、Apple ボリューム購入プログラムのトークンで実行されます。


[VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|actionName|String|[VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)からアクション名継承|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|[VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)から継承される、アクションの状態です。 可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。|
|startDateTime|DateTimeOffset|アクションが開始された時刻[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)から継承されました。|
|lastUpdatedDateTime|DateTimeOffset|動作状態が最後に[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)からの継承の更新|
|totalLicensesCount|Int32|無効にしようとしていたライセンスの数のカウントです。|
|failedLicensesCount|Int32|取り消しに失敗したライセンスの数のカウントです。|
|actionFailureReason|[vppTokenActionFailureReason](../resources/intune-shared-vpptokenactionfailurereason.md)|取り消しライセンス操作が失敗した理由です。 可能な値は、`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate` です。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenRevokeLicensesActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024,
  "actionFailureReason": "String"
}
```




