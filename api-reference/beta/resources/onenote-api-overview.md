---
title: OneNote REST API を使用する
description: 'Microsoft Graph を使用すると、アプリはユーザーの OneNote ノートブック、セクション、および個人または組織のアカウントのページへの承認されたアクセス権を取得できます。 適切な委任またはアプリケーションのアクセス許可を持つアプリは、サインインしているユーザーまたはテナント内のユーザーの OneNote データにアクセスできます。 '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 7db3024224dde7ee4c95d2e3840187709471cecd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566046"
---
# <a name="use-the-onenote-rest-api"></a>OneNote REST API を使用する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph を使用すると、アプリはユーザーの OneNote ノートブック、セクション、および個人または組織のアカウントのページへの承認されたアクセス権を取得できます。 [適切な委任またはアプリケーションのアクセス許可](/graph/permissions-reference#notes-permissions)を持つアプリは、サインインしているユーザーまたはテナント内のユーザーの OneNote データにアクセスできます。 

## <a name="root-url"></a>ルート URL
OneNote サービスのルート URL は、OneNote API へのすべての呼び出しで次の形式を使用します。
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

URL `version`内のセグメントは、使用する Microsoft Graph のバージョンを表します。

- 安定した運用コードには `v1.0` を使用します。
- 開発中の機能を試すには `beta` を使用します。 ベータ版のエンドポイントの機能は変更される可能性があります。運用コードでは使用しないことをお勧めします。

この場所は、office 365 またはコンシューマー OneDrive、グループノートブック、または office 365 上の SharePoint サイトでホストされるチームノートブックのユーザーノートブックであることができます。 

![OneNote API 開発スタック](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a>ユーザーノートブック
コンシューマー onedrive または onedrive for business の個人用ノートブックにアクセスするには、次のいずれかの url を使用します。

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- 現在のユーザーがアクセスできる OneNote コンテンツには `me` を使用します (所有と共有)。
- 指定されたユーザー (URL 内) が現在のユーザーと共有している OneNote コンテンツには `users/{id}` を使用します。 [ユーザー](users.md) API を使用します。
> **注:** get 要求を行うことによって、ユーザー id `https://graph.microsoft.com/v1.0/users`を取得できます。

### <a name="group-notebooks"></a>グループノートブック

グループによって所有されているノートブックにアクセスするには、次のサービスルート URL を使用します。

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a>SharePoint サイトのノートブック
SharePoint チームサイトで所有されているノートブックにアクセスするには、次のサービスルート URL を使用します。

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
