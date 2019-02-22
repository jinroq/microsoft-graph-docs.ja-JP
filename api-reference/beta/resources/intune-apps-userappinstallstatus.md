---
title: userappinstallstatus リソースの種類
description: ユーザーのインストール状態のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4778728fbec389b276e5098ffa859f13ccb6a9e4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143961"
---
# <a name="userappinstallstatus-resource-type"></a>userappinstallstatus リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ユーザーのインストール状態のプロパティが含まれています。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[userappinstallstatuses 状態を一覧表示する](../api/intune-apps-userappinstallstatus-list.md)|[userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)コレクション|[userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[userappinstallstatus の取得](../api/intune-apps-userappinstallstatus-get.md)|[userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)|[userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[userappinstallstatus の作成](../api/intune-apps-userappinstallstatus-create.md)|[userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)|新しい[userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトを作成します。|
|[userappinstallstatus の削除](../api/intune-apps-userappinstallstatus-delete.md)|なし|[userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)を削除します。|
|[userappinstallstatus の更新](../api/intune-apps-userappinstallstatus-update.md)|[userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)|[userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|userName|String|ユーザー名です。|
|userPrincipalName|String|ユーザープリンシパル名。|
|installedDeviceCount|Int32|インストールされたデバイスの数です。|
|failedDeviceCount|Int32|失敗したデバイスの数です。|
|notInstalledDeviceCount|Int32|インストールされていないデバイスの数です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|アプリ|[mobileApp](../resources/intune-apps-mobileapp.md)|モバイルアプリへのナビゲーションリンク。|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)コレクション|デバイス上のアプリのインストール状態。|

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




