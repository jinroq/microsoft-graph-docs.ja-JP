---
title: managedAndroidLobApp リソース タイプ
description: 管理対象 Android 基幹業務アプリのプロパティと継承されたプロパティが含まれます。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 79c2143700d52e2bf3119e0be5445f3b65163ed1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990846"
---
# <a name="managedandroidlobapp-resource-type"></a>managedAndroidLobApp リソース タイプ

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

管理対象 Android 基幹業務アプリのプロパティと継承されたプロパティが含まれます。

[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List managedAndroidLobApps](../api/intune-apps-managedandroidlobapp-list.md)|[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) コレクション|[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get managedAndroidLobApp](../api/intune-apps-managedandroidlobapp-get.md)|[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)|[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create managedAndroidLobApp](../api/intune-apps-managedandroidlobapp-create.md)|[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)|新しい [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) オブジェクトを作成します。|
|[Delete managedAndroidLobApp](../api/intune-apps-managedandroidlobapp-delete.md)|なし|[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) を削除します。|
|[Update managedAndroidLobApp](../api/intune-apps-managedandroidlobapp-update.md)|[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)|[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|displayName|String|管理者が提供またはインポートしたアプリのタイトル。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|説明|String|アプリの説明。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|publisher|String|アプリの発行元。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|createdDateTime|DateTimeOffset|アプリが作成された日時。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|アプリが最後に変更された日時。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|isFeatured|Boolean|アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|privacyInformationUrl|String|プライバシーに関する声明の URL。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|informationUrl|String|詳細情報の URL。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|owner|String|アプリの所有者。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|developer|String|アプリの開発者。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|notes|String|アプリ用のメモ。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|uploadState|Int32|アップロードの状態です。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|アプリの発行の状態。 アプリが発行されていない限り、アプリを割り当てることができません。 [MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。 可能な値は、`notPublished`、`processing`、`published` です。|
|appAvailability|[managedAppAvailability](../resources/intune-apps-managedappavailability.md)|アプリケーションの可用性。 [ManagedApp](../resources/intune-apps-managedapp.md)から継承されます。 可能な値は、`global`、`lineOfBusiness` です。|
|version|String|アプリケーションのバージョン。 [managedApp](../resources/intune-apps-managedapp.md) から継承します|
|committedContentVersion|String|内部にコミットされたコンテンツのバージョン。 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します|
|fileName|String|メインの Lob アプリケーションのファイル名。 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します|
|size|Int64|アップロードされたすべてのファイルを含む合計サイズ。 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します|
|packageId|String|パッケージの識別子。|
|identityName|String|ID 名。|
|minimumSupportedOperatingSystem|[androidMinimumOperatingSystem](../resources/intune-apps-androidminimumoperatingsystem.md)|該当するオペレーティング システムの最小の値です。|
|versionName|String|管理対象 Android 基幹業務 (LoB) アプリのバージョン名。|
|versionCode|String|管理対象 Android 基幹業務 (LoB) アプリのバージョン コード。|
|identityVersion|String|ID のバージョン。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション|このアプリのカテゴリのリスト。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション|このモバイル アプリのグループ割り当てのリスト。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|モバイル アプリ インストール概要です。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)コレクション|このモバイル アプリケーションのインストール状況の一覧です。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)コレクション|このモバイル アプリケーションのインストール状況の一覧です。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|contentVersions|[mobileAppContent](../resources/intune-apps-mobileappcontent.md) コレクション|このアプリのコンテンツのバージョンのリスト。 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAndroidLobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "uploadState": 1024,
  "publishingState": "String",
  "appAvailability": "String",
  "version": "String",
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "packageId": "String",
  "identityName": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "String",
  "versionCode": "String",
  "identityVersion": "String"
}
```





