---
title: softwareUpdateStatusSummary リソースの種類
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: fcdf2045afbd22596a90596b2f171ef79f71e9fb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326510"
---
# <a name="softwareupdatestatussummary-resource-type"></a>softwareUpdateStatusSummary リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

まだ文書化されていません
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[Get softwareUpdateStatusSummary](../api/intune-deviceconfig-softwareupdatestatussummary-get.md)|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update softwareUpdateStatusSummary](../api/intune-deviceconfig-softwareupdatestatussummary-update.md)|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。|
|displayName|String|ポリシーの名前。|
|compliantDeviceCount|Int32|準拠デバイスの数。|
|nonCompliantDeviceCount|Int32|準拠していないデバイスの数。|
|remediatedDeviceCount|Int32|修復済みデバイスの数。|
|errorDeviceCount|Int32|エラーが発生したデバイスの数。|
|unknownDeviceCount|Int32|不明なデバイスの数。|
|conflictDeviceCount|Int32|競合デバイスの数。|
|notApplicableDeviceCount|Int32|該当しないデバイスの数。|
|compliantUserCount|Int32|準拠ユーザーの数。|
|nonCompliantUserCount|Int32|準拠していないユーザーの数。|
|remediatedUserCount|Int32|修復済みユーザーの数。|
|errorUserCount|Int32|エラーが発生したユーザーの数。|
|unknownUserCount|Int32|不明なユーザーの数。|
|conflictUserCount|Int32|競合ユーザーの数。|
|notApplicableUserCount|Int32|該当しないユーザーの数。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.softwareUpdateStatusSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "String (identifier)",
  "displayName": "String",
  "compliantDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "conflictDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantUserCount": 1024,
  "nonCompliantUserCount": 1024,
  "remediatedUserCount": 1024,
  "errorUserCount": 1024,
  "unknownUserCount": 1024,
  "conflictUserCount": 1024,
  "notApplicableUserCount": 1024
}
```





