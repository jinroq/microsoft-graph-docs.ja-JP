---
title: intuneBrandingProfile リソースの種類
description: このエンティティには、会社のポータル アプリケーションとエンド ・ ユーザーの web ポータルのテナントのレベルの外観をカスタマイズするために使用するデータが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b299964627a89598c28f15dfeed8ce6e13bede8c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411100"
---
# <a name="intunebrandingprofile-resource-type"></a>intuneBrandingProfile リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このエンティティには、会社のポータル アプリケーションとエンド ・ ユーザーの web ポータルのテナントのレベルの外観をカスタマイズするために使用するデータが含まれています。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト intuneBrandingProfiles](../api/intune-wip-intunebrandingprofile-list.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)コレクション|[IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトのプロパティと関係を一覧表示します。|
|[IntuneBrandingProfile を取得します。](../api/intune-wip-intunebrandingprofile-get.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|[IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトのプロパティと関係を参照してください。|
|[IntuneBrandingProfile を作成します。](../api/intune-wip-intunebrandingprofile-create.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|新しい[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトを作成します。|
|[IntuneBrandingProfile を削除します。](../api/intune-wip-intunebrandingprofile-delete.md)|なし|の[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)を削除します。|
|[IntuneBrandingProfile を更新します。](../api/intune-wip-intunebrandingprofile-update.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|[IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトのプロパティを更新します。|
|[assign action](../api/intune-wip-intunebrandingprofile-assign.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|プロファイル キー|
|profilename プロパティ|String|プロファイルの名前|
|profileDescription|String|プロファイルの説明|
|isDefaultProfile|Boolean|既定のプロファイルが使用される場合について説明します。|
|createdDateTime|DateTimeOffset|BrandingProfile が作成された日時です。|
|lastModifiedDateTime|DateTimeOffset|BrandingProfile の最終変更日時。|
|displayName|String|エンド ユーザーに表示される会社名または組織名。|
|contactITName|String|IT サポートを担当する個人名または組織名。|
|contactITPhoneNumber|String|IT サポートを担当する個人または組織の電話番号。|
|contactITEmailAddress|String|IT サポートを担当する個人または組織のメール アドレス。|
|contactITNotes|String|IT サポートを担当する個人または組織に関するテキスト コメント。|
|privacyUrl|String|会社または組織のプライバシー ポリシーの URL。|
|onlineSupportSiteUrl|String|会社または組織の IT ヘルプデスク サイトの URL。|
|onlineSupportSiteName|String|会社または組織の IT ヘルプデスク サイトの表示名。|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|会社のポータル アプリケーションと Web ポータルで使用する主要なテーマの色。|
|showLogo|Boolean|管理者が指定したロゴ画像が表示されるかどうかを表すブール値。|
|showDisplayNameNextToLogo|Boolean|管理者が指定した表示名がロゴ画像のとなりに表示されるかどうかを表すブール値。|
|themeColorLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|ロゴ イメージがテーマの背景色を会社のポータル アプリケーションに表示されます。|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|ロゴのイメージは明るい背景に会社のポータル アプリケーションに表示されます。|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md)|会社のポータル アプリケーションのランディング ページに表示されるカスタムのイメージ|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|assignments|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)コレクション|一連のブランド化のプロファイルの割り当てをグループ化します。|

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
  }
}
```




