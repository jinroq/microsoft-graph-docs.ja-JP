---
title: mobileAppInstallStatus リソースの種類
description: デバイス用のモバイルアプリのインストール状態のプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5bedb9308b414c4ea44c814c40dcd32ca33074d1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36322626"
---
# <a name="mobileappinstallstatus-resource-type"></a>mobileAppInstallStatus リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイス用のモバイルアプリのインストール状態のプロパティが含まれています。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト mobileAppInstallStatuses](../api/intune-apps-mobileappinstallstatus-list.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)コレクション|[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[MobileAppInstallStatus を取得する](../api/intune-apps-mobileappinstallstatus-get.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[MobileAppInstallStatus を作成する](../api/intune-apps-mobileappinstallstatus-create.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|新しい[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトを作成します。|
|[MobileAppInstallStatus の削除](../api/intune-apps-mobileappinstallstatus-delete.md)|None|[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)を削除します。|
|[MobileAppInstallStatus の更新](../api/intune-apps-mobileappinstallstatus-update.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。|
|deviceName|String|[デバイス名]|
|deviceId|String|デバイス ID|
|lastSyncDateTime|DateTimeOffset|最終同期日時|
|mobileAppInstallStatusValue|[Resultappstate](../resources/intune-shared-resultantappstate.md)|アプリのインストール状態。 可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。|
|installState|[Resultappstate](../resources/intune-shared-resultantappstate.md)|アプリのインストール状態。 可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。|
|installStateDetail|[resultantAppStateDetail](../resources/intune-apps-resultantappstatedetail.md)|アプリのインストール状態の詳細。 可能な値: `noAdditionalDetails`、 `dependencyFailedToInstall` `dependencyWithRequirementsNotMet` `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `seeInstallErrorCode` `autoInstallDisabled` `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `powerShellScriptRequirementNotMet` `registryRequirementNotMet`、、、、、、、、、、、、 `fileSystemRequirementNotMet` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.|
|errorCode|Int32|インストールまたはアンインストールの失敗のエラーコード。|
|osVersion|String|OS のバージョン|
|osDescription|String|OS の説明|
|userName|String|デバイスのユーザー名|
|userPrincipalName|String|ユーザー プリンシパル名|
|displayVersion|String|アプリケーションの人間の読み取り可能なバージョン|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|アプリ|[mobileApp](../resources/intune-apps-mobileapp.md)|モバイルアプリへのナビゲーションリンク。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppInstallStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "mobileAppInstallStatusValue": "String",
  "installState": "String",
  "installStateDetail": "String",
  "errorCode": 1024,
  "osVersion": "String",
  "osDescription": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "displayVersion": "String"
}
```



