---
title: deleteUserFromSharedAppleDeviceActionResult リソースの種類
description: 共有の Apple デバイスのアクションの結果からユーザーを削除する
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 997b9d9339abe44f8bc7427d9533b43066eac3b8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975457"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a>deleteUserFromSharedAppleDeviceActionResult リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

共有の Apple デバイスのアクションの結果からユーザーを削除する

[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承します

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|actionName|String|[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名|
|actionState|[actionState](../resources/intune-devices-actionstate.md)|[DeviceActionResult](../resources/intune-devices-deviceactionresult.md)から継承される、アクションの状態です。 可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。|
|startDateTime|DateTimeOffset|アクションが開始された時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)|
|lastUpdatedDateTime|DateTimeOffset|アクション状態の最終更新時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)|
|userPrincipalName|String|削除するユーザーのユーザー プリンシパル名|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deleteUserFromSharedAppleDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deleteUserFromSharedAppleDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```



