---
title: officeSuiteApp リソースの種類
description: Office365 スイート アプリケーションのプロパティと継承されたプロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2be565af88961ebafe4ed978524763797a3fe475
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395532"
---
# <a name="officesuiteapp-resource-type"></a>officeSuiteApp リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Office365 スイート アプリケーションのプロパティと継承されたプロパティが含まれています。


[mobileApp](../resources/intune-apps-mobileapp.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト officeSuiteApps](../api/intune-apps-officesuiteapp-list.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)コレクション|[OfficeSuiteApp](../resources/intune-apps-officesuiteapp.md)オブジェクトのプロパティと関係を一覧表示します。|
|[OfficeSuiteApp を取得します。](../api/intune-apps-officesuiteapp-get.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|[OfficeSuiteApp](../resources/intune-apps-officesuiteapp.md)オブジェクトのプロパティと関係を参照してください。|
|[OfficeSuiteApp を作成します。](../api/intune-apps-officesuiteapp-create.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|新しい[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)オブジェクトを作成します。|
|[OfficeSuiteApp を削除します。](../api/intune-apps-officesuiteapp-delete.md)|なし|の[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)を削除します。|
|[OfficeSuiteApp を更新します。](../api/intune-apps-officesuiteapp-update.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|[OfficeSuiteApp](../resources/intune-apps-officesuiteapp.md)オブジェクトのプロパティを更新します。|

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
|isAssigned|Boolean|アプリケーションが少なくとも 1 つのグループに割り当てられているかどうかを示す値です。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|roleScopeTagIds|String コレクション|このモバイル アプリケーションのスコープのタグ id の一覧です。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|autoAcceptEula|Boolean|エンド ・ ユーザーのデバイスに自動的に使用許諾契約書をそのまま使用する値。|
|productIds|[officeProductId](../resources/intune-apps-officeproductid.md)コレクション|Office365 スイート SKU を表すプロダクト Id です。|
|excludedApps|[excludedApps](../resources/intune-apps-excludedapps.md)|選択した Office365 製品 id。 から除外されている場合、アプリケーションを表すためのプロパティ|
|useSharedComputerActivation|Boolean|Office365 アプリケーション スイートではなく、共有のコンピューターのライセンス認証が使用されるかどうかを表すプロパティです。|
|updateChannel|[officeUpdateChannel](../resources/intune-apps-officeupdatechannel.md)|Office365 更新チャネルを表すプロパティです。 可能な値は、`none`、`current`、`deferred`、`firstReleaseCurrent`、`firstReleaseDeferred` です。|
|officePlatformArchitecture|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|Office365 アプリケーション スイートのバージョンを表すプロパティです。 使用可能な値: `none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。|
|localesToInstall|String コレクション|インストールされているロケールを表すプロパティ Office365 からアプリケーションがインストールされています。 標準の RFC 6033 を使用します。 Ref。https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx|
|installProgressDisplayLevel|[officeSuiteInstallProgressDisplayLevel](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|デバイスのインストール中のセットアップの UI の表示のレベルを指定します。 使用可能な値は、`none`、`full` です。|
|shouldUninstallOlderVersionsOfOffice|Boolean|Office365 のアプリケーション スイートをかデバイスに配置する場合は、既存の Office MSI をアンインストールするかどうかを決定するプロパティ。|
|targetVersion|String|デバイス上に配置されたままする必要があります Office365 アプリケーション スイートの特定のターゲットのバージョンを表すプロパティです。|
|updateVersion|String|ターゲットの特定のバージョンで Office365 アプリケーション スイートの利用可能な更新プログラムのバージョンを表すプロパティです。|
|officeConfigurationXml|Binary|Office 用リソースのアプリケーションに指定できる XML 構成ファイルを表すプロパティです。 その他のすべてのプロパティに優先します。 存在する場合、XML 構成ファイルを使用してアプリケーションを作成します。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション|このアプリのカテゴリのリスト。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション|このモバイル アプリのグループ割り当てのリスト。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|モバイル アプリ インストール概要です。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)コレクション|このモバイル アプリケーションのインストール状況の一覧です。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)コレクション|このモバイル アプリケーションのインストール状況の一覧です。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeSuiteApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeSuiteApp",
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
  "isAssigned": true,
  "roleScopeTagIds": [
    "String"
  ],
  "autoAcceptEula": true,
  "productIds": [
    "String"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "String",
  "officePlatformArchitecture": "String",
  "localesToInstall": [
    "String"
  ],
  "installProgressDisplayLevel": "String",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "String",
  "updateVersion": "String",
  "officeConfigurationXml": "binary"
}
```




