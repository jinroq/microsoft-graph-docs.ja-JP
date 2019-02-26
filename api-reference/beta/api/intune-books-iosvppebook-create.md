---
title: iosVppEBook の作成
description: 新しい iosVppEBook オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bf780e1bc3bcb15392a6f2a1b164ef3c94ab1cc2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165220"
---
# <a name="create-iosvppebook"></a>iosVppEBook の作成

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

新しい [iosVppEBook](../resources/intune-books-iosvppebook.md) オブジェクトを作成します。

## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。

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
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、iosVppEBook オブジェクトの JSON 表記を指定します。

次の表に、iosVppEBook の作成時に必要になるプロパティを示します。

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
|roleScopeTagIds|String コレクション|このエンティティインスタンスの範囲タグのリスト。|



## <a name="response"></a>応答
成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosVppEBook](../resources/intune-books-iosvppebook.md) オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
Content-type: application/json
Content-length: 854

{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
  "appleId": "Apple Id value",
  "vppOrganizationName": "Vpp Organization Name value",
  "genres": [
    "Genres value"
  ],
  "language": "Language value",
  "seller": "Seller value",
  "totalLicenseCount": 1,
  "usedLicenseCount": 0,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1026

{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "id": "3b9f627e-627e-3b9f-7e62-9f3b7e629f3b",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
  "appleId": "Apple Id value",
  "vppOrganizationName": "Vpp Organization Name value",
  "genres": [
    "Genres value"
  ],
  "language": "Language value",
  "seller": "Seller value",
  "totalLicenseCount": 1,
  "usedLicenseCount": 0,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




