---
title: OneNote REST API を使用する
description: 'Microsoft Graph を使用すると、アプリは個人または組織のアカウントでユーザーの OneNote ノートブック、セクション、および画面に正当にアクセスできます。 適切な代理アクセス許可またはアプリケーション アクセス許可を使用すると、アプリはサインインしているユーザーまたはテナント内のユーザーの OneNote データにアクセスできます。 '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: ceb5ac30786ecfd207a2076d471e9d004b60f8d3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462957"
---
# <a name="use-the-onenote-rest-api"></a>OneNote REST API を使用する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph を使用すると、アプリは個人または組織のアカウントでユーザーの OneNote ノートブック、セクション、および画面に正当にアクセスできます。 [適切な代理アクセス許可またはアプリケーション アクセス許可を使用すると](/graph/permissions-reference#notes-permissions)、アプリはサインインしているユーザーまたはテナント内のユーザーの OneNote データにアクセスできます。 

## <a name="root-url"></a>ルート URL
OneNote サービスのルート URL は、OneNote API へのすべての呼び出しで次の形式を使用します。
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

URL の `version` セグメントは、使用する Microsoft Graph のバージョンを示しています。

- 安定した運用コードには `v1.0` を使用します。
- 開発中の機能を試すには `beta` を使用します。 ベータ版のエンドポイントの特徴と機能は予告なしに変更されることがあります。運用コード内で使用することはお勧めしません。

Office 365 またはコンシューマー OneDrive のユーザー ノートブック、Office 365 のグループ ノートブック、または SharePoint サイトでホストされているチームのノートブックを場所として指定できます。 

![OneNote API 開発スタック](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a>ユーザー ノートブック
コンシューマー OneDrive または OneDrive for Business の個人用ノートブックにアクセスするには、次の URL のいずれかを使用します。

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- 現在のユーザーがアクセスできる OneNote コンテンツには `me` を使用します (所有と共有)。
- 指定されたユーザー (URL 内) が現在のユーザーと共有している OneNote コンテンツには `users/{id}` を使用します。 [ユーザー](users.md) API を使用します。
> **注:** `https://graph.microsoft.com/v1.0/users` で GET 要求を行うことにより、ユーザー ID を取得できます。

### <a name="group-notebooks"></a>グループ ノートブック

グループによって所有されているノートブックにアクセスするには、次のサービス ルート URL を使用します。

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a>SharePoint サイト ノートブック
SharePoint チーム サイトによって所有されているノートブックにアクセスするには、次のサービス ルート URL を使用します。

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
