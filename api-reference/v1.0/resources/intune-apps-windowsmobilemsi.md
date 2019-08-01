---
title: windowsMobileMSI リソース タイプ
description: Windows Mobile MSI 基幹業務アプリケーションのプロパティと継承されたプロパティが含まれます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 61f35eb4df5e7da98011d849e525a661559f440d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032068"
---
# <a name="windowsmobilemsi-resource-type"></a>windowsMobileMSI リソース タイプ

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows Mobile MSI 基幹業務アプリケーションのプロパティと継承されたプロパティが含まれます。


[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List windowsMobileMSIs](../api/intune-apps-windowsmobilemsi-list.md)|[windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) コレクション|[windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get windowsMobileMSI](../api/intune-apps-windowsmobilemsi-get.md)|[windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md)|[windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create windowsMobileMSI](../api/intune-apps-windowsmobilemsi-create.md)|[windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md)|新しく [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) オブジェクトを作成します。|
|[Delete windowsMobileMSI](../api/intune-apps-windowsmobilemsi-delete.md)|なし|[windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) を削除します。|
|[Update windowsMobileMSI](../api/intune-apps-windowsmobilemsi-update.md)|[windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md)|[windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) オブジェクトのプロパティを更新します。|

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
|committedContentVersion|String|内部にコミットされたコンテンツのバージョン。 [mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します|
|fileName|文字列型 (String)|メインの LOB アプリケーションのファイル名。 [mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します|
|size|Int64|アップロードされたすべてのファイルを含む合計サイズ。 [mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します|
|commandLine|String|コマンド ライン。|
|productCode|String|製品コード。|
|productVersion|String|Windows Mobile MSI 基幹業務 (LoB) アプリの製品のバージョン。|
|ignoreVersionDetection|Boolean|アプリをデバイスにインストールした後に、アプリのバージョンを使用してアプリを検出するかどうかを制御するブール値。 自己更新機能を使用する Windows Mobile MSI 基幹業務 (LoB) アプリの場合は、true に設定します。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション|このアプリのカテゴリのリスト。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション|このモバイル アプリのグループ割り当てのリスト。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|contentVersions|[mobileAppContent](../resources/intune-apps-mobileappcontent.md) コレクション|このアプリのコンテンツのバージョンのリスト。 [mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsMobileMSI"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "commandLine": "String",
  "productCode": "String",
  "productVersion": "String",
  "ignoreVersionDetection": true
}
```



