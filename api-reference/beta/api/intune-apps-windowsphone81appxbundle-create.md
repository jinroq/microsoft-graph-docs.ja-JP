---
title: windowsPhone81AppXBundle を作成する
description: 新しい windowsPhone81AppXBundle オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e0c59bcfc3a976ea0ec077444f28e854e2da465
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32487848"
---
# <a name="create-windowsphone81appxbundle"></a>windowsPhone81AppXBundle を作成する

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

新しい[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)オブジェクトを作成します。

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
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、windowsPhone81AppXBundle オブジェクトの JSON 表記を指定します。

次の表に、windowsPhone81AppXBundle の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|エンティティのキー。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|displayName|String|管理者が提供またはインポートしたアプリのタイトル。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|説明|String|アプリの説明。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
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
|uploadState|Int32|アップロード状態。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|アプリの発行の状態。 アプリが発行されていない限り、アプリを割り当てることができません。 [mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。 使用可能な値は、`notPublished`、`processing`、`published` です。|
|isAssigned|Boolean|アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|roleScopeTagIds|String collection|このモバイルアプリの範囲タグ id のリスト。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|dependentappcount|Int32|子アプリが持つ依存関係の合計数。 [mobileApp](../resources/intune-apps-mobileapp.md) から継承します|
|committedContentVersion|String|内部にコミットされたコンテンツのバージョン。 [mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します|
|fileName|文字列型 (String)|メインの LOB アプリケーションのファイル名。 [mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します|
|size|Int64|アップロードされたすべてのファイルを含む合計サイズ。 [mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します|
|applicableArchitectures|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|このアプリを実行できる Windows アーキテクチャ。 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承されます。 可能な値は `none`、`x86`、`x64`、`arm`、`neutral`、`arm64` です。|
|identityName|String|ID 名。 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。|
|identityPublisherHash|String|ID の発行元のハッシュ。 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。|
|identityResourceIdentifier|String|ID のリソースの識別子。 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。|
|minimumSupportedOperatingSystem|[windowsMinimumOperatingSystem](../resources/intune-apps-windowsminimumoperatingsystem.md)|該当するオペレーティング システムの最小の値。 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。|
|phoneProductIdentifier|String|電話の製品識別子。 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。|
|phonePublisherId|String|電話の発行元 Id。 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承されます。|
|identityVersion|String|ID のバージョン。 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。|
|appXPackageInformationList|[windowspackageinformation](../resources/intune-apps-windowspackageinformation.md)コレクション|AppX パッケージ情報のリスト。|



## <a name="response"></a>応答
成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2211

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true
      }
    }
  ]
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2383

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
  "id": "2433be7c-be7c-2433-7cbe-33247cbe3324",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true
      }
    }
  ]
}
```





