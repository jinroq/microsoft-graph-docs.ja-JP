---
title: OneNote REST API を使用する
description: Graph では、個人または組織のアカウントのユーザーの OneNote ノートブック、セクション、およびページへのアクセスの認証を取得するアプリを使用できます。 適切な委任またはアプリケーションのアクセス許可をアプリがサインインしているユーザーや、テナント内のユーザーの OneNote のデータにアクセスできます。
ms.openlocfilehash: c439e7896eea85e84d567e54aaa57bb5191a70d2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020605"
---
# <a name="use-the-onenote-rest-api"></a>OneNote REST API を使用する

Graph では、個人または組織のアカウントのユーザーの OneNote ノートブック、セクション、およびページへのアクセスの認証を取得するアプリを使用できます。 アプリは、[委任、またはアプリケーションの適切なアクセス許可](/graph/permissions-reference#notes-permissions)では、サインイン中のユーザーや、テナント内のユーザーの OneNote のデータにアクセスできます。

## <a name="root-url"></a>ルート URL
OneNote サービスのルート URL は、OneNote API へのすべての呼び出しで次の形式を使用します。
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```
`version` 、URL 内のセグメントが使用する Microsoft Graph のバージョンを表します。

- 安定した運用コードには `v1.0` を使用します。
- 開発中の機能を試すには `beta` を使用します。 ベータの終了点で機能が変わることがあります。実行コードで使用することはお勧めしません。

場所には、Office 365 またはコンシューマー OneDrive 上のユーザーのノートブック、ノートブックのグループ、または Office 365 で SharePoint サイトでホストされているチームのノートブックを指定できます。 

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
> **注:** GET 要求を行うと、ユーザー Id を取得することができます`https://graph.microsoft.com/v1.0/users`。

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

