---
title: intuneBrandingProfile リソースの種類
description: このエンティティにはデータが含まれており、これを使用して、会社のポータルアプリケーションとエンドユーザーの web ポータルのテナントレベルの外観をカスタマイズできます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f21cc97cd701f9826743475c4055aed6bafe9ca
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144703"
---
# <a name="intunebrandingprofile-resource-type"></a>intuneBrandingProfile リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このエンティティにはデータが含まれており、これを使用して、会社のポータルアプリケーションとエンドユーザーの web ポータルのテナントレベルの外観をカスタマイズできます。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト intuneBrandingProfiles](../api/intune-wip-intunebrandingprofile-list.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)コレクション|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[intuneBrandingProfile を取得する](../api/intune-wip-intunebrandingprofile-get.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[intuneBrandingProfile を作成する](../api/intune-wip-intunebrandingprofile-create.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|新しい[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトを作成します。|
|[intuneBrandingProfile の削除](../api/intune-wip-intunebrandingprofile-delete.md)|なし|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)を削除します。|
|[intuneBrandingProfile の更新](../api/intune-wip-intunebrandingprofile-update.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトのプロパティを更新します。|
|[assign action](../api/intune-wip-intunebrandingprofile-assign.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|プロファイルキー|
|profileName|String|プロファイルの名前|
|profiledescription|String|プロファイルの説明|
|isdefaultprofile|ブール値|既定でプロファイルが使用されているかどうかを示します。|
|createdDateTime|DateTimeOffset|BrandingProfile が作成されたとき。|
|lastModifiedDateTime|DateTimeOffset|BrandingProfile が最後に変更された日時。|
|displayName|String|エンド ユーザーに表示される会社名または組織名。|
|contactITName|String|IT サポートを担当する個人名または組織名。|
|contactITPhoneNumber|String|IT サポートを担当する個人または組織の電話番号。|
|contactITEmailAddress|String|IT サポートを担当する個人または組織のメール アドレス。|
|contactITNotes|String|IT サポートを担当する個人または組織に関するテキスト コメント。|
|privacyUrl|String|会社または組織のプライバシー ポリシーの URL。|
|onlineSupportSiteUrl|String|会社または組織の IT ヘルプデスク サイトの URL。|
|onlineSupportSiteName|String|会社または組織の IT ヘルプデスク サイトの表示名。|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|会社のポータル アプリケーションと Web ポータルで使用する主要なテーマの色。|
|showLogo|ブール値|管理者が指定したロゴ画像が表示されるかどうかを表すブール値。|
|showDisplayNameNextToLogo|Boolean|管理者が指定した表示名がロゴ画像のとなりに表示されるかどうかを表すブール値。|
|themeColorLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|テーマの色の背景にある、ポータルサイトアプリに表示されるロゴ画像。|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|明るい背景上に会社のポータルアプリに表示されるロゴ画像。|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md)|会社のポータルアプリのランディングページに表示されるカスタマイズ画像|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|assignments|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)コレクション|ブランド化プロファイルのグループの割り当てのリスト。|

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




