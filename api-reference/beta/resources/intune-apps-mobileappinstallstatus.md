---
title: mobileAppInstallStatus リソースの種類
description: デバイスのモバイル アプリケーションのインストール状態のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a81113001a1ff06b530b2b9249ee705b9cd5ac40
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880501"
---
# <a name="mobileappinstallstatus-resource-type"></a>mobileAppInstallStatus リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

デバイスのモバイル アプリケーションのインストール状態のプロパティが含まれています。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト mobileAppInstallStatuses](../api/intune-apps-mobileappinstallstatus-list.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)コレクション|[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトのプロパティと関係を一覧表示します。|
|[MobileAppInstallStatus を取得します。](../api/intune-apps-mobileappinstallstatus-get.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトのプロパティと関係を参照してください。|
|[MobileAppInstallStatus を作成します。](../api/intune-apps-mobileappinstallstatus-create.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|新しい[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトを作成します。|
|[MobileAppInstallStatus を削除します。](../api/intune-apps-mobileappinstallstatus-delete.md)|なし|の[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)を削除します。|
|[MobileAppInstallStatus を更新します。](../api/intune-apps-mobileappinstallstatus-update.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。|
|deviceName|String|デバイス名|
|deviceId|String|デバイス ID|
|lastSyncDateTime|DateTimeOffset|前回の同期日時|
|mobileAppInstallStatusValue|[resultantAppState](../resources/intune-shared-resultantappstate.md)|アプリケーションのインストール状態です。 可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。|
|installState|[resultantAppState](../resources/intune-shared-resultantappstate.md)|アプリケーションのインストール状態です。 可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。|
|installStateDetail|[resultantAppStateDetail](../resources/intune-apps-resultantappstatedetail.md)|アプリケーションのインストール状態の詳細。 可能な値は、`noAdditionalDetails`、`seeInstallErrorCode`、`seeUninstallErrorCode`、`pendingReboot`、`platformNotApplicable`、`minimumCpuSpeedNotMet`、`minimumLogicalProcessorCountNotMet`、`minimumPhysicalMemoryNotMet`、`minimumOsVersionNotMet`、`minimumDiskSpaceNotMet`、`processorArchitectureNotApplicable` です。|
|errorCode|Int32|エラーは、インストール用のコードか、障害をアンインストールします。|
|osVersion|String|OS のバージョン|
|osDescription|String|OS の説明|
|userName|String|デバイスのユーザー名|
|userPrincipalName|String|ユーザー プリンシパル名|
|displayVersion|String|人間の読み取り可能なバージョンのアプリケーション|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|アプリ|[mobileApp](../resources/intune-apps-mobileapp.md)|モバイル アプリケーションへのナビゲーション リンクです。|

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





