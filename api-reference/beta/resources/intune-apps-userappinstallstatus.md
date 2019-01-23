---
title: userAppInstallStatus リソースの種類
description: プロパティには、ユーザーのインストールのステータスが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1e1369e35af2343bebd609c760075a830649a1f2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399893"
---
# <a name="userappinstallstatus-resource-type"></a>userAppInstallStatus リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

プロパティには、ユーザーのインストールのステータスが含まれています。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト userAppInstallStatuses](../api/intune-apps-userappinstallstatus-list.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)コレクション|[UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティと関係を一覧表示します。|
|[UserAppInstallStatus を取得します。](../api/intune-apps-userappinstallstatus-get.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|[UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティと関係を参照してください。|
|[UserAppInstallStatus を作成します。](../api/intune-apps-userappinstallstatus-create.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|新しい[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトを作成します。|
|[UserAppInstallStatus を削除します。](../api/intune-apps-userappinstallstatus-delete.md)|なし|の[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)を削除します。|
|[UserAppInstallStatus を更新します。](../api/intune-apps-userappinstallstatus-update.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|[UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|userName|String|ユーザー名です。|
|userPrincipalName|String|ユーザー プリンシパル名です。|
|installedDeviceCount|Int32|インストールされたデバイスの数です。|
|failedDeviceCount|Int32|失敗したデバイスの数です。|
|notInstalledDeviceCount|Int32|インストールされていないデバイスの数です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|アプリ|[mobileApp](../resources/intune-apps-mobileapp.md)|モバイル アプリケーションへのナビゲーション リンクです。|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)コレクション|デバイス上のアプリケーションのインストール状態です。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userAppInstallStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userAppInstallStatus",
  "id": "String (identifier)",
  "userName": "String",
  "userPrincipalName": "String",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024
}
```




