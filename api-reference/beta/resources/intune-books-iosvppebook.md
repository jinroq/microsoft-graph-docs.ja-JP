---
title: iosVppEBook リソースの種類
description: iOS Vpp eBook のプロパティを含むクラスです。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 54940efc8fe6a87336ecb627fe817126191bbc9e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991689"
---
# <a name="iosvppebook-resource-type"></a>iosVppEBook リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

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
|id|文字列|エンティティのキー。 [managedEBook](../resources/intune-books-managedebook.md) から継承します|
|displayName|String|電子ブックの名前。 [managedEBook](../resources/intune-books-managedebook.md) から継承します|
|description|文字列型 (String)|説明。 [managedEBook](../resources/intune-books-managedebook.md) から継承します|
|publisher|String|発行元。 [managedEBook](../resources/intune-books-managedebook.md) から継承します|
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
|roleScopeTagIds|文字列コレクション|このエンティティインスタンスの範囲タグのリスト。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|categories|[Managedebookcategory](../resources/intune-books-managedebookcategory.md)コレクション|この電子ブックのカテゴリのリスト。 [managedEBook](../resources/intune-books-managedebook.md) から継承します|
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





