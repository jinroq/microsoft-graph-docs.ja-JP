---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Permission
localization_priority: Normal
ms.openlocfilehash: 6a5a0af9c95900232ff87aa7aedb731a83a91cc5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518850"
---
# <a name="permission-resource-type"></a><span data-ttu-id="bf2fa-102">Permission リソース型</span><span class="sxs-lookup"><span data-stu-id="bf2fa-102">permission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf2fa-103">**permission** リソースは、[DriveItem](driveitem.md) リソースに付与された共有アクセス許可についての情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-103">The **permission** resource provides information about a sharing permission granted for a [driveItem](driveitem.md) resource.</span></span>

<span data-ttu-id="bf2fa-104">共有アクセス許可にはさまざまなフォームがあります。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-104">Sharing permissions have a number of different forms.</span></span>
<span data-ttu-id="bf2fa-105">**permission** リソースは、これらの異なるフォームをリソースのファセットを通じて表します。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-105">The **permission** resource represents these different forms through facets on the resource.</span></span>

><span data-ttu-id="bf2fa-106">**注:** ビジネスと SharePoint のドキュメント ライブラリの OneDrive では、 **inheritedFrom**プロパティは返されません。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-106">**Note:** OneDrive for Business and SharePoint document libraries do not return the **inheritedFrom** property.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf2fa-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bf2fa-107">JSON representation</span></span>

<span data-ttu-id="bf2fa-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="bf2fa-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf2fa-109">Properties</span></span>

| <span data-ttu-id="bf2fa-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf2fa-110">Property</span></span>            | <span data-ttu-id="bf2fa-111">型</span><span class="sxs-lookup"><span data-stu-id="bf2fa-111">Type</span></span>                        | <span data-ttu-id="bf2fa-112">説明</span><span class="sxs-lookup"><span data-stu-id="bf2fa-112">Description</span></span>
|:--------------------|:----------------------------|:-------------------------
| <span data-ttu-id="bf2fa-113">id</span><span class="sxs-lookup"><span data-stu-id="bf2fa-113">id</span></span>                  | <span data-ttu-id="bf2fa-114">String</span><span class="sxs-lookup"><span data-stu-id="bf2fa-114">String</span></span>                      | <span data-ttu-id="bf2fa-p102">項目の全アクセス許可の中の、アクセス許可の一意の識別子です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-p102">The unique identifier of the permission among all permissions on the item. Read-only.</span></span>
| <span data-ttu-id="bf2fa-117">grantedTo</span><span class="sxs-lookup"><span data-stu-id="bf2fa-117">grantedTo</span></span>           | <span data-ttu-id="bf2fa-118">[IdentitySet][]</span><span class="sxs-lookup"><span data-stu-id="bf2fa-118">[IdentitySet][]</span></span>             | <span data-ttu-id="bf2fa-p103">ユーザー タイプのアクセス許可、ユーザーとこのアクセス許可のアプリケーションの詳細。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-p103">For user type permissions, the details of the users & applications for this permission. Read-only.</span></span>
| <span data-ttu-id="bf2fa-121">grantedToIdentities</span><span class="sxs-lookup"><span data-stu-id="bf2fa-121">grantedToIdentities</span></span> | <span data-ttu-id="bf2fa-122">コレクション ([IdentitySet][])</span><span class="sxs-lookup"><span data-stu-id="bf2fa-122">Collection([IdentitySet][])</span></span> | <span data-ttu-id="bf2fa-123">リンクの種類のアクセス許可のアクセス許可の付与先ユーザーの詳細です。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-123">For link type permissions, the details of the users to whom permission was granted.</span></span> <span data-ttu-id="bf2fa-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-124">Read-only.</span></span>
| <span data-ttu-id="bf2fa-125">invitation</span><span class="sxs-lookup"><span data-stu-id="bf2fa-125">invitation</span></span>          | <span data-ttu-id="bf2fa-126">[SharingInvitation][]</span><span class="sxs-lookup"><span data-stu-id="bf2fa-126">[SharingInvitation][]</span></span>       | <span data-ttu-id="bf2fa-p105">このアクセス許可に任意に関連付けられた共有招待状の詳細情報です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-p105">Details of any associated sharing invitation for this permission. Read-only.</span></span>
| <span data-ttu-id="bf2fa-129">inheritedFrom</span><span class="sxs-lookup"><span data-stu-id="bf2fa-129">inheritedFrom</span></span>       | <span data-ttu-id="bf2fa-130">[ItemReference][]</span><span class="sxs-lookup"><span data-stu-id="bf2fa-130">[ItemReference][]</span></span>           | <span data-ttu-id="bf2fa-p106">現在のアクセス許可が先祖から継承されている場合、その先祖への参照を提供します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-p106">Provides a reference to the ancestor of the current permission, if it is inherited from an ancestor. Read-only.</span></span>
| <span data-ttu-id="bf2fa-133">link</span><span class="sxs-lookup"><span data-stu-id="bf2fa-133">link</span></span>                | <span data-ttu-id="bf2fa-134">[SharingLink][]</span><span class="sxs-lookup"><span data-stu-id="bf2fa-134">[SharingLink][]</span></span>             | <span data-ttu-id="bf2fa-p107">現在のアクセス許可がリンク タイプのアクセス許可である場合は、そのリンクの詳細を提供します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-p107">Provides the link details of the current permission, if it is a link type permissions. Read-only.</span></span>
| <span data-ttu-id="bf2fa-137">roles</span><span class="sxs-lookup"><span data-stu-id="bf2fa-137">roles</span></span>               | <span data-ttu-id="bf2fa-138">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="bf2fa-138">Collection(String)</span></span>          | <span data-ttu-id="bf2fa-p108">`read` など、アクセス許可の種類。ロールの完全なリストは以下を参照してください。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-p108">The type of permission, e.g. `read`. See below for the full list of roles. Read-only.</span></span>
| <span data-ttu-id="bf2fa-142">shareId</span><span class="sxs-lookup"><span data-stu-id="bf2fa-142">shareId</span></span>             | <span data-ttu-id="bf2fa-143">String</span><span class="sxs-lookup"><span data-stu-id="bf2fa-143">String</span></span>                      | <span data-ttu-id="bf2fa-p109">**[共有][] API** 経由で、この共有項目にアクセスするために使用できる一意のトークン。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-p109">A unique token that can be used to access this shared item via the **[shares API][]**. Read-only.</span></span>
| <span data-ttu-id="bf2fa-146">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bf2fa-146">expirationDateTime</span></span>  | <span data-ttu-id="bf2fa-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf2fa-147">DateTimeOffset</span></span>              | <span data-ttu-id="bf2fa-148">Yyyy の形式で MM の DateTimeOffset の ddTHH:mm:ssZ は、アクセス許可の有効期限を示します。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-148">A format of yyyy-MM-ddTHH:mm:ssZ of DateTimeOffset indicates the expiration time of the permission.</span></span> <span data-ttu-id="bf2fa-149">DateTime.MinValue を示しますがこのアクセス許可の有効期限が設定されていません。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-149">DateTime.MinValue indicates there is no expiration set for this permission.</span></span> <span data-ttu-id="bf2fa-150">省略可能。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-150">Optional.</span></span>
| <span data-ttu-id="bf2fa-151">HasPassword</span><span class="sxs-lookup"><span data-stu-id="bf2fa-151">hasPassword</span></span>         | <span data-ttu-id="bf2fa-152">ブール値</span><span class="sxs-lookup"><span data-stu-id="bf2fa-152">Boolean</span></span>                     | <span data-ttu-id="bf2fa-153">これは、応答でのみ表示されてパスワードがこのアクセス許可の設定があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-153">This indicates whether password is set for this permission, it's only showing in response.</span></span> <span data-ttu-id="bf2fa-154">オプションおよび読み取り専用であり、OneDrive 個人のみです。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-154">Optional and Read-only and for OneDrive Personal only.</span></span>

### <a name="roles-enumeration-values"></a><span data-ttu-id="bf2fa-155">ロールの列挙値</span><span class="sxs-lookup"><span data-stu-id="bf2fa-155">Roles enumeration values</span></span>

| <span data-ttu-id="bf2fa-156">値</span><span class="sxs-lookup"><span data-stu-id="bf2fa-156">Value</span></span>        | <span data-ttu-id="bf2fa-157">詳細</span><span class="sxs-lookup"><span data-stu-id="bf2fa-157">Details</span></span>                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | <span data-ttu-id="bf2fa-158">項目のメタデータと内容を読み取る機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-158">Provides the ability to read the metadata and contents of the item.</span></span>            |
| `write`     | <span data-ttu-id="bf2fa-159">項目のメタデータと内容の読み取りと変更の機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-159">Provides the ability to read and modify the metadata and contents of the item.</span></span> |
| `sp.owner`  | <span data-ttu-id="bf2fa-160">SharePoint および OneDrive for Business の場合、これは所有者ロールを表します。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-160">For SharePoint and OneDrive for Business this represents the owner role.</span></span>       |
| `sp.member` | <span data-ttu-id="bf2fa-161">SharePoint および OneDrive for Business の場合、これはメンバー ロールを表します。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-161">For SharePoint and OneDrive for Business this represents the member role.</span></span>      |

<span data-ttu-id="bf2fa-162">permission リソースは、_ファセット_ を使用して、リソースによって表されるアクセス許可の種類に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-162">The permission resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="bf2fa-163">共有リンクには、アイテムにアクセスするために必要な一意のトークンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-163">Sharing links contain a unique token required to access the item.</span></span>

<span data-ttu-id="bf2fa-164">[**招待**][SharingInvitation] ファセットを持つアクセス許可は、特定のユーザーやグループをファイルへのアクセスへ招待することで追加されたアクセス許可を表します。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-164">Permissions with an [**invitation**][SharingInvitation] facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

## <a name="sharing-links"></a><span data-ttu-id="bf2fa-165">共有リンク</span><span class="sxs-lookup"><span data-stu-id="bf2fa-165">Sharing links</span></span>

<span data-ttu-id="bf2fa-166">[**リンク**][SharingLink]のファセットは、項目を作成したリンクを共有にアクセスを許可します。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-166">Permissions with a [**link**][SharingLink] facet represent sharing links created on the item.</span></span>
<span data-ttu-id="bf2fa-167">これらは、最も一般的な種類のアクセス許可です。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-167">These are the most common kinds of permissions.</span></span>
<span data-ttu-id="bf2fa-168">共有リンクでは、ファイルまたはフォルダーへのアクセスに使用できる一意な URL を提供します。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-168">Sharing links provide a unique URL that can be used to access a file or folder.</span></span>
<span data-ttu-id="bf2fa-169">それらは、さまざまな方法でアクセスを許可するを設定できます。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-169">They can be set up to grant access in a variety of ways.</span></span>
<span data-ttu-id="bf2fa-170">[CreateLink][] API を使用するには、組織にサインインしてすべてのユーザーに対して機能するリンクを作成するなど、サインインすることがなく、すべてのユーザーに適合するリンクを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-170">For example, you can use the [createLink][] API to create a link that works for anyone signed into your organization, or you can create a link that works for anyone, without needing to sign in.</span></span>
<span data-ttu-id="bf2fa-171">[招待][]API を使用するか、会社にいるかどうかは、特定のユーザーに対してのみ機能するリンクを作成します。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-171">You can use the [invite][] API to create a link that only works for specific people, whether they're in your company or not.</span></span>

<span data-ttu-id="bf2fa-172">リンクを共有するためのいくつかの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-172">Here are some examples of sharing links.</span></span>

### <a name="view-link"></a><span data-ttu-id="bf2fa-173">表示リンク</span><span class="sxs-lookup"><span data-stu-id="bf2fa-173">View link</span></span>

<span data-ttu-id="bf2fa-174">このビューのリンクは、リンクを使用してすべてのユーザーに読み取り専用アクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-174">This view link provides read-only access to anyone with the link.</span></span>

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

### <a name="edit-link"></a><span data-ttu-id="bf2fa-175">編集リンク</span><span class="sxs-lookup"><span data-stu-id="bf2fa-175">Edit link</span></span>

<span data-ttu-id="bf2fa-176">この [編集] リンクは、リンクを使用して組織内のすべてのユーザーに読み取りおよび書き込みアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-176">This edit link provides read and write access to anyone in the organization with the link.</span></span>

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

### <a name="specific-people-link"></a><span data-ttu-id="bf2fa-177">特定の人のリンク</span><span class="sxs-lookup"><span data-stu-id="bf2fa-177">Specific people link</span></span>

<span data-ttu-id="bf2fa-178">このリンクで特定のユーザーに読み取りおよび書き込みアクセスを提供する、`grantedToIdentities`コレクションです。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-178">This link provides read and write access to the specific people in the `grantedToIdentities` collection.</span></span>

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

## <a name="sharing-invitations"></a><span data-ttu-id="bf2fa-179">共有への招待</span><span class="sxs-lookup"><span data-stu-id="bf2fa-179">Sharing invitations</span></span>

<span data-ttu-id="bf2fa-180">[招待][]API によって送信されたアクセス許可は、[招待][SharingInvitation]ファセットの追加情報があります。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-180">Permissions sent by the [invite][] API may have additional information in the [invitation][SharingInvitation] facet.</span></span>
<span data-ttu-id="bf2fa-181">招待状は、既知のアカウントに一致しない電子メール アドレスに送信された、招待は、償還、最初にユーザーがリンクをクリックして、サインインが行われるまで、 **grantedTo**プロパティが設定できません。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-181">If an invitation was sent to an email address that doesn't match a known account, the **grantedTo** property may not be set until the invitation is redeemed, which occurs the first time the user clicks the link and signs in.</span></span>

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

<span data-ttu-id="bf2fa-182">ユーザーによって共有の招待状が引き換えられると、**grantedTo** プロパティにはアクセス許可を引き換えたアカウントに関する情報が格納されます。</span><span class="sxs-lookup"><span data-stu-id="bf2fa-182">After the sharing invitation has been redeemed by a user, the **grantedTo** property will contain the information about the account that redeemed the permissions:</span></span>

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

## <a name="methods"></a><span data-ttu-id="bf2fa-183">メソッド</span><span class="sxs-lookup"><span data-stu-id="bf2fa-183">Methods</span></span>

| <span data-ttu-id="bf2fa-184">メソッド</span><span class="sxs-lookup"><span data-stu-id="bf2fa-184">Method</span></span>                                                   | <span data-ttu-id="bf2fa-185">REST パス</span><span class="sxs-lookup"><span data-stu-id="bf2fa-185">REST Path</span></span>
|:---------------------------------------------------------|:-----------------------
| [<span data-ttu-id="bf2fa-186">アクセス許可を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="bf2fa-186">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="bf2fa-187">アクセス許可を取得する</span><span class="sxs-lookup"><span data-stu-id="bf2fa-187">Get permission</span></span>](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| <span data-ttu-id="bf2fa-188">[[作成] リンク][createLink]</span><span class="sxs-lookup"><span data-stu-id="bf2fa-188">[Create link][createLink]</span></span>                                | `POST /drive/items/{item-id}/createLink`
| <span data-ttu-id="bf2fa-189">[人を招待][招待]</span><span class="sxs-lookup"><span data-stu-id="bf2fa-189">[Invite people][invite]</span></span>                                  | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="bf2fa-190">Update</span><span class="sxs-lookup"><span data-stu-id="bf2fa-190">Update</span></span>](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="bf2fa-191">Delete</span><span class="sxs-lookup"><span data-stu-id="bf2fa-191">Delete</span></span>](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`



[createLink]: ../api/driveitem-createlink.md
[IdentitySet]: identityset.md
[招待]: ../api/driveitem-invite.md
[invite]: ../api/driveitem-invite.md
[ItemReference]: itemreference.md
[共有 API]: ../api/shares-get.md
[shares API]: ../api/shares-get.md
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
