---
title: OneNote REST API を使用する
description: 'Graph では、個人または組織のアカウントのユーザーの OneNote ノートブック、セクション、およびページへのアクセスの認証を取得するアプリを使用できます。 適切な委任またはアプリケーションのアクセス許可をアプリがサインインしているユーザーや、テナント内のユーザーの OneNote のデータにアクセスできます。 '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 7db3024224dde7ee4c95d2e3840187709471cecd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525627"
---
# <a name="use-the-onenote-rest-api"></a>OneNote REST API を使用する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Graph では、個人または組織のアカウントのユーザーの OneNote ノートブック、セクション、およびページへのアクセスの認証を取得するアプリを使用できます。 アプリは、[委任、またはアプリケーションの適切なアクセス許可](/graph/permissions-reference#notes-permissions)では、サインイン中のユーザーや、テナント内のユーザーの OneNote のデータにアクセスできます。 

## <a name="root-url"></a>ルート URL
OneNote サービスのルート URL は、OneNote API へのすべての呼び出しで次の形式を使用します。
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

`version` 、URL 内のセグメントが使用する Microsoft Graph のバージョンを表します。

- 安定した運用コードには `v1.0` を使用します。
- 開発中の機能を試すには `beta` を使用します。 ベータの終了点で機能が変わることがあります。実行コードで使用することはお勧めしません。

Office 365 またはコンシューマー OneDrive のユーザー ノートブック、Office 365 のグループ ノートブック、または SharePoint サイトでホストされているチームのノートブックを場所として指定できます。 

![OneNote の API の開発履歴](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a>ユーザーのノートブック
OneDrive または OneDrive ビジネスの消費者の個人のノートブックにアクセスするには、次の Url のいずれかを使用します。

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- 現在のユーザーがアクセスできる OneNote コンテンツには `me` を使用します (所有と共有)。
- 指定されたユーザー (URL 内) が現在のユーザーと共有している OneNote コンテンツには `users/{id}` を使用します。 [ユーザー](users.md) API を使用します。
> **注:** `https://graph.microsoft.com/v1.0/users`で GET 要求を行うことにより、ユーザー ID を取得できます。

### <a name="group-notebooks"></a>グループ ノートブック

グループによって所有されているノートブックにアクセスするには、次のサービスのルート URL を使用します。

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a>SharePoint サイトのノートブック
SharePoint チーム サイトによって所有されているノートブックにアクセスするには、次のサービスのルート URL を使用します。

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenote-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
