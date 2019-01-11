---
title: embeddedSIMDeviceState リソースの種類
description: デバイスに関連して埋め込み SIM アクティベーション コードの展開状態を説明します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 15e969037a93ee11c300f7b18b0c8afcb36d0ce1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881516"
---
# <a name="embeddedsimdevicestate-resource-type"></a>embeddedSIMDeviceState リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

デバイスに関連して埋め込み SIM アクティベーション コードの展開状態を説明します。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト embeddedSIMDeviceStates](../api/intune-esim-embeddedsimdevicestate-list.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)コレクション|[EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトのプロパティと関係を一覧表示します。|
|[EmbeddedSIMDeviceState を取得します。](../api/intune-esim-embeddedsimdevicestate-get.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|[EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトのプロパティと関係を参照してください。|
|[EmbeddedSIMDeviceState を作成します。](../api/intune-esim-embeddedsimdevicestate-create.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|新しい[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトを作成します。|
|[EmbeddedSIMDeviceState を削除します。](../api/intune-esim-embeddedsimdevicestate-delete.md)|なし|の[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)を削除します。|
|[EmbeddedSIMDeviceState を更新します。](../api/intune-esim-embeddedsimdevicestate-update.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|[EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|埋め込みの SIM のデバイスの状態の一意の識別子です。 システムでは、作成時に割り当てられた値が生成されます。|
|createdDateTime|DateTimeOffset|埋め込みの SIM のデバイスの状態が作成された時刻。 サービス側が生成されます。|
|変更された日時|DateTimeOffset|埋め込み SIM デバイスのステータスが最後に修正された時間です。 サービス側を更新します。|
|lastSyncDateTime|DateTimeOffset|SIM の埋め込みデバイスが最後にチェックインする時間です。 サービス側を更新します。|
|universalIntegratedCircuitCardIdentifier|String|汎用集積回路カードの識別子 (UICCID) を展開する先となるプロファイルは、ハードウェアを識別します。|
|deviceName|String|サブスクリプションには、デバイス名などのデスクトップでの準備|
|userName|String|サブスクリプションが joe@contoso.com などに準備されているユーザー名|
|state|[embeddedSIMDeviceStateValue](../resources/intune-esim-embeddedsimdevicestatevalue.md)|デバイスに適用されるプロファイルの操作の状態。 可能な値は、`notEvaluated`、`failed`、`installing`、`installed`、`deleting`、`error`、`deleted`、`removedByUser` です。|
|stateDetails|String|プロビジョニングの状態の説明の文字列を指定します。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.embeddedSIMDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "universalIntegratedCircuitCardIdentifier": "String",
  "deviceName": "String",
  "userName": "String",
  "state": "String",
  "stateDetails": "String"
}
```





