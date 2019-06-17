---
title: Ioslobappプロビジョニング構成リソースの種類
description: このトピックでは、iOS Lob アプリプロビジョニング構成リソースが公開する、宣言されたメソッド、プロパティ、リレーションシップについて説明します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f4de887116625579e0041403e99d42045c015ec
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991213"
---
# <a name="ioslobappprovisioningconfiguration-resource-type"></a>Ioslobappプロビジョニング構成リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このトピックでは、iOS Lob アプリプロビジョニング構成リソースが公開する、宣言されたメソッド、プロパティ、リレーションシップについて説明します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[Ioslobappプロビジョニング構成を一覧表示する](../api/intune-apps-ioslobappprovisioningconfiguration-list.md)|[Ioslobappプロビジョニング構成](../resources/intune-apps-ioslobappprovisioningconfiguration.md)コレクション|[Ioslobappプロビジョニング構成](../resources/intune-apps-ioslobappprovisioningconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[Ioslobappプロビジョニング構成を取得する](../api/intune-apps-ioslobappprovisioningconfiguration-get.md)|[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)|[Ioslobappプロビジョニング構成](../resources/intune-apps-ioslobappprovisioningconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Ioslobappプロビジョニング構成を作成する](../api/intune-apps-ioslobappprovisioningconfiguration-create.md)|[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)|新しい[Ioslobappプロビジョニング構成](../resources/intune-apps-ioslobappprovisioningconfiguration.md)オブジェクトを作成します。|
|[Ioslobappプロビジョニング構成の削除](../api/intune-apps-ioslobappprovisioningconfiguration-delete.md)|None|[Ioslobappプロビジョニング構成](../resources/intune-apps-ioslobappprovisioningconfiguration.md)を削除します。|
|[Ioslobappプロビジョニング構成の更新](../api/intune-apps-ioslobappprovisioningconfiguration-update.md)|[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)|[Ioslobappプロビジョニング構成](../resources/intune-apps-ioslobappprovisioningconfiguration.md)オブジェクトのプロパティを更新します。|
|[assign アクション](../api/intune-apps-ioslobappprovisioningconfiguration-assign.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。|
|expirationDateTime|DateTimeOffset|オプションのプロファイルの有効期限の日付と時刻。|
|payloadFileName|String|ペイロードファイル名 (*. mobileprovision | *.xml)。|
|payload|Binary|ペイロード。 (UTF8 でエンコードされたバイト配列)|
|roleScopeTagIds|文字列コレクション|この iOS LOB アプリプロビジョニング構成エンティティのスコープタグのリスト。|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。|
|description|String|デバイス構成について管理者が提供した説明です。|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。|
|displayName|String|デバイス構成について管理者が指定した名前です。|
|version|Int32|デバイス構成のバージョン。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|groupAssignments|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)コレクション|関連付けられているグループの割り当て。|
|assignments|[Ioslobappプロビジョニング Configurationassignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)コレクション|Ioslobappプロビジョニング構成に関連付けられたグループの割り当て。|
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
  "roleScopeTagIds": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```





