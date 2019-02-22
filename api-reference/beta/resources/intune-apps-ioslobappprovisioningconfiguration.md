---
title: ioslobappプロビジョニング構成リソースの種類
description: このトピックでは、IOS Lob アプリプロビジョニング構成リソースが公開する、宣言されたメソッド、プロパティ、リレーションシップについて説明します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5ab481571cce9bd986b31d12c41705f8fb48558b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151038"
---
# <a name="ioslobappprovisioningconfiguration-resource-type"></a>ioslobappプロビジョニング構成リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このトピックでは、IOS Lob アプリプロビジョニング構成リソースが公開する、宣言されたメソッド、プロパティ、リレーションシップについて説明します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[ioslobappプロビジョニング構成を一覧表示する](../api/intune-apps-ioslobappprovisioningconfiguration-list.md)|[ioslobappプロビジョニング構成](../resources/intune-apps-ioslobappprovisioningconfiguration.md)コレクション|[ioslobappプロビジョニング構成](../resources/intune-apps-ioslobappprovisioningconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[ioslobappプロビジョニング構成を取得する](../api/intune-apps-ioslobappprovisioningconfiguration-get.md)|[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)|[ioslobappプロビジョニング構成](../resources/intune-apps-ioslobappprovisioningconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[ioslobappプロビジョニング構成を作成する](../api/intune-apps-ioslobappprovisioningconfiguration-create.md)|[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)|新しい[ioslobappプロビジョニング構成](../resources/intune-apps-ioslobappprovisioningconfiguration.md)オブジェクトを作成します。|
|[ioslobappプロビジョニング構成の削除](../api/intune-apps-ioslobappprovisioningconfiguration-delete.md)|なし|[ioslobappプロビジョニング構成](../resources/intune-apps-ioslobappprovisioningconfiguration.md)を削除します。|
|[ioslobappプロビジョニング構成の更新](../api/intune-apps-ioslobappprovisioningconfiguration-update.md)|[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)|[ioslobappプロビジョニング構成](../resources/intune-apps-ioslobappprovisioningconfiguration.md)オブジェクトのプロパティを更新します。|
|[assign action](../api/intune-apps-ioslobappprovisioningconfiguration-assign.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。|
|expirationDateTime|DateTimeOffset|オプションのプロファイルの有効期限の日付と時刻。|
|payloadFileName|String|ペイロードファイル名 (*. mobileprovision | *.xml)。|
|payload|Binary|ペイロード。 (UTF8 でエンコードされたバイト配列)|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。|
|説明|文字列|デバイス構成について管理者が提供した説明です。|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。|
|displayName|String|デバイス構成について管理者が指定した名前です。|
|version|Int32|デバイス構成のバージョン。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|groupAssignments|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)コレクション|関連付けられているグループの割り当て。|
|assignments|[ioslobappプロビジョニング configurationassignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)コレクション|ioslobappプロビジョニング構成に関連付けられたグループの割り当て。|
|deviceStatuses|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)コレクション|このモバイルアプリ構成のデバイスインストール状態のリスト。|
|userStatuses|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) コレクション|このモバイルアプリ構成のユーザーインストール状態のリスト。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosLobAppProvisioningConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "id": "String (identifier)",
  "expirationDateTime": "String (timestamp)",
  "payloadFileName": "String",
  "payload": "binary",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```




