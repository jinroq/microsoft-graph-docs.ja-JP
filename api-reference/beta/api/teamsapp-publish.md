---
title: アクセス許可
description: 'マイクロソフト チーム アプリケーション カタログにアプリケーションを発行します。 '
author: nkramer
ms.openlocfilehash: 01d552a013b3d1324893bd775611e797253ff261
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335197"
---
# <a name="publish-apps-to-your-organizations-app-catalog"></a>アプリケーションを組織のアプリケーションのカタログに発行します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

マイクロソフト チーム アプリケーション カタログに[アプリケーション](../resources/teamsapp.md)を発行します。 この API が、アプリケーションを公開して、組織のカタログ (テナント アプリケーション カタログ) に具体的には、作成されたリソースがある`distributionMethod`  =  `organization`。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)」を参照してください。

>**注:** グローバル管理者だけでは、この API を呼び出すことができます。 

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)|
|:----------------------------------     |:-------------|
| 委任 (職場または学校のアカウント)     | AppCatalog.ReadWrite.All |
| 委任 (個人用 Microsoft アカウント) | サポートされていません|
| アプリケーション                            | 非サポート|

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a>要求ヘッダー

| ヘッダー        | 値           |
|:--------------|:--------------  |
| Authorization | ベアラー {トークン}。必須。  |
| Content-Type  | アプリケーション/zip |

## <a name="request-body"></a>要求本文

チーム Zip のマニフェスト ペイロード。 チームのアプリケーションのファイルは[、アプリケーション パッケージの作成を参照してください](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)zip 形式で圧縮します。 その組織の別のアプリケーションと同じマニフェスト ID を持つ組織のアプリケーションを作成することはできません。

## <a name="response"></a>応答

かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードと[teamsCatalogApp](../resources/teamsapp.md)オブジェクトです。

## <a name="example"></a>例

### <a name="request"></a>要求

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

マイクロソフト チームのアプリケーションの zip ファイルを作成する方法の詳細については、[作成されたアプリケーション パッケージ](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)を参照してください。 

### <a name="response"></a>応答

```
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
  "externalId": "b5561ec9-8cab-4aa3-8aa2-d8d7172e4311",
  "name": "Test App",
  "version": "1.0.0",
  "distributionMethod": "organization"
}
```
