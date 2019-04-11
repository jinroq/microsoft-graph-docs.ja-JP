---
title: embeddedSIMDeviceState リソースの種類
description: デバイスに関して埋め込まれた SIM ライセンス認証コードの展開状態を記述します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8cd14c92e5619cbce071190b966d3274386cec89
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31804369"
---
# <a name="embeddedsimdevicestate-resource-type"></a>embeddedSIMDeviceState リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスに関して埋め込まれた SIM ライセンス認証コードの展開状態を記述します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト embeddedSIMDeviceStates](../api/intune-esim-embeddedsimdevicestate-list.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)コレクション|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[embeddedSIMDeviceState を取得する](../api/intune-esim-embeddedsimdevicestate-get.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[embeddedSIMDeviceState を作成する](../api/intune-esim-embeddedsimdevicestate-create.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|新しい[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトを作成します。|
|[embeddedSIMDeviceState の削除](../api/intune-esim-embeddedsimdevicestate-delete.md)|なし|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)を削除します。|
|[embeddedSIMDeviceState の更新](../api/intune-esim-embeddedsimdevicestate-update.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|埋め込まれている SIM デバイスの状態を表す一意の識別子です。 作成時に割り当てられたシステム生成値。|
|createdDateTime|DateTimeOffset|埋め込み SIM デバイスの状態が作成された時刻。 サービス側を生成しました。|
|modifiedDateTime|DateTimeOffset|埋め込み SIM デバイスの状態が最後に変更された時刻。 サービス側を更新しました。|
|lastSyncDateTime|DateTimeOffset|埋め込まれた SIM デバイスが最後にチェックインされた時刻。 サービス側を更新しました。|
|universalIntegratedCircuitCardIdentifier|文字列|プロファイルが展開されるハードウェアを識別するユニバーサル統合回路カード識別子 (UICCID)。|
|deviceName|文字列|サブスクリプションが準備されたデバイス名 (デスクトップの例: JOE)|
|userName|String|サブスクリプションが準備されたユーザー名 (例:)joe@contoso.com|
|state|[embeddedSIMDeviceStateValue](../resources/intune-esim-embeddedsimdevicestatevalue.md)|デバイスに適用されるプロファイル操作の状態。 可能な値は、`notEvaluated`、`failed`、`installing`、`installed`、`deleting`、`error`、`deleted`、`removedByUser` です。|
|statedetails|文字列|プロビジョニング状態の文字列の説明。|

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





