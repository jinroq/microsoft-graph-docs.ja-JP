---
title: remoteActionAudit リソースの種類
description: 特定のテナントに属するデバイスで開始されたリモートアクションのレポート。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cb00a4d1d160fe4afdfa5c466b3b23e10c693c09
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372112"
---
# <a name="remoteactionaudit-resource-type"></a>remoteActionAudit リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

特定のテナントに属するデバイスで開始されたリモートアクションのレポート。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[RemoteActionAudits を一覧表示する](../api/intune-devices-remoteactionaudit-list.md)|[Remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)コレクション|[Remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[RemoteActionAudit の取得](../api/intune-devices-remoteactionaudit-get.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|[Remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[RemoteActionAudit の作成](../api/intune-devices-remoteactionaudit-create.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|新しい[Remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトを作成します。|
|[RemoteActionAudit の削除](../api/intune-devices-remoteactionaudit-delete.md)|None|[Remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)を削除します。|
|[RemoteActionAudit の更新](../api/intune-devices-remoteactionaudit-update.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|[Remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|レポート Id。|
|deviceDisplayName|String|Intune デバイス名。|
|userName|文字列型 (String)|\[非\]推奨 InitiatedByUserPrincipalName を代わりに使用してください。|
|initiatedByUserPrincipalName|String|デバイスのアクションを開始したユーザーの形式は UPN です。|
|action|[remoteAction](../resources/intune-devices-remoteaction.md)|アクション名。 可能な値: `unknown`、 `factoryReset` `removeCompanyData` `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `locateDevice` `rebootNow` `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser`、、、、、、、、、、、、 `quickScan` `fullScan` `windowsDefenderUpdateSignatures` `factoryResetKeepEnrollmentData` `updateDeviceAccount` `automaticRedeployment` `shutDown`, `rotateFileVaultKey`, `getFileVaultKey`, `setDeviceName`.|
|requestDateTime|DateTimeOffset|アクションが発行された日時 (UTC)。|
|deviceOwnerUserPrincipalName|String|デバイス所有者の Upn。|
|deviceIMEI|String|デバイスの IMEI。|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|アクションの状態。 可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。|
|managedDeviceId|String|アクションのターゲット。|

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
  "actionState": "String",
  "managedDeviceId": "String"
}
```



