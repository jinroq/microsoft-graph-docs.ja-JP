---
title: revokeAppleVppLicensesActionResult リソースの種類
description: アップル Vpp ライセンスのアクションの結果を取り消す
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b7e578ee695e171a1a91167b61e47af717dd82c0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879101"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a>revokeAppleVppLicensesActionResult リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

アップル Vpp ライセンスのアクションの結果を取り消す

[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承します

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|actionName|String|[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|[DeviceActionResult](../resources/intune-devices-deviceactionresult.md)から継承される、アクションの状態です。 可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。|
|startDateTime|DateTimeOffset|アクションが開始された時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)|
|lastUpdatedDateTime|DateTimeOffset|アクション状態の最終更新時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)|
|totalLicensesCount|Int32|関連付けられている Apple Vpp ライセンスの合計数|
|failedLicensesCount|Int32|アップル Vpp ライセンスを失効に失敗した数の合計|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.revokeAppleVppLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.revokeAppleVppLicensesActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024
}
```





