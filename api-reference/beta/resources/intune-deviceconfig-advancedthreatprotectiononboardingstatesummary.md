---
title: advancedThreatProtectionOnboardingStateSummary リソースの種類
description: Windows defender 脅威の高度な保護契約時の状態の概要アカウント間で。
ms.openlocfilehash: 8d870d51a7bb39bcc06472febd7d85f63b993a0a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072329"
---
# <a name="advancedthreatprotectiononboardingstatesummary-resource-type"></a>advancedThreatProtectionOnboardingStateSummary リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Windows defender 脅威の高度な保護契約時の状態の概要アカウント間で。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[AdvancedThreatProtectionOnboardingStateSummary を取得します。](../api/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary-get.md)|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|[AdvancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)オブジェクトのプロパティと関係を参照してください。|
|[AdvancedThreatProtectionOnboardingStateSummary を更新します。](../api/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary-update.md)|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|[AdvancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|一意識別子|
|unknownDeviceCount|Int32|不明なデバイスの数|
|notApplicableDeviceCount|Int32|該当しないデバイスの数|
|compliantDeviceCount|Int32|準拠デバイスの数|
|remediatedDeviceCount|Int32|修復済みデバイスの数|
|nonCompliantDeviceCount|Int32|準拠していないデバイスの数|
|errorDeviceCount|Int32|エラー デバイスの数|
|conflictDeviceCount|Int32|競合デバイスの数|
|notAssignedDeviceCount|Int32|割り当てられていないデバイスの数|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|advancedThreatProtectionOnboardingDeviceSettingStates|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)コレクション|まだ文書化されていません|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.advancedThreatProtectionOnboardingStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024,
  "notAssignedDeviceCount": 1024
}
```





