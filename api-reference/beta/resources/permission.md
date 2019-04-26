---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Permission
localization_priority: Normal
ms.openlocfilehash: 12390583dcb1a87a5c9492ae3dcbcb132a66f69c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568257"
---
# <a name="permission-resource-type"></a>permission リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**permission**リソースは、[ドライブ項目](driveitem.md)リソースに対して付与された共有アクセス許可に関する情報を提供します。

共有アクセス許可にはさまざまなフォームがあります。
**permission**リソースは、リソースのファセットを使用して、これらのさまざまなフォームを表します。

>**注:** OneDrive for business および SharePoint のドキュメントライブラリは、 **inheritedfrom**プロパティを返しません。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "link",
    "grantedTo",
    "grantedToIdentities",
    "invitation",
    "inheritedFrom",
    "shareId",
    "expirationDateTime",
    "hasPassword"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.permission"
}-->

```json
{
  "id": "string (identifier)",
  "grantedTo": {"@odata.type": "microsoft.graph.identitySet"},
  "grantedToIdentities": [{"@odata.type": "microsoft.graph.identitySet"}],
  "inheritedFrom": {"@odata.type": "microsoft.graph.itemReference"},
  "invitation": {"@odata.type": "microsoft.graph.sharingInvitation"},
  "link": {"@odata.type": "microsoft.graph.sharingLink"},
  "roles": ["string"],
  "shareId": "string",
  "expirationDateTime": "string (timestamp)",
  "hasPassword": "boolean"
}
```

## <a name="properties"></a>プロパティ

| プロパティ            | 型                        | 説明
|:--------------------|:----------------------------|:-------------------------
| id                  | String                      | 項目の全アクセス許可の中の、アクセス許可の一意の識別子です。読み取り専用。
| grantedTo           | [IdentitySet][]             | ユーザー タイプのアクセス許可、ユーザーとこのアクセス許可のアプリケーションの詳細。読み取り専用。
| grantedToIdentities | コレクション (id[セット][]) | リンクの種類のアクセス許可では、アクセス許可が付与されたユーザーの詳細。 読み取り専用。
| invitation          | [SharingInvitation][]       | このアクセス許可に任意に関連付けられた共有招待状の詳細情報です。読み取り専用。
| inheritedFrom       | [ItemReference][]           | 現在のアクセス許可が先祖から継承されている場合、その先祖への参照を提供します。読み取り専用。
| link                | [SharingLink][]             | 現在のアクセス許可がリンク タイプのアクセス許可である場合は、そのリンクの詳細を提供します。読み取り専用。
| roles               | Collection(String)          | `read` など、アクセス許可の種類。ロールの完全なリストは以下を参照してください。読み取り専用。
| shareId             | String                      | 共有**[API][]** を介してこの共有アイテムにアクセスするために使用できる一意のトークン。 読み取り専用。
| expirationDateTime  | DateTimeOffset              | yyyy-mm-yyyy-mm-ddthh: mm: ssz の形式は、アクセス許可の有効期限を示します。 MinValue は、このアクセス許可に有効期限が設定されていないことを示します。 省略可能。
| hasPassword         | Boolean                     | これは、このアクセス許可に対してパスワードが設定されているかどうかを示します。これは応答でのみ表示されます。 省略可能で、読み取り専用で、OneDrive 個人用のみです。

### <a name="roles-enumeration-values"></a>Roles 列挙値

| 値        | 詳細                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | 項目のメタデータと内容を読み取る機能を提供します。            |
| `write`     | 項目のメタデータと内容の読み取りと変更の機能を提供します。 |
| `sp.owner`  | SharePoint および OneDrive for Business の場合、これは所有者ロールを表します。       |
| `sp.member` | SharePoint および OneDrive for Business の場合、これはメンバー ロールを表します。      |

permission リソースは、_ファセット_ を使用して、リソースによって表されるアクセス許可の種類に関する情報を提供します。

共有リンクには、アイテムへのアクセスに必要な一意のトークンが含まれています。

[**招待**][SharingInvitation] ファセットを持つアクセス許可は、特定のユーザーやグループをファイルへのアクセスへ招待することで追加されたアクセス許可を表します。

## <a name="sharing-links"></a>共有リンク

[**リンク**][SharingLink] ファセットのあるアクセス許可は、項目上に作成された共有リンクを表します。
最も一般的なアクセス許可の種類を次に示します。
共有リンクは、ファイルまたはフォルダーへのアクセスに使用できる一意の URL を提供します。
さまざまな方法でアクセスを許可するように設定できます。
たとえば、 [createlink][] API を使用して、組織にサインインしているユーザーに対して機能するリンクを作成したり、サインインを必要とせずにすべてのユーザーに対して機能するリンクを作成したりできます。
[invite][] API を使用すると、社内にいるかどうかに関係なく、特定のユーザーに対してのみ機能するリンクを作成することができます。

共有リンクの例を次に示します。

### <a name="view-link"></a>表示リンク

このビューリンクは、リンクを持つすべてのユーザーに読み取り専用アクセスを提供します。

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-view-link" } -->

```json
{
  "id": "1",
  "roles": ["read"],
  "link": {
    "scope": "anonymous",
    "type": "view",
    "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
    "application": { "id": "1234", "displayName": "Sample Application" }
  },
  "shareId": "!LKj1lkdlals90j1nlkascl",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

### <a name="edit-link"></a>編集リンク

この編集リンクは、リンクを使用して組織内のすべてのユーザーに読み取り/書き込みアクセスを提供します。

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-edit-link" } -->

```json
{
  "id": "2ceefb3g32hh",
  "roles": ["write"],
  "link": {
    "scope": "organization",
    "type": "edit",
    "webUrl": "https://contoso.sharepoint.com/:w:/t/design/fj277ghautbb422707565gnvg23",
    "application": { "id": "1234", "displayName": "Sample Application" }
  },
  "shareId": "!LKj1lkdlals90j1nlkascl",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

### <a name="specific-people-link"></a>特定の人物リンク

このリンクにより、 `grantedToIdentities`コレクション内の特定のユーザーに対する読み取りおよび書き込みアクセス権が提供されます。

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-people-link" } -->

```json
{
  "id": "3",
  "grantedToIdentities": [
    {
       "user": {
        "id": "35fij1974gb8832",
        "displayName": "Misty Suarez"
      }
    },
    {
       "user": {
        "id": "9397721fh4hgh73",
        "displayName": "Judith Clemons"
      }
    }
  ],
  "roles": ["write"],
  "link": {
    "webUrl": "https://contoso.sharepoint.com/:w:/t/design/a577ghg9hgh737613bmbjf839026561fmzhsr85ng9f3hjck2t5s",
    "application": { "id": "1234", "displayName": "Sample Application" }
  },
  "shareId": "!LKj1lkdlals90j1nlkascl",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

## <a name="sharing-invitations"></a>共有への招待

[invite][] API によって送信されるアクセス許可には、[招待][sharinginvitation]ファセットに追加情報が含まれている場合があります。
招待状が既知のアカウントに一致しない電子メールアドレスに送信された場合、招待が引き換えられるまで、 **grantedTo**プロパティは設定されません。これは、ユーザーが最初にリンクをクリックしてサインインするときに発生します。

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-invite-email" } -->

```json
{
  "id": "1",
  "roles": ["write"],
  "invitation": {
    "email": "jd@fabrikam.com",
    "signInRequired": true
  },
  "shareId": "FWxc1lasfdbEAGM5fI7B67aB5ZMPDMmQ11U",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

ユーザーによって共有の招待状が引き換えられると、**grantedTo** プロパティにはアクセス許可を引き換えたアカウントに関する情報が格納されます。

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-invite-redeemed" } -->

```json
{
  "id": "1",
  "roles": ["write"],
  "grantedTo": {
    "user": {
      "id": "5D33DD65C6932946",
      "displayName": "John Doe"
    }
  },
  "invitation": {
    "email": "jd@fabrikam.com",
    "signInRequired": true
  },
  "shareId": "FWxc1lasfdbEAGM5fI7B67aB5ZMPDMmQ11U",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

## <a name="methods"></a>メソッド

| Method                                                   | REST パス
|:---------------------------------------------------------|:-----------------------
| [アクセス許可を一覧表示する](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [アクセス許可を取得する](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| [リンクの作成][createlink]                                | `POST /drive/items/{item-id}/createLink`
| [ユーザーを招待]する[invite]                                  | `POST /drive/items/{item-id}/invite`
| [更新する](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [削除](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`



[createLink]: ../api/driveitem-createlink.md
[IdentitySet]: identityset.md
[全員]: ../api/driveitem-invite.md
[ItemReference]: itemreference.md
[共有 API]: ../api/shares-get.md
[SharingInvitation]: sharinginvitation.md
[SharingLink]: sharinglink.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The permission object provides information about permissions and roles and sharing information.",
  "keywords": "sharing,permissions,read,write,acl",
  "section": "documentation",
  "tocPath": "Resources/Permission",
  "suppressions": [
    "Error: /api-reference/beta/resources/permission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
