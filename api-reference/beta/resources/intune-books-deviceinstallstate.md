---
title: deviceInstallState リソースの種類
description: デバイスのインストール状態のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bd0fb8d9f73cf19c4bd2b8be0e6ff40c8247b247
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782675"
---
# <a name="deviceinstallstate-resource-type"></a>deviceInstallState リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスのインストール状態のプロパティが含まれています。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceInstallStates のリスト](../api/intune-books-deviceinstallstate-list.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md) コレクション|[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get deviceInstallState](../api/intune-books-deviceinstallstate-get.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceInstallState の作成](../api/intune-books-deviceinstallstate-create.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md)|新しい [deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトを作成します。|
|[Delete deviceInstallState](../api/intune-books-deviceinstallstate-delete.md)|なし|[deviceInstallState](../resources/intune-books-deviceinstallstate.md) を削除します。|
|[deviceInstallState の更新](../api/intune-books-deviceinstallstate-update.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|deviceName|文字列|デバイス名。|
|deviceId|文字列|デバイス ID。|
|lastSyncDateTime|DateTimeOffset|最後の同期日時。|
|installState|[installState](../resources/intune-books-installstate.md)|電子ブックのインストールの状態。 可能な値は、`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown` です。|
|errorCode|文字列|インストール失敗のエラー コード。|
|osVersion|文字列|OS バージョン。|
|osDescription|文字列|OS の説明。|
|userName|String|デバイスのユーザー名です。|

## <a name="relationships"></a>リレーションシップ
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





