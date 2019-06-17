---
title: mobileAppIntentAndStateDetail リソースの種類
description: 特定のデバイスのモバイルアプリの意図とインストール状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 99374d098d103b9a9898f10ea105ab41ca7bef41
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34988077"
---
# <a name="mobileappintentandstatedetail-resource-type"></a>mobileAppIntentAndStateDetail リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

特定のデバイスのモバイルアプリの意図とインストール状態。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|applicationId|文字列型 (String)|MobieApp 識別子。|
|displayName|String|管理者が提供またはインポートしたアプリのタイトル。|
|mobileAppIntent|[mobileAppIntent](../resources/intune-troubleshooting-mobileappintent.md)|モバイルアプリの目的。 可能な値は、`available`、`notAvailable`、`requiredInstall`、`requiredUninstall`、`requiredAndAvailableInstall`、`availableInstallWithoutEnrollment`、`exclude` です。|
|displayVersion|String|アプリケーションの人間の読み取り可能なバージョン|
|installState|[Resultappstate](../resources/intune-shared-resultantappstate.md)|アプリのインストール状態。 可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。|
|supportedDeviceTypes|[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md)コレクション|アプリでサポートされているプラットフォーム。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndStateDetail",
  "applicationId": "String",
  "displayName": "String",
  "mobileAppIntent": "String",
  "displayVersion": "String",
  "installState": "String",
  "supportedDeviceTypes": [
    {
      "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
      "type": "String",
      "minimumOperatingSystemVersion": "String",
      "maximumOperatingSystemVersion": "String"
    }
  ]
}
```





