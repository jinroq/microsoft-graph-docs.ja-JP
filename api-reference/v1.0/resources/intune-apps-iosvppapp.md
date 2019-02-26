---
title: iosVppApp リソース タイプ
description: iOS ボリューム購入プログラム (VPP) アプリのプロパティと継承されたプロパティが含まれます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: caed1d1643c50d45e7b5659aaa0e815026e6ddfc
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252890"
---
# <a name="iosvppapp-resource-type"></a>iosVppApp リソース タイプ

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

iOS ボリューム購入プログラム (VPP) アプリのプロパティと継承されたプロパティが含まれます。


[mobileApp](../resources/intune-apps-mobileapp.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List iosVppApps](../api/intune-apps-iosvppapp-list.md)|[iosVppApp](../resources/intune-apps-iosvppapp.md) コレクション|[iosVppApp](../resources/intune-apps-iosvppapp.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get iosVppApp](../api/intune-apps-iosvppapp-get.md)|[iosVppApp](../resources/intune-apps-iosvppapp.md)|[iosVppApp](../resources/intune-apps-iosvppapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create iosVppApp](../api/intune-apps-iosvppapp-create.md)|[iosVppApp](../resources/intune-apps-iosvppapp.md)|新しい [iosVppApp](../resources/intune-apps-iosvppapp.md) オブジェクトを作成します。|
|[Delete iosVppApp](../api/intune-apps-iosvppapp-delete.md)|なし|[iosVppApp](../resources/intune-apps-iosvppapp.md) を削除します。|
|[Update iosVppApp](../api/intune-apps-iosvppapp-update.md)|[iosVppApp](../resources/intune-apps-iosvppapp.md)|[iosVppApp](../resources/intune-apps-iosvppapp.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|displayName|String|管理者が提供またはインポートしたアプリのタイトル。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|説明|文字列|アプリの説明。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
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
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|アプリの発行の状態。 アプリが発行されていない限り、アプリを割り当てることができません。 [mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。 可能な値は `notPublished`、`processing`、`published` です。|
|usedLicenseCount|Int32|使用中の VPP ライセンスの数。|
|totalLicenseCount|Int32|VPP ライセンスの総数。|
|releaseDateTime|DateTimeOffset|VPP アプリケーションのリリースの日時。|
|appStoreUrl|String|ストアの URL。|
|licensingType|[vppLicensingType](../resources/intune-apps-vpplicensingtype.md)|サポートされているライセンスの種類。|
|applicableDeviceType|[iosDeviceType](../resources/intune-apps-iosdevicetype.md)|該当する iOS デバイスの種類。|
|vppTokenOrganizationName|文字列|Apple Volume Purchase Program のトークンに関連付けられている組織|
|vppTokenAccountType|[vppTokenAccountType](../resources/intune-shared-vpptokenaccounttype.md)|特定の Apple Volume Purchase Program のトークンが関連付けられている、ボリューム購入プログラムの種類。 使用可能な値は、`business`、`education` です。 可能な値は、`business`、`education` です。|
|vppTokenAppleId|String|特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。|
|bundleId|文字列型 (String)|ID 名。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション|このアプリのカテゴリのリスト。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション|このモバイル アプリのグループ割り当てのリスト。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppApp",
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
  "usedLicenseCount": 1024,
  "totalLicenseCount": 1024,
  "releaseDateTime": "String (timestamp)",
  "appStoreUrl": "String",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "String",
  "vppTokenAccountType": "String",
  "vppTokenAppleId": "String",
  "bundleId": "String"
}
```



