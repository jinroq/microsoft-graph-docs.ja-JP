---
title: IntuneBrandingProfile を更新します。
description: IntuneBrandingProfile オブジェクトのプロパティを更新します。
ms.openlocfilehash: 094de592e0e8d80472f1b0c6ed3d751ac79ba863
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073793"
---
# <a name="update-intunebrandingprofile"></a>IntuneBrandingProfile を更新します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

[IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトのプロパティを更新します。
## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementApps.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文
要求の本文に[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトの JSON の形式を指定します。

[IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)を作成するときに必要なプロパティを次の表に示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|String|プロファイル キー|
|profilename プロパティ|String|プロファイルの名前|
|profileDescription|String|プロファイルの説明|
|isDefaultProfile|ブール値|既定のプロファイルが使用される場合について説明します。|
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



## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトです。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
Content-type: application/json
Content-length: 1209

{
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1,
    "g": 1,
    "b": 1
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1377

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "fcd6136c-136c-fcd6-6c13-d6fc6c13d6fc",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1,
    "g": 1,
    "b": 1
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```





