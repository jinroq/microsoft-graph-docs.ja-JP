---
title: win32LobApp リソースの種類
description: プロパティと Win32 アプリケーションの継承されたプロパティが含まれています。
ms.openlocfilehash: 00bbf4be533d56661786bbde3ae68478af5d27b9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071329"
---
# <a name="win32lobapp-resource-type"></a>win32LobApp リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

プロパティと Win32 アプリケーションの継承されたプロパティが含まれています。

[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト win32LobApps](../api/intune-apps-win32lobapp-list.md)|[win32LobApp](../resources/intune-apps-win32lobapp.md)コレクション|[Win32LobApp](../resources/intune-apps-win32lobapp.md)オブジェクトのプロパティと関係を一覧表示します。|
|[Win32LobApp を取得します。](../api/intune-apps-win32lobapp-get.md)|[win32LobApp](../resources/intune-apps-win32lobapp.md)|[Win32LobApp](../resources/intune-apps-win32lobapp.md)オブジェクトのプロパティと関係を参照してください。|
|[Win32LobApp を作成します。](../api/intune-apps-win32lobapp-create.md)|[win32LobApp](../resources/intune-apps-win32lobapp.md)|新しい[win32LobApp](../resources/intune-apps-win32lobapp.md)オブジェクトを作成します。|
|[Win32LobApp を削除します。](../api/intune-apps-win32lobapp-delete.md)|なし|の[win32LobApp](../resources/intune-apps-win32lobapp.md)を削除します。|
|[Win32LobApp を更新します。](../api/intune-apps-win32lobapp-update.md)|[win32LobApp](../resources/intune-apps-win32lobapp.md)|[Win32LobApp](../resources/intune-apps-win32lobapp.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
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
|committedContentVersion|String|内部にコミットされたコンテンツのバージョン。 [mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します|
|fileName|String|メインの Lob アプリケーションのファイル名。 [mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します|
|size|Int64|アップロードされたすべてのファイルを含む合計サイズ。 [mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します|
|installCommandLine|String|このアプリケーションをインストールするのにはコマンド ・ ライン|
|uninstallCommandLine|String|このアプリケーションをアンインストールするのにはコマンド ・ ライン|
|applicableArchitectures|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|このアプリを実行できる Windows アーキテクチャ。 可能な値は、`none`、`x86`、`x64`、`arm`、`neutral` です。|
|minimumSupportedOperatingSystem|[windowsMinimumOperatingSystem](../resources/intune-apps-windowsminimumoperatingsystem.md)|該当するオペレーティング システムの最小の値です。|
|minimumFreeDiskSpaceInMB|Int32|このアプリケーションをインストールするために必要な最小空きディスク容量の値。|
|minimumMemoryInMB|Int32|このアプリケーションをインストールするために必要な物理メモリの最小の値。|
|minimumNumberOfProcessors|Int32|このアプリケーションをインストールするために必要な最小のプロセッサの数の値。|
|minimumCpuSpeedInMHz|Int32|このアプリケーションをインストールするために必要な最低限の CPU 速度の値です。|
|detectionRules|[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)コレクション|Win32 基幹業務 (LoB) アプリケーションを検出する検出ルールです。|
|installExperience|[win32LobAppInstallExperience](../resources/intune-apps-win32lobappinstallexperience.md)|このアプリケーションのインストール経験。|
|開始|[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)コレクション|リターン コードは、インストール時の動作を転記します。|
|msiInformation|[win32LobAppMsiInformation](../resources/intune-apps-win32lobappmsiinformation.md)|この Win32 アプリケーションでは、MSI アプリケーションの場合は、MSI 詳細です。|
|setupFilePath|String|暗号化された Win32LobApp パッケージのセットアップ ファイルの相対パスです。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション|このアプリのカテゴリのリスト。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション|このモバイル アプリのグループ割り当てのリスト。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|モバイル アプリ インストール概要です。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)コレクション|このモバイル アプリケーションのインストール状況の一覧です。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)コレクション|このモバイル アプリケーションのインストール状況の一覧です。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|contentVersions|[mobileAppContent](../resources/intune-apps-mobileappcontent.md) コレクション|このアプリのコンテンツのバージョンのリスト。 [mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.win32LobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobApp",
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
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "installCommandLine": "String",
  "uninstallCommandLine": "String",
  "applicableArchitectures": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "minimumFreeDiskSpaceInMB": 1024,
  "minimumMemoryInMB": 1024,
  "minimumNumberOfProcessors": 1024,
  "minimumCpuSpeedInMHz": 1024,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "String",
      "valueName": "String",
      "detectionType": "String",
      "operator": "String",
      "detectionValue": "String"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "String"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 1024,
      "type": "String"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "String",
    "productVersion": "String",
    "upgradeCode": "String",
    "requiresReboot": true,
    "packageType": "String"
  },
  "setupFilePath": "String"
}
```





