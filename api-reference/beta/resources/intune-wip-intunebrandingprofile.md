---
title: intuneBrandingProfile リソースの種類
description: このエンティティにはデータが含まれており、これを使用して、会社のポータルアプリケーションとエンドユーザーの web ポータルのテナントレベルの外観をカスタマイズできます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2beeedc1481a4ac01277b31a310fc7f9f30c261a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983555"
---
# <a name="intunebrandingprofile-resource-type"></a>intuneBrandingProfile リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このエンティティにはデータが含まれており、これを使用して、会社のポータルアプリケーションとエンドユーザーの web ポータルのテナントレベルの外観をカスタマイズできます。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト intuneBrandingProfiles](../api/intune-wip-intunebrandingprofile-list.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)コレクション|[IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[IntuneBrandingProfile を取得する](../api/intune-wip-intunebrandingprofile-get.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|[IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[IntuneBrandingProfile を作成する](../api/intune-wip-intunebrandingprofile-create.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|新しい[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトを作成します。|
|[IntuneBrandingProfile の削除](../api/intune-wip-intunebrandingprofile-delete.md)|None|[IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)を削除します。|
|[IntuneBrandingProfile の更新](../api/intune-wip-intunebrandingprofile-update.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|[IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトのプロパティを更新します。|
|[assign アクション](../api/intune-wip-intunebrandingprofile-assign.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|プロファイルキー|
|profileName|String|プロファイルの名前|
|profileDescription|String|プロファイルの説明|
|isDefaultProfile|Boolean|プロファイルが既定として使用されるかどうかを表すブール値|
|createdDateTime|DateTimeOffset|BrandingProfile が作成された時刻|
|lastModifiedDateTime|DateTimeOffset|BrandingProfile が最後に変更された時刻|
|displayName|String|エンドユーザーに表示される会社名または組織名|
|contactITName|String|IT サポートを担当する個人または組織の名前|
|contactITPhoneNumber|String|IT サポートを担当する個人または組織の電話番号|
|contactITEmailAddress|String|IT サポートを担当する個人または組織の電子メールアドレス|
|contactITNotes|String|IT サポートを担当する個人または組織に関するテキストコメント|
|privacyUrl|String|会社/組織のプライバシーポリシーの URL|
|onlineSupportSiteUrl|String|会社または組織の IT ヘルプデスクサイトへの URL|
|onlineSupportSiteName|String|会社/組織の IT ヘルプデスクサイトの表示名|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|会社のポータルアプリケーションと web ポータルで使用される主要なテーマの色|
|showLogo|Boolean|管理者が指定したロゴ画像が表示されるかどうかを表すブール値|
|showDisplayNameNextToLogo|Boolean|管理者が指定した表示名がロゴ画像の隣に表示されるかどうかを表すブール値|
|themeColorLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|ロゴの背景色がテーマになっている、ポータルサイトアプリに表示されるロゴ画像|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|ロゴの背景が明るい、ポータルサイトアプリに表示されるロゴ画像|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md)|会社のポータルアプリのランディングページに表示されるカスタマイズ画像|
|customPrivacyMessage|String|デバイスで管理者がアクセスできる内容に関するテキストコメント|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|assignments|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)コレクション|ブランド化プロファイルのグループ割り当ての一覧|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.intuneBrandingProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "String (identifier)",
  "profileName": "String",
  "profileDescription": "String",
  "isDefaultProfile": true,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "privacyUrl": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1024,
    "g": 1024,
    "b": 1024
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "customPrivacyMessage": "String"
}
```





