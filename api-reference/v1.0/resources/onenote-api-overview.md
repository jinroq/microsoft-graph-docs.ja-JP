# <a name="use-the-onenote-rest-api"></a>OneNote REST API を使用する

Microsoft Graph では、個人または組織のアカウントのユーザーの OneNote ノートブック、セクション、およびページにアプリからアクセスする権限を取得できます。 [適切な代理アクセス許可またはアプリケーション アクセス許可](../../../concepts/permissions_reference.md#notes-permissions)を使用すると、アプリはサインインしているユーザーまたはテナント内のユーザーの OneNote データにアクセスできます。

## <a name="root-url"></a>ルート URL
OneNote サービスのルート URL は、OneNote API へのすべての呼び出しで次の形式を使用します。
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```
URL の `version` セグメントは、使用する Microsoft Graph のバージョンを示しています。

- `v1.0`  は、安定した製品コード用です。
- `beta`  は、開発中の機能を試すのに使用します。 ベータのエンドポイントで機能が変わることがあります。製品コードで使用することはお勧めしません。

Office 365 またはコンシューマー OneDrive のユーザー ノートブック、Office 365 のグループ ノートブック、または SharePoint サイトでホストされているチームのノートブックを場所として指定できます。 

![OneNote API の開発スタック](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a>ユーザーのノートブック
コンシューマー OneDrive または OneDrive for Business の個人用ノートブックにアクセスするには、次の URL のいずれかを使用します。

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- `me` は、現在のユーザーがアクセスできる OneNote コンテンツのためのものです (所有と共有)。
- `users/{id}` は、指定されたユーザー (URL 内) が現在のユーザーと共有している OneNote コンテンツのためのものです。 [ユーザー](users.md) API を使用します。
> **注:** `https://graph.microsoft.com/v1.0/users`で GET 要求を行うことにより、ユーザー ID を取得できます。

### <a name="group-notebooks"></a>グループ ノートブック
グループによって所有されているノートブックにアクセスするには、次のサービス ルート URL を使用します。

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a>SharePoint サイトのノートブック

SharePoint チーム サイトによって所有されているノートブックにアクセスするには、次のサービス ルート URL を使用します。

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

