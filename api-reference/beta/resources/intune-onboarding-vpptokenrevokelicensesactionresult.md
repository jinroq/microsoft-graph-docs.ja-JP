---
title: vppTokenRevokeLicensesActionResult リソースの種類
description: Apple ボリューム購入プログラムのトークンに対して実行された取り消しライセンス操作の状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4be11b14c51f7de9f03de6705a9b2cf71fc0c362
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369389"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a>vppTokenRevokeLicensesActionResult リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Apple ボリューム購入プログラムのトークンに対して実行された取り消しライセンス操作の状態。


[Vpptokenactionresult](../resources/intune-onboarding-vpptokenactionresult.md)から継承します

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|actionName|String|[Vpptokenactionresult](../resources/intune-onboarding-vpptokenactionresult.md)から継承されるアクション名|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|[Vpptokenactionresult](../resources/intune-onboarding-vpptokenactionresult.md)から継承されたアクションの状態。 可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。|
|startDateTime|DateTimeOffset|アクションが[Vpptokenactionresult](../resources/intune-onboarding-vpptokenactionresult.md)から継承された時刻|
|lastUpdatedDateTime|DateTimeOffset|アクション状態が最後に更新された時刻。 [Vpptokenactionresult](../resources/intune-onboarding-vpptokenactionresult.md)から継承|
|合計の合計数|Int32|失効しようとしたライセンスの数。|
|failedLicensesCount|Int32|失効に失敗したライセンスの数。|
|actionFailureReason|[vppTokenActionFailureReason](../resources/intune-shared-vpptokenactionfailurereason.md)|失効ライセンスの処理の失敗の理由。 可能な値は、`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate` です。|

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



