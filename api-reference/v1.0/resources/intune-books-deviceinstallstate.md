---
title: deviceInstallState リソースの種類
description: デバイスのインストール状態のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6e737a58fc9547d54feeeeef47136286285c1e99
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565983"
---
# <a name="deviceinstallstate-resource-type"></a>deviceInstallState リソースの種類

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスのインストール状態のプロパティが含まれています。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceInstallStates のリスト](../api/intune-books-deviceinstallstate-list.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md) コレクション|[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[deviceInstallState の取得](../api/intune-books-deviceinstallstate-get.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceInstallState の作成](../api/intune-books-deviceinstallstate-create.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md)|新しい [deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトを作成します。|
|[deviceInstallState の削除](../api/intune-books-deviceinstallstate-delete.md)|なし|[deviceInstallState](../resources/intune-books-deviceinstallstate.md) を削除します。|
|[deviceInstallState の更新](../api/intune-books-deviceinstallstate-update.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|deviceName|String|デバイス名。|
|deviceId|String|デバイス ID。|
|lastSyncDateTime|DateTimeOffset|最後の同期日時。|
|installState|[installState](../resources/intune-books-installstate.md)|電子ブックのインストールの状態。 可能な値は、`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown` です。|
|errorCode|String|インストール失敗のエラー コード。|
|osVersion|String|OS バージョン。|
|osDescription|String|OS の説明。|
|userName|String|デバイスのユーザー名です。|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceInstallState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "installState": "String",
  "errorCode": "String",
  "osVersion": "String",
  "osDescription": "String",
  "userName": "String"
}
```



