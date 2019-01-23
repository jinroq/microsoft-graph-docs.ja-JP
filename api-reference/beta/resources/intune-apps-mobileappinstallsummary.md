---
title: mobileAppInstallSummary リソースの種類
description: モバイル アプリケーションのインストールの概要のプロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a2bd7c30c1b00e83731766bcd80f9a9fafd8e8b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416714"
---
# <a name="mobileappinstallsummary-resource-type"></a>mobileAppInstallSummary リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

モバイル アプリケーションのインストールの概要のプロパティが含まれています。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[MobileAppInstallSummary を取得します。](../api/intune-apps-mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|[MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトのプロパティと関係を参照してください。|
|[MobileAppInstallSummary を更新します。](../api/intune-apps-mobileappinstallsummary-update.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|[MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|installedDeviceCount|Int32|このアプリケーションを正常にインストールするデバイスの数です。|
|failedDeviceCount|Int32|このアプリケーションのインストールに失敗したデバイスの数。|
|notApplicableDeviceCount|Int32|このアプリケーションには適用されていないデバイスの数です。|
|notInstalledDeviceCount|Int32|このアプリケーションをインストールしていないデバイスの数。|
|pendingInstallDeviceCount|Int32|このアプリケーションをインストールするのには通知しているデバイスの数です。|
|installedUserCount|Int32|このアプリケーションをインストールするのにはデバイスがすべて成功しているユーザーの数です。|
|failedUserCount|Int32|1 を持っているユーザー、またはこのアプリケーションのインストールに失敗した複数のデバイスの数です。|
|notApplicableUserCount|Int32|デバイスがなかったすべてこのアプリケーションに適用可能なユーザーの数です。|
|notInstalledUserCount|Int32|このアプリケーションがインストールされていない 1 つ以上のデバイスを持っているユーザーの数です。|
|pendingInstallUserCount|Int32|1 を持っているユーザー、またはこのアプリケーションをインストールし、0 のデバイス障害を通知している複数のデバイスの数です。|

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




