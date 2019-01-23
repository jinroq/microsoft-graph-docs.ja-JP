---
title: remoteActionAudit リソースの種類
description: 特定のテナントに属するデバイス上で初期化されたリモートの操作のレポートです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ebe93b2f2e70011fb75a08b91938f26d723d1d5c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404912"
---
# <a name="remoteactionaudit-resource-type"></a>remoteActionAudit リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

特定のテナントに属するデバイス上で初期化されたリモートの操作のレポートです。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト remoteActionAudits](../api/intune-devices-remoteactionaudit-list.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)コレクション|[RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトのプロパティと関係を一覧表示します。|
|[RemoteActionAudit を取得します。](../api/intune-devices-remoteactionaudit-get.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|[RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトのプロパティと関係を参照してください。|
|[RemoteActionAudit を作成します。](../api/intune-devices-remoteactionaudit-create.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|新しい[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトを作成します。|
|[RemoteActionAudit を削除します。](../api/intune-devices-remoteactionaudit-delete.md)|なし|の[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)を削除します。|
|[RemoteActionAudit を更新します。](../api/intune-devices-remoteactionaudit-update.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|[RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|レポートの id。|
|deviceDisplayName|String|Intune デバイスの名前です。|
|userName|String|\[推奨\]InitiatedByUserPrincipalName を代わりに使用してください。|
|initiatedByUserPrincipalName|String|デバイスのアクションを開始したユーザーは、UPN 形式です。|
|action|[remoteAction](../resources/intune-devices-remoteaction.md)|アクション名。 使用可能な値: `unknown`、 `factoryReset`、 `removeCompanyData`、 `resetPasscode`、 `remoteLock`、 `enableLostMode`、 `disableLostMode`、 `locateDevice`、 `rebootNow`、 `recoverPasscode`、 `cleanWindowsDevice`、 `logoutSharedAppleDeviceActiveUser`、 `quickScan`、 `fullScan`、 `windowsDefenderUpdateSignatures`、 `factoryResetKeepEnrollmentData`、 `updateDeviceAccount`、 `automaticRedeployment`、 `shutDown`.|
|requestDateTime|DateTimeOffset|UTC で指定されたアクションを発行した時の時間です。|
|deviceOwnerUserPrincipalName|String|デバイス所有者の Upn。|
|deviceIMEI|String|デバイスの IMEI。|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|動作状態です。 可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteActionAudit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "initiatedByUserPrincipalName": "String",
  "action": "String",
  "requestDateTime": "String (timestamp)",
  "deviceOwnerUserPrincipalName": "String",
  "deviceIMEI": "String",
  "actionState": "String"
}
```




