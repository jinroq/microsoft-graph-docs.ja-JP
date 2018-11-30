---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Permission
ms.openlocfilehash: 0a98080434dcb18944e58c2f1ada5019e3c32332
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023342"
---
# <a name="permission-resource-type"></a>permission リソースの種類

**permission** リソースは、[DriveItem](driveitem.md) リソースに付与された共有アクセス許可についての情報を提供します。

共有アクセス許可にはさまざまなフォームがあります。
**permission** リソースは、これらの異なるフォームをリソースのファセットを通じて表します。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "link",
    "grantedTo",
    "invitation",
    "inheritedFrom",
    "shareId"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.permission"
}-->
```json
{
  "id": "string (identifier)",
  "grantedTo": {"@odata.type": "microsoft.graph.identitySet"},
  "inheritedFrom": {"@odata.type": "microsoft.graph.itemReference"},
  "invitation": {"@odata.type": "microsoft.graph.sharingInvitation"},
  "link": {"@odata.type": "microsoft.graph.sharingLink"},
  "roles": ["string"],
  "shareId": "string"
}
```

## <a name="properties"></a>プロパティ

| プロパティ      | 型                                      | 説明
|:--------------|:------------------------------------------|:-----------------
| id            | String                                    | 項目の全アクセス許可の中の、アクセス許可の一意の識別子です。読み取り専用。
| grantedTo     | [IdentitySet](identityset.md)             | ユーザー タイプのアクセス許可、ユーザーとこのアクセス許可のアプリケーションの詳細。読み取り専用。
| invitation    | [SharingInvitation][]                     | このアクセス許可に任意に関連付けられた共有招待状の詳細情報です。読み取り専用。
| inheritedFrom | [ItemReference](itemreference.md)         | 現在のアクセス許可が先祖から継承されている場合、その先祖への参照を提供します。読み取り専用。
| link          | [SharingLink][]                           | 現在のアクセス許可がリンク タイプのアクセス許可である場合は、そのリンクの詳細を提供します。読み取り専用。
| roles         | Collection of String                      | `read` など、アクセス許可の種類。ロールの完全なリストは以下を参照してください。読み取り専用。
| shareId       | String                                    | [**共有** API](../api/shares-get.md) 経由で、この共有項目にアクセスするために使用できる一意のトークン。読み取り専用です。

permission リソースは、_ファセット_ を使用して、リソースによって表されるアクセス許可の種類に関する情報を提供します。

[**リンク**][SharingLink] ファセットのあるアクセス許可は、項目上に作成された共有リンクを表します。共有リンクは、リンクを持つすべてのユーザーの項目へのアクセス許可を提供する一意のトークンを含みます。

[**招待**][SharingInvitation] ファセットを持つアクセス許可は、特定のユーザーやグループをファイルへのアクセスへ招待することで追加されたアクセス許可を表します。

[SharingInvitation]: sharinginvitation.md
[SharingLink]: sharinglink.md

## <a name="roles-enumeration"></a>ロール列挙

| ロール        | 詳細                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | 項目のメタデータと内容を読み取る機能を提供します。            |
| `write`     | 項目のメタデータと内容の読み取りと変更の機能を提供します。 |
| `sp.owner`  | SharePoint および OneDrive for Business の場合、これは所有者ロールを表します。       |
| `sp.member` | SharePoint および OneDrive for Business の場合、これはメンバー ロールを表します。      |

## <a name="sharing-links"></a>共有リンク
最も一般的なアクセス許可の種類は、共有リンクです。
共有リンクは、共有されるリソースと、そのリソースへのアクセスを実現する認証トークンの両方を含む一意の URL を提供します。 ユーザーは、共有リンクによって共有されるコンテンツにアクセスするために、サインインする必要がありません。 ユーザーは、コンテンツへの読み取り専用アクセス権を付与するリンク、またはコンテンツへの書き込み可能なアクセス権を付与するリンクを共有できます。

### <a name="view-link"></a>表示リンク
表示リンクでは、項目への読み取り専用アクセスを提供します。

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-view-link" } -->
```json
{
  "id": "1",
  "roles": ["read"],
  "link": {
    "type": "view",
    "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
    "application": { "id": "1234", "displayName": "Sample Application" }
  },
  "shareId": "!LKj1lkdlals90j1nlkascl"
}
```

### <a name="edit-link"></a>編集リンク
編集リンクでは、項目への読み取りおよび書き込みアクセスを提供します。

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-edit-link" } -->
```json
{
  "id": "2",
  "roles": ["write"],
  "link": {
    "type": "edit",
    "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
    "application": { "id": "1234", "displayName": "Sample Application" }
  },
  "shareId": "!LKj1lkdlals90j1nlkascl"
}
```

### <a name="sharing-invitation"></a>共有の招待
共有リンクの作成に加えて、電子メール アドレスでユーザーを招待できます。
このシナリオでは、ユーザーの電子メールに送信される招待状がアクセス許可によって作成されます。

#### <a name="invitation-to-an-email-address"></a>電子メール アドレスへの招待状
アカウントが一致していないユーザーに電子メール アドレスでアクセス許可が送信された場合、**grantedTo** プロパティは、招待状が引き換えられるまで設定されません。招待状の引き換えは、ユーザーが初めてリンクをクリックしてサインインしたときに発生します。

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-invite-email" } -->
```json
{
  "id": "1",
  "roles": ["write"],
  "invitation": {
    "email": "jd@gmail.com",
    "signInRequired": true
  },
  "shareId": "FWxc1lasfdbEAGM5fI7B67aB5ZMPDMmQ11U"
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
    "email": "jd@outlook.com",
    "signInRequired": true
  },
  "shareId": "FWxc1lasfdbEAGM5fI7B67aB5ZMPDMmQ11U"
}
```

## <a name="methods"></a>メソッド

| Method                                                   | REST パス
|:---------------------------------------------------------|:-----------------------
| [アクセス許可を一覧表示する](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [アクセス許可を取得する](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| [追加する](../api/driveitem-invite.md)                        | `POST /drive/items/{item-id}/invite`
| [更新する](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [削除](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`


## <a name="remarks"></a>備考

OneDrive for Business と SharePoint ドキュメント ライブラリは、**inheritedFrom** プロパティを返しません。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The permission object provides information about permissions and roles and sharing information.",
  "keywords": "sharing,permissions,read,write,acl",
  "section": "documentation",
  "tocPath": "Resources/Permission"
} -->
