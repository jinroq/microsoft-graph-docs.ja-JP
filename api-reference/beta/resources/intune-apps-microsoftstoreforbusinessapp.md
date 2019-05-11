---
title: microsoftStoreForBusinessApp リソースの種類
description: ビジネス向け Microsoft Store のアプリです。 このクラスは、作成、削除、更新をサポートしていません。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8870982c1322f5ee2c14dc399020f34e2fcc0924
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950047"
---
# <a name="microsoftstoreforbusinessapp-resource-type"></a>microsoftStoreForBusinessApp リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ビジネス向け Microsoft Store のアプリです。 このクラスは、作成、削除、更新をサポートしていません。


[mobileApp](../resources/intune-apps-mobileapp.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[microsoftStoreForBusinessApps のリスト](../api/intune-apps-microsoftstoreforbusinessapp-list.md)|[microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) コレクション|[microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[microsoftStoreForBusinessApp の取得](../api/intune-apps-microsoftstoreforbusinessapp-get.md)|[microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)|[microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[microsoftStoreForBusinessApp の作成](../api/intune-apps-microsoftstoreforbusinessapp-create.md)|[microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)|新しい [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) オブジェクトを作成します。|
|[microsoftStoreForBusinessApp の削除](../api/intune-apps-microsoftstoreforbusinessapp-delete.md)|なし|[microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) を削除します。|
|[microsoftStoreForBusinessApp の更新](../api/intune-apps-microsoftstoreforbusinessapp-update.md)|[microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)|[microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) オブジェクトのプロパティを更新します。|

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
|uploadState|Int32|アップロード状態。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|アプリの発行の状態。 アプリが発行されていない限り、アプリを割り当てることができません。 [MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。 可能な値は、`notPublished`、`processing`、`published` です。|
|isAssigned|Boolean|アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|roleScopeTagIds|String collection|このモバイルアプリの範囲タグ id のリスト。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|dependentAppCount|Int32|子アプリが持つ依存関係の合計数。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|usedLicenseCount|Int32|使用中の、ビジネス向け Microsoft Store ライセンスの数。|
|totalLicenseCount|Int32|ビジネス向け Microsoft Store ライセンスの合計数。|
|productKey|String|アプリのプロダクト キー|
|licenseType|[Microsoft Storeforbusinesslicensetype](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|アプリライセンスの種類。 可能な値は、`offline`、`online` です。|
|packageIdentityName|String|アプリ パッケージの識別子|
|licensingType|[vppLicensingType](../resources/intune-apps-vpplicensingtype.md)|サポートされているライセンスの種類。|

## <a name="relationships"></a>関係
|リレーションシップ|型|説明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション|このアプリのカテゴリのリスト。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション|このモバイル アプリのグループ割り当てのリスト。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|モバイル アプリ インストール概要です。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)コレクション|このモバイルアプリのインストール状態のリスト。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|userStatuses|[Userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)コレクション|このモバイルアプリのインストール状態のリスト。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|関連性|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)コレクション|このモバイルアプリのリレーションシップのリスト。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|containedApps|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)コレクション|パッケージとして機能する mobileApp に含まれているアプリのコレクション。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
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
  "usedLicenseCount": 1024,
  "totalLicenseCount": 1024,
  "productKey": "String",
  "licenseType": "String",
  "packageIdentityName": "String",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  }
}
```




