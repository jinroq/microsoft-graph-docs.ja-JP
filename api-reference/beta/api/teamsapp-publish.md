---
title: アクセス許可
description: 'Microsoft Teams アプリカタログにアプリを発行します。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7acd916aa04200c626d8045e7da5a6d00be8a951
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544560"
---
# <a name="publish-apps-to-your-organizations-app-catalog"></a>組織のアプリカタログにアプリを発行する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Teams アプリカタログに[アプリ](../resources/teamsapp.md)を発行します。 具体的には、この API は、アプリを組織のカタログ (テナントのアプリカタログ) に公開します。作成されたリソース`distributionMethod`  =  `organization`には、があります。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)」を参照してください。

>**注:** この API は、グローバル管理者のみが呼び出すことができます。 

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

Teams の Zip マニフェストのペイロード。 Teams アプリケーションの zip ファイルについ[ては、「アプリパッケージを作成する」を参照してください](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)。 その組織の別のアプリと同じマニフェスト ID を持つ組織に対してアプリを作成することはできません。

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、 [teamsCatalogApp](../resources/teamsapp.md)オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

Microsoft Teams アプリケーション zip ファイルを作成する方法については、「[アプリパッケージを作成](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)する」を参照してください。 

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/teamsapp-publish.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
