---
title: vppTokenRevokeLicensesActionResult リソースの種類
description: 取り消しライセンスのステータスは、Apple ボリューム購入プログラムのトークンで実行されます。
author: tfitzmac
ms.openlocfilehash: a4188a269f9273b955fd29b32348dec82023b181
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351458"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a>vppTokenRevokeLicensesActionResult リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

取り消しライセンスのステータスは、Apple ボリューム購入プログラムのトークンで実行されます。

[VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)から継承します。

## <a name="properties"></a>Properties
|プロパティ|種類|説明|
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





