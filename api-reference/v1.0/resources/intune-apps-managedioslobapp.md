---
title: managedIOSLobApp リソース タイプ
description: 管理対象 iOS 基幹業務アプリのプロパティと継承されたプロパティが含まれます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6cce7d2de9abef7b569f51e7e3a11f5a4e8d40bf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032278"
---
# <a name="managedioslobapp-resource-type"></a>managedIOSLobApp リソース タイプ

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

管理対象 iOS 基幹業務アプリのプロパティと継承されたプロパティが含まれます。


[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List managedIOSLobApps](../api/intune-apps-managedioslobapp-list.md)|[managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) コレクション|[managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get managedIOSLobApp](../api/intune-apps-managedioslobapp-get.md)|[managedIOSLobApp](../resources/intune-apps-managedioslobapp.md)|[managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create managedIOSLobApp](../api/intune-apps-managedioslobapp-create.md)|[managedIOSLobApp](../resources/intune-apps-managedioslobapp.md)|新しい [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) オブジェクトを作成します。|
|[Delete managedIOSLobApp](../api/intune-apps-managedioslobapp-delete.md)|なし|[managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) を削除します。|
|[Update managedIOSLobApp](../api/intune-apps-managedioslobapp-update.md)|[managedIOSLobApp](../resources/intune-apps-managedioslobapp.md)|[managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|displayName|文字列|管理者が提供またはインポートしたアプリのタイトル。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|description|String|アプリの説明。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|publisher|String|アプリの発行元。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|createdDateTime|DateTimeOffset|アプリが作成された日時。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|アプリが最後に変更された日時。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|isFeatured|Boolean|アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|privacyInformationUrl|String|プライバシーに関する声明の URL。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|informationUrl|String|詳細情報の URL。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|owner|String|アプリの所有者。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|developer|String|アプリの開発者。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|notes|String|アプリ用のメモ。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|アプリの発行の状態。 アプリが発行されていない限り、アプリを割り当てることができません。 [MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。 可能な値は、`notPublished`、`processing`、`published` です。|
|appAvailability|[managedAppAvailability](../resources/intune-apps-managedappavailability.md)|アプリケーションの可用性。 [Managedapp](../resources/intune-apps-managedapp.md)から継承されます。 可能な値は、`global`、`lineOfBusiness` です。|
|version|String|アプリケーションのバージョン。 [managedApp](../resources/intune-apps-managedapp.md) から継承します|
|committedContentVersion|String|内部にコミットされたコンテンツのバージョン。 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します|
|fileName|String|メインの LOB アプリケーションのファイル名。 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します|
|size|Int64|アップロードされたすべてのファイルを含む合計サイズ。 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します|
|bundleId|String|ID 名。|
|applicableDeviceType|[iosDeviceType](../resources/intune-apps-iosdevicetype.md)|このアプリを実行できる iOS アーキテクチャ。|
|minimumSupportedOperatingSystem|[iosMinimumOperatingSystem](../resources/intune-apps-iosminimumoperatingsystem.md)|該当するオペレーティング システムの最小の値。|
|expirationDateTime|DateTimeOffset|有効期限。|
|VersionNumber|String|管理対象 iOS 基幹業務 (LoB) アプリのバージョン番号。|
|buildNumber|String|管理対象 iOS 基幹業務 (LoB) アプリのビルド番号。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション|このアプリのカテゴリのリスト。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション|このモバイル アプリのグループ割り当てのリスト。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|contentVersions|[mobileAppContent](../resources/intune-apps-mobileappcontent.md) コレクション|このアプリのコンテンツのバージョンのリスト。 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedIOSLobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "publishingState": "String",
  "appAvailability": "String",
  "version": "String",
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "bundleId": "String",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "String (timestamp)",
  "versionNumber": "String",
  "buildNumber": "String"
}
```



