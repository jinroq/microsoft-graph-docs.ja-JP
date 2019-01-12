---
title: userAppInstallStatus リソースの種類
description: プロパティには、ユーザーのインストールのステータスが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f17a504537b1230de175e033779441627f5f98be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938014"
---
# <a name="userappinstallstatus-resource-type"></a>userAppInstallStatus リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

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
|ID|String|エンティティのキー。|
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





