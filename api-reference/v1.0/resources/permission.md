---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: アクセス許可
localization_priority: Priority
description: Permission リソースでは、DriveItem リソースに付与された共有アクセス許可についての情報を提供します。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 95a5b9785285cd6286cf9ebefd8d62fa900c3d9d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035484"
---
# <a name="permission-resource-type"></a><span data-ttu-id="85a58-103">Permission リソース型</span><span class="sxs-lookup"><span data-stu-id="85a58-103">Permission resource type</span></span>

<span data-ttu-id="85a58-104">**Permission** リソースは、[DriveItem](driveitem.md) リソースに付与された共有アクセス許可についての情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="85a58-104">The **Permission** resource provides information about a sharing permission granted for a [DriveItem](driveitem.md) resource.</span></span>

<span data-ttu-id="85a58-105">共有アクセス許可にはさまざまなフォームがあります。</span><span class="sxs-lookup"><span data-stu-id="85a58-105">Sharing permissions have a number of different forms.</span></span>
<span data-ttu-id="85a58-106">**Permission** リソースは、これらのさまざまなフォームをリソースのファセットを通じて表します。</span><span class="sxs-lookup"><span data-stu-id="85a58-106">The **Permission** resource represents these different forms through facets on the resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="85a58-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="85a58-107">JSON representation</span></span>

<span data-ttu-id="85a58-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="85a58-108">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="85a58-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="85a58-109">Properties</span></span>

| <span data-ttu-id="85a58-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="85a58-110">Property</span></span>      | <span data-ttu-id="85a58-111">型</span><span class="sxs-lookup"><span data-stu-id="85a58-111">Type</span></span>                                      | <span data-ttu-id="85a58-112">説明</span><span class="sxs-lookup"><span data-stu-id="85a58-112">Description</span></span>
|:--------------|:------------------------------------------|:-----------------
| <span data-ttu-id="85a58-113">id</span><span class="sxs-lookup"><span data-stu-id="85a58-113">id</span></span>            | <span data-ttu-id="85a58-114">String</span><span class="sxs-lookup"><span data-stu-id="85a58-114">String</span></span>                                    | <span data-ttu-id="85a58-p102">項目の全アクセス許可の中の、アクセス許可の一意の識別子です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="85a58-p102">The unique identifier of the permission among all permissions on the item. Read-only.</span></span>
| <span data-ttu-id="85a58-117">grantedTo</span><span class="sxs-lookup"><span data-stu-id="85a58-117">grantedTo</span></span>     | [<span data-ttu-id="85a58-118">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="85a58-118">IdentitySet</span></span>](identityset.md)             | <span data-ttu-id="85a58-p103">ユーザー タイプのアクセス許可、ユーザーとこのアクセス許可のアプリケーションの詳細。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="85a58-p103">For user type permissions, the details of the users & applications for this permission. Read-only.</span></span>
| <span data-ttu-id="85a58-121">invitation</span><span class="sxs-lookup"><span data-stu-id="85a58-121">invitation</span></span>    | <span data-ttu-id="85a58-122">[SharingInvitation][]</span><span class="sxs-lookup"><span data-stu-id="85a58-122">[SharingInvitation][]</span></span>                     | <span data-ttu-id="85a58-p104">このアクセス許可に任意に関連付けられた共有招待状の詳細情報です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="85a58-p104">Details of any associated sharing invitation for this permission. Read-only.</span></span>
| <span data-ttu-id="85a58-125">inheritedFrom</span><span class="sxs-lookup"><span data-stu-id="85a58-125">inheritedFrom</span></span> | [<span data-ttu-id="85a58-126">ItemReference</span><span class="sxs-lookup"><span data-stu-id="85a58-126">ItemReference</span></span>](itemreference.md)         | <span data-ttu-id="85a58-p105">現在のアクセス許可が先祖から継承されている場合、その先祖への参照を提供します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="85a58-p105">Provides a reference to the ancestor of the current permission, if it is inherited from an ancestor. Read-only.</span></span>
| <span data-ttu-id="85a58-129">link</span><span class="sxs-lookup"><span data-stu-id="85a58-129">link</span></span>          | <span data-ttu-id="85a58-130">[SharingLink][]</span><span class="sxs-lookup"><span data-stu-id="85a58-130">[SharingLink][]</span></span>                           | <span data-ttu-id="85a58-p106">現在のアクセス許可がリンク タイプのアクセス許可である場合は、そのリンクの詳細を提供します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="85a58-p106">Provides the link details of the current permission, if it is a link type permissions. Read-only.</span></span>
| <span data-ttu-id="85a58-133">roles</span><span class="sxs-lookup"><span data-stu-id="85a58-133">roles</span></span>         | <span data-ttu-id="85a58-134">Collection of String</span><span class="sxs-lookup"><span data-stu-id="85a58-134">Collection of String</span></span>                      | <span data-ttu-id="85a58-p107">`read` など、アクセス許可の種類。ロールの完全なリストは以下を参照してください。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="85a58-p107">The type of permission, e.g. `read`. See below for the full list of roles. Read-only.</span></span>
| <span data-ttu-id="85a58-138">shareId</span><span class="sxs-lookup"><span data-stu-id="85a58-138">shareId</span></span>       | <span data-ttu-id="85a58-139">String</span><span class="sxs-lookup"><span data-stu-id="85a58-139">String</span></span>                                    | <span data-ttu-id="85a58-p108">
            [
            **共有** API](../api/shares-get.md) 経由で、この共有項目にアクセスするために使用できる一意のトークン。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="85a58-p108">A unique token that can be used to access this shared item via the [**shares** API](../api/shares-get.md). Read-only.</span></span>

<span data-ttu-id="85a58-142">permission リソースは、_ファセット_ を使用して、リソースによって表されるアクセス許可の種類に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="85a58-142">The permission resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="85a58-p109">[**リンク**][SharingLink] ファセットのあるアクセス許可は、項目上に作成された共有リンクを表します。共有リンクは、リンクを持つすべてのユーザーの項目へのアクセス許可を提供する一意のトークンを含みます。</span><span class="sxs-lookup"><span data-stu-id="85a58-p109">Permissions with a [**link**][SharingLink] facet represent sharing links created on the item. Sharing links contain a unique token that provides access to the item for anyone with the link.</span></span>

<span data-ttu-id="85a58-145">[**招待**][SharingInvitation] ファセットを持つアクセス許可は、特定のユーザーやグループをファイルへのアクセスへ招待することで追加されたアクセス許可を表します。</span><span class="sxs-lookup"><span data-stu-id="85a58-145">Permissions with an [**invitation**][SharingInvitation] facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

[SharingInvitation]: sharinginvitation.md
[SharingLink]: sharinglink.md

## <a name="roles-enumeration"></a><span data-ttu-id="85a58-148">ロール列挙</span><span class="sxs-lookup"><span data-stu-id="85a58-148">Roles enumeration</span></span>

| <span data-ttu-id="85a58-149">ロール</span><span class="sxs-lookup"><span data-stu-id="85a58-149">Role</span></span>        | <span data-ttu-id="85a58-150">詳細</span><span class="sxs-lookup"><span data-stu-id="85a58-150">Details</span></span>                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | <span data-ttu-id="85a58-151">項目のメタデータと内容を読み取る機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="85a58-151">Provides the ability to read the metadata and contents of the item.</span></span>            |
| `write`     | <span data-ttu-id="85a58-152">項目のメタデータと内容の読み取りと変更の機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="85a58-152">Provides the ability to read and modify the metadata and contents of the item.</span></span> |
| `sp.owner`  | <span data-ttu-id="85a58-153">SharePoint および OneDrive for Business の場合、これは所有者ロールを表します。</span><span class="sxs-lookup"><span data-stu-id="85a58-153">For SharePoint and OneDrive for Business this represents the owner role.</span></span>       |
| `sp.member` | <span data-ttu-id="85a58-154">SharePoint および OneDrive for Business の場合、これはメンバー ロールを表します。</span><span class="sxs-lookup"><span data-stu-id="85a58-154">For SharePoint and OneDrive for Business this represents the member role.</span></span>      |

## <a name="sharing-links"></a><span data-ttu-id="85a58-155">共有リンク</span><span class="sxs-lookup"><span data-stu-id="85a58-155">Sharing links</span></span>
<span data-ttu-id="85a58-p110">最も一般的なアクセス許可の種類は、共有リンクです。 共有リンクは、共有されるリソースと、そのリソースへのアクセスを実現する認証トークンの両方を含む一意の URL を提供します。 ユーザーは、共有リンクによって共有されるコンテンツにアクセスするために、サインインする必要がありません。 ユーザーは、コンテンツへの読み取り専用アクセス権を付与するリンク、またはコンテンツへの書き込み可能なアクセス権を付与するリンクを共有できます。</span><span class="sxs-lookup"><span data-stu-id="85a58-p110">The most common type of permissions are sharing links. Sharing links provide a unique URL that includes both the resource being shared and an authentication token that provides access to the resource. Users don't need to sign-in to access the content shared with a sharing link. Users can share a link that gives read-only access to the content or writable access to the content.</span></span>

### <a name="view-link"></a><span data-ttu-id="85a58-160">表示リンク</span><span class="sxs-lookup"><span data-stu-id="85a58-160">View Link</span></span>
<span data-ttu-id="85a58-161">表示リンクでは、項目への読み取り専用アクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="85a58-161">A view link provides read-only access to an item.</span></span>

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

### <a name="edit-link"></a><span data-ttu-id="85a58-162">編集リンク</span><span class="sxs-lookup"><span data-stu-id="85a58-162">Edit link</span></span>
<span data-ttu-id="85a58-163">編集リンクでは、項目への読み取りおよび書き込みアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="85a58-163">An edit link provides read and write access to an item.</span></span>

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

### <a name="sharing-invitation"></a><span data-ttu-id="85a58-164">共有の招待</span><span class="sxs-lookup"><span data-stu-id="85a58-164">Sharing Invitation</span></span>
<span data-ttu-id="85a58-p111">共有リンクの作成に加えて、電子メール アドレスでユーザーを招待できます。 このシナリオでは、ユーザーの電子メールに送信される招待状がアクセス許可によって作成されます。</span><span class="sxs-lookup"><span data-stu-id="85a58-p111">In addition to creating sharing links, a user can be invited by e-mail address. In this scenario the permission creates an invitation that is sent to the user's email.</span></span>

#### <a name="invitation-to-an-email-address"></a><span data-ttu-id="85a58-167">電子メール アドレスへの招待状</span><span class="sxs-lookup"><span data-stu-id="85a58-167">Invitation to an email address</span></span>
<span data-ttu-id="85a58-168">アカウントが一致していないユーザーに電子メール アドレスでアクセス許可が送信された場合、**grantedTo** プロパティは、招待状が引き換えられるまで設定されません。招待状の引き換えは、ユーザーが初めてリンクをクリックしてサインインしたときに発生します。</span><span class="sxs-lookup"><span data-stu-id="85a58-168">If the permission was sent via an email address to a recipient who does not have a matching account, the **grantedTo** property may not be set until the invitation is redeemed, which occurs the first time a user clicks the link and signs in.</span></span>

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

<span data-ttu-id="85a58-169">ユーザーによって共有の招待状が引き換えられると、**grantedTo** プロパティにはアクセス許可を引き換えたアカウントに関する情報が格納されます。</span><span class="sxs-lookup"><span data-stu-id="85a58-169">After the sharing invitation has been redeemed by a user, the **grantedTo** property will contain the information about the account that redeemed the permissions:</span></span>

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

## <a name="methods"></a><span data-ttu-id="85a58-170">メソッド</span><span class="sxs-lookup"><span data-stu-id="85a58-170">Methods</span></span>

| <span data-ttu-id="85a58-171">Method</span><span class="sxs-lookup"><span data-stu-id="85a58-171">Method</span></span>                                                   | <span data-ttu-id="85a58-172">REST パス</span><span class="sxs-lookup"><span data-stu-id="85a58-172">REST Path</span></span>
|:---------------------------------------------------------|:-----------------------
| [<span data-ttu-id="85a58-173">アクセス許可を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="85a58-173">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="85a58-174">アクセス許可を取得する</span><span class="sxs-lookup"><span data-stu-id="85a58-174">Get permission</span></span>](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="85a58-175">追加する</span><span class="sxs-lookup"><span data-stu-id="85a58-175">Add</span></span>](../api/driveitem-invite.md)                        | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="85a58-176">更新する</span><span class="sxs-lookup"><span data-stu-id="85a58-176">Update</span></span>](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="85a58-177">削除</span><span class="sxs-lookup"><span data-stu-id="85a58-177">Delete</span></span>](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`


## <a name="remarks"></a><span data-ttu-id="85a58-178">備考</span><span class="sxs-lookup"><span data-stu-id="85a58-178">Remarks</span></span>

<span data-ttu-id="85a58-179">OneDrive for Business と SharePoint ドキュメント ライブラリは、**inheritedFrom** プロパティを返しません。</span><span class="sxs-lookup"><span data-stu-id="85a58-179">OneDrive for Business and SharePoint document libraries do not return the **inheritedFrom** property.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The permission object provides information about permissions and roles and sharing information.",
  "keywords": "sharing,permissions,read,write,acl",
  "section": "documentation",
  "tocPath": "Resources/Permission"
} -->
