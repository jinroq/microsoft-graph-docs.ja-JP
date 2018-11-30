---
title: deviceInstallState リソースの種類
description: デバイスのインストール状態のプロパティが含まれています。
ms.openlocfilehash: 944cb57d397ffe7b75f0a378680b0f1468b10f49
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073022"
---
# <a name="deviceinstallstate-resource-type"></a>deviceInstallState リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

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





