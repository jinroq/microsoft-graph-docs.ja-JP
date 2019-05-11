---
title: mobileAppRelationshipState リソースの種類
description: UPN とデバイス id のコンテキストでの子アプリのインストール状態の詳細について説明します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 35080ad21137387fb63ff2fcb22233ff1be74cde
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949893"
---
# <a name="mobileapprelationshipstate-resource-type"></a>mobileAppRelationshipState リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

UPN とデバイス id のコンテキストでの子アプリのインストール状態の詳細について説明します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|sourceIds|String collection|送信元モバイルアプリの id のコレクション。|
|targetId|String|関連するターゲットアプリの id。|
|targetDisplayName|String|関連するターゲットアプリの表示名。|
|deviceId|String|対応するデバイス id。|
|installState|[Resultappstate](../resources/intune-shared-resultantappstate.md)|ターゲットアプリのアプリのインストール状態。 可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。|
|installStateDetail|[resultantAppStateDetail](../resources/intune-apps-resultantappstatedetail.md)|アプリのインストール状態の詳細。 可能な値: `noAdditionalDetails`、 `dependencyFailedToInstall` `dependencyWithRequirementsNotMet` `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `seeInstallErrorCode` `autoInstallDisabled` `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `powerShellScriptRequirementNotMet` `registryRequirementNotMet`、、、、、、、、、、、、 `fileSystemRequirementNotMet` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.|
|errorCode|Int32|ターゲットアプリのインストールまたはアンインストールに失敗した場合のエラーコード。|
|targetLastSyncDateTime|DateTimeOffset|ターゲットアプリの最終同期時刻。|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppRelationshipState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppRelationshipState",
  "sourceIds": [
    "String"
  ],
  "targetId": "String",
  "targetDisplayName": "String",
  "deviceId": "String",
  "installState": "String",
  "installStateDetail": "String",
  "errorCode": 1024,
  "targetLastSyncDateTime": "String (timestamp)"
}
```




