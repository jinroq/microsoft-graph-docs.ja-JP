---
title: mobileAppInstallSummary リソースの種類
description: モバイル アプリケーションのインストールの概要のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a75dba8303d254aff911cc66931d52abb8b76c07
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916027"
---
# <a name="mobileappinstallsummary-resource-type"></a>mobileAppInstallSummary リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

モバイル アプリケーションのインストールの概要のプロパティが含まれています。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[MobileAppInstallSummary を取得します。](../api/intune-apps-mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|[MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトのプロパティと関係を参照してください。|
|[MobileAppInstallSummary を更新します。](../api/intune-apps-mobileappinstallsummary-update.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|[MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。|
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





