---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Permission
ms.openlocfilehash: 195d4840fdb25339eda3858c0bac2395ee9b1c4a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073304"
---
# <a name="permission-resource-type"></a>リソースのアクセス許可の種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**アクセス許可**リソースは、 [driveItem](driveitem.md)リソースの共有権限に関する情報を提供します。

共有アクセス許可にはさまざまなフォームがあります。
**アクセス許可**リソースは、リソースの面でこれらの異なる形式を表します。

>**注:** ビジネスと SharePoint のドキュメント ライブラリの OneDrive では、 **inheritedFrom**プロパティは返されません。

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
| grantedToIdentities | コレクション ([IdentitySet][]) | リンクの種類のアクセス許可のアクセス許可の付与先ユーザーの詳細です。 読み取り専用。
| invitation          | [SharingInvitation][]       | このアクセス許可に任意に関連付けられた共有招待状の詳細情報です。読み取り専用。
| inheritedFrom       | [ItemReference][]           | 現在のアクセス許可が先祖から継承されている場合、その先祖への参照を提供します。読み取り専用。
| link                | [SharingLink][]             | 現在のアクセス許可がリンク タイプのアクセス許可である場合は、そのリンクの詳細を提供します。読み取り専用。
| roles               | Collection(String)          | `read` など、アクセス許可の種類。ロールの完全なリストは以下を参照してください。読み取り専用。
| shareId             | String                      | この**[API の共有][]** を使用して共有アイテムにアクセスするために使用できる一意なトークンです。 読み取り専用。
| expirationDateTime  | DateTimeOffset              | Yyyy の形式で MM の DateTimeOffset の ddTHH:mm:ssZ は、アクセス許可の有効期限を示します。 DateTime.MinValue を示しますがこのアクセス許可の有効期限が設定されていません。 省略可能。
| hasPassword         | ブール値                     | これは、応答でのみ表示されてパスワードがこのアクセス許可の設定があるかどうかを示します。 オプションおよび読み取り専用であり、OneDrive 個人のみです。

### <a name="roles-enumeration-values"></a>ロールの列挙値

| 値        | 詳細                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | 項目のメタデータと内容を読み取る機能を提供します。            |
| `write`     | 項目のメタデータと内容の読み取りと変更の機能を提供します。 |
| `sp.owner`  | SharePoint および OneDrive for Business の場合、これは所有者ロールを表します。       |
| `sp.member` | SharePoint および OneDrive for Business の場合、これはメンバー ロールを表します。      |

permission リソースは、_ファセット_ を使用して、リソースによって表されるアクセス許可の種類に関する情報を提供します。

共有リンクには、アイテムにアクセスするために必要な一意のトークンが含まれています。

[**招待**][SharingInvitation] ファセットを持つアクセス許可は、特定のユーザーやグループをファイルへのアクセスへ招待することで追加されたアクセス許可を表します。

## <a name="sharing-links"></a>共有リンク

[**リンク**][SharingLink]のファセットは、項目を作成したリンクを共有にアクセスを許可します。
これらは、最も一般的な種類のアクセス許可です。
共有リンクでは、ファイルまたはフォルダーへのアクセスに使用できる一意な URL を提供します。
それらは、さまざまな方法でアクセスを許可するを設定できます。
[CreateLink][] API を使用するには、組織にサインインしてすべてのユーザーに対して機能するリンクを作成するなど、サインインすることがなく、すべてのユーザーに適合するリンクを作成することができます。
[招待][]API を使用するか、会社にいるかどうかは、特定のユーザーに対してのみ機能するリンクを作成します。

リンクを共有するためのいくつかの例を次に示します。

### <a name="view-link"></a>ビューのリンク

このビューのリンクは、リンクを使用してすべてのユーザーに読み取り専用アクセスを提供します。

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

この [編集] リンクは、リンクを使用して組織内のすべてのユーザーに読み取りおよび書き込みアクセスを提供します。

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

### <a name="specific-people-link"></a>特定の人のリンク

このリンクで特定のユーザーに読み取りおよび書き込みアクセスを提供する、`grantedToIdentities`コレクションです。

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

[招待][]API によって送信されたアクセス許可は、[招待][SharingInvitation]ファセットの追加情報があります。
招待状は、既知のアカウントに一致しない電子メール アドレスに送信された、招待は、償還、最初にユーザーがリンクをクリックして、サインインが行われるまで、 **grantedTo**プロパティが設定できません。

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

| メソッド                                                   | REST パス
|:---------------------------------------------------------|:-----------------------
| [アクセス許可を一覧表示する](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [アクセス許可を取得する](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| [[作成] リンク][createLink]                                | `POST /drive/items/{item-id}/createLink`
| [人を招待][招待]                                  | `POST /drive/items/{item-id}/invite`
| [Update](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [削除](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`



[createLink]: ../api/driveitem-createlink.md
[IdentitySet]: identityset.md
[招待]: ../api/driveitem-invite.md
[ItemReference]: itemreference.md
[共有 API]: ../api/shares-get.md
[SharingInvitation]: sharinginvitation.md
[SharingLink]: sharinglink.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The permission object provides information about permissions and roles and sharing information.",
  "keywords": "sharing,permissions,read,write,acl",
  "section": "documentation",
  "tocPath": "Resources/Permission"
} -->
