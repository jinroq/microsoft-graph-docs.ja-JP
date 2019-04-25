---
title: officeSuiteApp リソースの種類
description: Office365 Suite アプリのプロパティと継承されたプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0109154dada9ddfdf848b698b052f68c68527259
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551793"
---
# <a name="officesuiteapp-resource-type"></a>officeSuiteApp リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Office365 Suite アプリのプロパティと継承されたプロパティが含まれています。


[mobileApp](../resources/intune-apps-mobileapp.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト officeSuiteApps](../api/intune-apps-officesuiteapp-list.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)コレクション|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[officeSuiteApp を取得する](../api/intune-apps-officesuiteapp-get.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[officeSuiteApp を作成する](../api/intune-apps-officesuiteapp-create.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|新しい[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)オブジェクトを作成します。|
|[officeSuiteApp の削除](../api/intune-apps-officesuiteapp-delete.md)|なし|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)を削除します。|
|[officeSuiteApp の更新](../api/intune-apps-officesuiteapp-update.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|エンティティのキー。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|displayName|String|管理者が提供またはインポートしたアプリのタイトル。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
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
|uploadState|Int32|アップロード状態。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|アプリの発行の状態。 アプリが発行されていない限り、アプリを割り当てることができません。 [mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。 使用可能な値は、`notPublished`、`processing`、`published` です。|
|isAssigned|Boolean|アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|roleScopeTagIds|String collection|このモバイルアプリの範囲タグ id のリスト。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|dependentappcount|Int32|子アプリが持つ依存関係の合計数。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|autoAcceptEula|ブール値|enduser のデバイスで EULA に自動的に同意する値。|
|productIds|[officeproductid](../resources/intune-apps-officeproductid.md)コレクション|Office365 スイート SKU を表す製品 id。|
|excludedApps|[excludedApps](../resources/intune-apps-excludedapps.md)|選択した Office365 製品 Id から除外されるアプリを表すプロパティ。|
|。 usesharedcomputeractivation|ブール値|office 365 アプリスイートに対して共有コンピューターのライセンス認証が使用されていないかどうかを表すプロパティ。|
|updateChannel|[officeUpdateChannel](../resources/intune-apps-officeupdatechannel.md)|Office365 更新チャネルを表すプロパティ。 可能な値は、`none`、`current`、`deferred`、`firstReleaseCurrent`、`firstReleaseDeferred` です。|
|officePlatformArchitecture|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|Office365 アプリスイートのバージョンを表すプロパティ。 可能な値は `none`、`x86`、`x64`、`arm`、`neutral`、`arm64` です。|
|次|String collection|Office365 のアプリをインストールするときにインストールされるロケールを表すプロパティ。 標準の RFC 6033 を使用します。 Refhttps://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx|
|install進捗 displaylevel|[officeSuiteInstallProgressDisplayLevel](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|デバイス上のインストールの進行状況のセットアップ UI の表示レベルを指定します。 可能な値は、`none`、`full` です。|
|shouldUninstallOlderVersionsOfOffice|ブール値|Office365 アプリスイートがデバイスに展開されている場合に、既存の Office MSI をアンインストールするかどうかを決定するプロパティ。|
|targetVersion|String|デバイスに展開されたままにする必要がある、Office365 アプリスイートの特定のターゲットバージョンを表すプロパティ。|
|updateversion|String|Office365 アプリスイートで特定のターゲットバージョンが利用可能な更新バージョンを表すプロパティ。|
|officeConfigurationXml|Binary|Office ProPlus アプリに指定できる XML 構成ファイルを表すプロパティ。 他のすべてのプロパティより優先されます。 指定した場合、XML 構成ファイルを使用してアプリが作成されます。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション|このアプリのカテゴリのリスト。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション|このモバイル アプリのグループ割り当てのリスト。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|モバイル アプリ インストール概要です。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)コレクション|このモバイルアプリのインストール状態のリスト。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|userStatuses|[userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)コレクション|このモバイルアプリのインストール状態のリスト。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|関連性|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)コレクション|このモバイルアプリのリレーションシップのリスト。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|

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
  "dependentAppCount": 1024,
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
    "teams": true,
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





