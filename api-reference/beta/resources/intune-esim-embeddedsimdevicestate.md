---
title: embeddedSIMDeviceState リソースの種類
description: デバイスに関して埋め込まれた SIM ライセンス認証コードの展開状態を記述します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 697517ffd5f7ab3aee99e39914554cc445a43bd7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011149"
---
# <a name="embeddedsimdevicestate-resource-type"></a>embeddedSIMDeviceState リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスに関して埋め込まれた SIM ライセンス認証コードの展開状態を記述します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト embeddedSIMDeviceStates](../api/intune-esim-embeddedsimdevicestate-list.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)コレクション|[EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[EmbeddedSIMDeviceState を取得する](../api/intune-esim-embeddedsimdevicestate-get.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|[EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[EmbeddedSIMDeviceState を作成する](../api/intune-esim-embeddedsimdevicestate-create.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|新しい[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトを作成します。|
|[EmbeddedSIMDeviceState の削除](../api/intune-esim-embeddedsimdevicestate-delete.md)|None|[EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)を削除します。|
|[EmbeddedSIMDeviceState の更新](../api/intune-esim-embeddedsimdevicestate-update.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|[EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|埋め込まれている SIM デバイスの状態を表す一意の識別子です。 作成時に割り当てられたシステム生成値。|
|createdDateTime|DateTimeOffset|埋め込み SIM デバイスの状態が作成された時刻。 サービス側を生成しました。|
|modifiedDateTime|DateTimeOffset|埋め込み SIM デバイスの状態が最後に変更された時刻。 サービス側を更新しました。|
|lastSyncDateTime|DateTimeOffset|埋め込まれた SIM デバイスが最後にチェックインされた時刻。 サービス側を更新しました。|
|universalIntegratedCircuitCardIdentifier|String|プロファイルが展開されるハードウェアを識別するユニバーサル統合回路カード識別子 (UICCID)。|
|deviceName|String|サブスクリプションが準備されたデバイス名 (デスクトップの例: JOE)|
|userName|String|サブスクリプションが準備されたユーザー名 (joe@contoso.com など)|
|state|[embeddedSIMDeviceStateValue](../resources/intune-esim-embeddedsimdevicestatevalue.md)|デバイスに適用されるプロファイル操作の状態。 可能な値は、`notEvaluated`、`failed`、`installing`、`installed`、`deleting`、`error`、`deleted`、`removedByUser` です。|
|stateDetails|String|プロビジョニング状態の文字列の説明。|

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





