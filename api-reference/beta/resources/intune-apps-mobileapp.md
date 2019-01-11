---
title: mobileApp リソースの種類
description: Intune モバイル アプリの基本プロパティを含む抽象クラスです。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 01bde6a94c0d16b26b20d1ba30e69bec0457972e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812538"
---
# <a name="mobileapp-resource-type"></a>mobileApp リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Intune モバイル アプリの基本プロパティを含む抽象クラスです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[mobileApps のリスト](../api/intune-apps-mobileapp-list.md)|[mobileApp](../resources/intune-apps-mobileapp.md) コレクション|[mobileApp](../resources/intune-apps-mobileapp.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[MobileApp の取得](../api/intune-apps-mobileapp-get.md)|[mobileApp](../resources/intune-apps-mobileapp.md)|[mobileApp](../resources/intune-apps-mobileapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[アクションの割り当て](../api/intune-apps-mobileapp-assign.md)|なし|まだ文書化されていません|
|[getMobileAppCount 関数](../api/intune-apps-mobileapp-getmobileappcount.md)|Int64|まだ文書化されていません|
|[getTopMobileApps 関数](../api/intune-apps-mobileapp-gettopmobileapps.md)|[mobileApp](../resources/intune-apps-mobileapp.md) コレクション|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。|
|displayName|String|管理者が提供またはインポートしたアプリのタイトルです。|
|説明|String|アプリの説明。|
|publisher|String|アプリの発行元。|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。|
|createdDateTime|DateTimeOffset|アプリが作成された日時。|
|lastModifiedDateTime|DateTimeOffset|アプリが最後に変更された日時。|
|isFeatured|Boolean|アプリが管理者のおすすめとしてマークされたかどうかを示す値。|
|privacyInformationUrl|String|プライバシーに関する声明の URL。|
|informationUrl|String|詳細情報の URL。|
|owner|String|アプリの所有者。|
|developer|String|アプリの開発者。|
|notes|String|アプリ用のメモ。|
|uploadState|Int32|アップロードの状態です。|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|アプリの発行の状態。 アプリが発行されていない限り、アプリを割り当てることができません。 可能な値は、`notPublished`、`processing`、`published` です。|

## <a name="relationships"></a>関係
|リレーションシップ|型|説明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション|このアプリのカテゴリのリストです。|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション|このモバイル アプリのグループ割り当てのリスト。|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|モバイル アプリ インストール概要です。|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)コレクション|このモバイル アプリケーションのインストール状況の一覧です。|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)コレクション|このモバイル アプリケーションのインストール状況の一覧です。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileApp",
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
  "publishingState": "String"
}
```





