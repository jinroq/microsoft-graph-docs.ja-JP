---
title: vppTokenRevokeLicensesActionResult リソースの種類
description: Apple ボリューム購入プログラムのトークンに対して実行された取り消しライセンス操作の状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 432419f337750362256140b8d13a1841b49907d4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566466"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a>vppTokenRevokeLicensesActionResult リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Apple ボリューム購入プログラムのトークンに対して実行された取り消しライセンス操作の状態。


[vpptokenactionresult](../resources/intune-onboarding-vpptokenactionresult.md)から継承します

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|actionName|String|[vpptokenactionresult](../resources/intune-onboarding-vpptokenactionresult.md)から継承されるアクション名|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|[vpptokenactionresult](../resources/intune-onboarding-vpptokenactionresult.md)から継承されたアクションの状態。 可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。|
|startDateTime|DateTimeOffset|アクションが[vpptokenactionresult](../resources/intune-onboarding-vpptokenactionresult.md)から継承された時刻|
|lastUpdatedDateTime|DateTimeOffset|アクション状態が最後に更新された時刻。 [vpptokenactionresult](../resources/intune-onboarding-vpptokenactionresult.md)から継承|
|合計の合計数|Int32|失効しようとしたライセンスの数。|
|failedLicensesCount|Int32|失効に失敗したライセンスの数。|
|actionFailureReason|[vppTokenActionFailureReason](../resources/intune-shared-vpptokenactionfailurereason.md)|失効ライセンスの処理の失敗の理由。 可能な値は、`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate` です。|

## <a name="relationships"></a>関係
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





