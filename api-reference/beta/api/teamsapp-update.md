---
title: アクセス許可
description: '以前に Microsoft Teams アプリカタログに発行したアプリを更新します。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2b9a16dc64557776eb6571ba3740249593684ba2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536854"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a>組織のアプリカタログに発行されたアプリを更新する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

以前に Microsoft Teams アプリカタログに発行した[アプリ](../resources/teamsapp.md)を更新します。 この API は、組織のアプリカタログ (テナントのアプリカタログ) に公開されたアプリを特に更新します。 組織のアプリカタログに発行するには、 `organization` teamsCatalogApp リソース**** の " [](../resources/teamsapp.md) " としてを指定します。

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
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a>要求ヘッダー

| ヘッダー        | 値           |
|:--------------|:--------------  |
| Authorization | ベアラー {トークン}。必須。  |
| Content-Type  | アプリケーション/zip |

## <a name="request-body"></a>要求本文

teams zip マニフェストペイロード: teams アプリケーション zip ファイルについ[ては、「アプリパッケージを作成する」を参照してください](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)。

>**注:** の[発行済みアプリの一覧](./teamsapp-list.md)から返された ID を使用して、更新するアプリを参照します。 zip アプリパッケージのマニフェストからの ID は使用しないでください。

## <a name="response"></a>応答

```
HTTP/1.1 204 No Content
```

## <a name="example"></a>例

### <a name="request"></a>要求

```
PUT https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

Teams アプリケーションの zip ファイルについては、 [「アプリパッケージの作成」を参照してください](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)。

### <a name="response"></a>応答

```
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/teamsapp-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
