---
title: resetPasscodeActionResult リソースの種類
description: パスコードのリセット アクションの結果
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 90a99b0ad365004365d65ffd7b428e540bcc00a9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949914"
---
# <a name="resetpasscodeactionresult-resource-type"></a>resetPasscodeActionResult リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

パスコードのリセット アクションの結果

[deviceActionResult](../resources/intune-devices-deviceactionresult.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|actionName|String|[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|[DeviceActionResult](../resources/intune-devices-deviceactionresult.md)から継承される、アクションの状態です。 可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。|
|startDateTime|DateTimeOffset|アクションが開始された時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)|
|lastUpdatedDateTime|DateTimeOffset|アクション状態の最終更新時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承|
|passcode|文字列型 (String)|デバイス用に新たに生成されたパスコード |

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resetPasscodeActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resetPasscodeActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "passcode": "String"
}
```





