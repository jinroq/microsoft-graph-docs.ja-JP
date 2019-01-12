---
title: microsoftStoreForBusinessApp リソースの種類
description: ビジネス向け Microsoft Store のアプリです。 このクラスは、作成、削除、更新をサポートしていません。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 329872a116fad871f121784af0269377782c2b17
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978670"
---
# <a name="microsoftstoreforbusinessapp-resource-type"></a>microsoftStoreForBusinessApp リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

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
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|アプリの発行の状態。 アプリが発行されていない限り、アプリを割り当てることができません。 [MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。 可能な値は、`notPublished`、`processing`、`published` です。|
|usedLicenseCount|Int32|使用中の、ビジネス向け Microsoft Store ライセンスの数。|
|totalLicenseCount|Int32|ビジネス向け Microsoft Store ライセンスの合計数。|
|productKey|String|アプリのプロダクト キー|
|licenseType|[microsoftStoreForBusinessLicenseType](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|アプリケーション ライセンスの種類。 使用可能な値は、`offline`、`online` です。|
|packageIdentityName|String|アプリ パッケージの識別子|

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
  "publishingState": "String",
  "usedLicenseCount": 1024,
  "totalLicenseCount": 1024,
  "productKey": "String",
  "licenseType": "String",
  "packageIdentityName": "String"
}
```



