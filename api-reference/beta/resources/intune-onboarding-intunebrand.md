---
title: intuneBrand リソース タイプ
description: intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 812282fdbe6cc6bb329682ab3d95e8e036c512f0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374338"
---
# <a name="intunebrand-resource-type"></a>intuneBrand リソース タイプ

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
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
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|ロゴの背景色が明るいポータル サイト アプリに表示されるロゴ画像。|
|darkBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|ロゴの背景色が暗いポータル サイト アプリに表示されるロゴ画像。|
|showNameNextToLogo|Boolean|管理者が指定した表示名がロゴ画像のとなりに表示されるかどうかを表すブール値。|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md)|会社のポータルアプリのランディングページに表示されるカスタマイズ画像|
|customPrivacyMessage|String|カスタムプライバシーメッセージ。|
|isRemoveDeviceDisabled|Boolean|Adminsistrator が企業所有のデバイスで [デバイスの削除] アクションを無効にしているかどうかを表すブール値。|
|isFactoryResetDisabled|Boolean|Adminsistrator が企業所有のデバイスで "出荷時のリセット" アクションを無効にしているかどうかを表すブール値。|
|showDisplayNameNextToLogo|Boolean|管理者が指定した表示名がロゴ画像のとなりに表示されるかどうかを表すブール値。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.intuneBrand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrand",
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
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "darkBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "showNameNextToLogo": true,
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "customPrivacyMessage": "String",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true,
  "showDisplayNameNextToLogo": true
}
```



