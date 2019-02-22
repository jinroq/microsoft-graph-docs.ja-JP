---
title: iosVppEBook リソースの種類
description: iOS Vpp eBook のプロパティを含むクラスです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ca890a6b15ac232d8fb685913379ba8bf69f35cc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149442"
---
# <a name="iosvppebook-resource-type"></a>iosVppEBook リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

iOS Vpp eBook のプロパティを含むクラスです。


[managedEBook](../resources/intune-books-managedebook.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[iosVppEBooks のリスト](../api/intune-books-iosvppebook-list.md)|[iosVppEBook](../resources/intune-books-iosvppebook.md) コレクション|[iosVppEBook](../resources/intune-books-iosvppebook.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[iosVppEBook の取得](../api/intune-books-iosvppebook-get.md)|[iosVppEBook](../resources/intune-books-iosvppebook.md)|[iosVppEBook](../resources/intune-books-iosvppebook.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[iosVppEBook の作成](../api/intune-books-iosvppebook-create.md)|[iosVppEBook](../resources/intune-books-iosvppebook.md)|新しい [iosVppEBook](../resources/intune-books-iosvppebook.md) オブジェクトを作成します。|
|[iosVppEBook の削除](../api/intune-books-iosvppebook-delete.md)|なし|[iosVppEBook](../resources/intune-books-iosvppebook.md) を削除します。|
|[iosVppEBook の更新](../api/intune-books-iosvppebook-update.md)|[iosVppEBook](../resources/intune-books-iosvppebook.md)|[iosVppEBook](../resources/intune-books-iosvppebook.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。 [managedEBook](../resources/intune-books-managedebook.md) から継承します|
|displayName|String|電子ブックの名前。 [managedEBook](../resources/intune-books-managedebook.md) から継承します|
|説明|文字列|説明。 [managedEBook](../resources/intune-books-managedebook.md) から継承します|
|publisher|文字列型 (String)|発行元です。 [managedEBook](../resources/intune-books-managedebook.md) から継承します|
|publishedDateTime|DateTimeOffset|電子ブックが発行された日時。 [managedEBook](../resources/intune-books-managedebook.md) から継承します|
|largeCover|[mimeContent](../resources/intune-shared-mimecontent.md)|ブック カバー。 [managedEBook](../resources/intune-books-managedebook.md) から継承します|
|createdDateTime|DateTimeOffset|電子ブック ファイルが作成された日時。 [managedEBook](../resources/intune-books-managedebook.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|電子ブックが最後に変更された日時。 [managedEBook](../resources/intune-books-managedebook.md) から継承します|
|informationUrl|String|詳細情報の URL。 [managedEBook](../resources/intune-books-managedebook.md) から継承します|
|privacyInformationUrl|String|プライバシーに関する声明の URL。 [managedEBook](../resources/intune-books-managedebook.md) から継承します|
|vppTokenId|Guid|Vpp トークン ID。|
|appleId|文字列|Vpp トークンに関連付けられている Apple ID。|
|vppOrganizationName|String|Vpp トークンの組織の名前。|
|genres|String コレクション|ジャンル。|
|language|String|言語。|
|seller|String|販売元。|
|totalLicenseCount|Int32|ライセンスの合計数。|
|usedLicenseCount|Int32|使用されているライセンスの数。|
|roleScopeTagIds|String collection|このエンティティインスタンスの範囲タグのリスト。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|categories|[managedebookcategory](../resources/intune-books-managedebookcategory.md)コレクション|この電子ブックのカテゴリのリスト。 [managedEBook](../resources/intune-books-managedebook.md) から継承します|
|assignments|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) コレクション|この電子ブックの割り当てのリストです。 [managedEBook](../resources/intune-books-managedebook.md) から継承します|
|installSummary|[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)|モバイル アプリ インストール概要です。 [managedEBook](../resources/intune-books-managedebook.md) から継承します|
|deviceStates|[deviceInstallState](../resources/intune-books-deviceinstallstate.md) コレクション|この電子ブックのインストール状態のリストです。 [managedEBook](../resources/intune-books-managedebook.md) から継承します|
|userStateSummary|[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) コレクション|この電子ブックのインストール状態のリストです。 [managedEBook](../resources/intune-books-managedebook.md) から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String",
  "vppTokenId": "Guid",
  "appleId": "String",
  "vppOrganizationName": "String",
  "genres": [
    "String"
  ],
  "language": "String",
  "seller": "String",
  "totalLicenseCount": 1024,
  "usedLicenseCount": 1024,
  "roleScopeTagIds": [
    "String"
  ]
}
```




