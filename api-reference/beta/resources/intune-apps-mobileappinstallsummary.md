---
title: mobileAppInstallSummary リソースの種類
description: モバイルアプリのインストールの概要のプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f1e1d1a815ba1d4c688819a8d94c8acdd5beffca
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991829"
---
# <a name="mobileappinstallsummary-resource-type"></a>mobileAppInstallSummary リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

モバイルアプリのインストールの概要のプロパティが含まれています。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[MobileAppInstallSummary を取得する](../api/intune-apps-mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|[MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[MobileAppInstallSummary の更新](../api/intune-apps-mobileappinstallsummary-update.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|[MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|installedDeviceCount|Int32|このアプリが正常にインストールされたデバイスの数。|
|failedDeviceCount|Int32|このアプリのインストールに失敗したデバイスの数。|
|notApplicableDeviceCount|Int32|このアプリに適用されないデバイスの数。|
|notInstalledDeviceCount|Int32|このアプリがインストールされていないデバイスの数。|
|pendingInstallDeviceCount|Int32|このアプリをインストールするように通知されたデバイスの数。|
|installedUserCount|Int32|このアプリをインストールするためにすべてのデバイスが正常に終了したユーザーの数。|
|failedUserCount|Int32|このアプリのインストールに失敗した1つ以上のデバイスを持つユーザーの数。|
|notApplicableUserCount|Int32|このアプリに適用されていないデバイスを持つユーザーの数。|
|notInstalledUserCount|Int32|このアプリをインストールしなかった1つ以上のデバイスを持つユーザーの数。|
|pendingInstallUserCount|Int32|このアプリをインストールするように通知された1つ以上のデバイスを保有していて、エラーがあるデバイスが0個あるユーザーの数。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppInstallSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "pendingInstallDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notApplicableUserCount": 1024,
  "notInstalledUserCount": 1024,
  "pendingInstallUserCount": 1024
}
```





