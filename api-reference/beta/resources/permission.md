---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Permission
localization_priority: Normal
ms.openlocfilehash: e8a4adaa3c1d41270e172f9d0b0e1bf3829927c5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344973"
---
# <a name="permission-resource-type"></a><span data-ttu-id="3bd24-102">permission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3bd24-102">permission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bd24-103">**permission**リソースは、[ドライブ項目](driveitem.md)リソースに対して付与された共有アクセス許可に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="3bd24-103">The **permission** resource provides information about a sharing permission granted for a [driveItem](driveitem.md) resource.</span></span>

<span data-ttu-id="3bd24-104">共有アクセス許可にはさまざまなフォームがあります。</span><span class="sxs-lookup"><span data-stu-id="3bd24-104">Sharing permissions have a number of different forms.</span></span>
<span data-ttu-id="3bd24-105">**permission**リソースは、リソースのファセットを使用して、これらのさまざまなフォームを表します。</span><span class="sxs-lookup"><span data-stu-id="3bd24-105">The **permission** resource represents these different forms through facets on the resource.</span></span>

><span data-ttu-id="3bd24-106">**注:** OneDrive for business および SharePoint のドキュメントライブラリは、 **inheritedfrom**プロパティを返しません。</span><span class="sxs-lookup"><span data-stu-id="3bd24-106">**Note:** OneDrive for Business and SharePoint document libraries do not return the **inheritedFrom** property.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3bd24-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3bd24-107">JSON representation</span></span>

<span data-ttu-id="3bd24-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3bd24-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="3bd24-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3bd24-109">Properties</span></span>

| <span data-ttu-id="3bd24-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3bd24-110">Property</span></span>            | <span data-ttu-id="3bd24-111">型</span><span class="sxs-lookup"><span data-stu-id="3bd24-111">Type</span></span>                        | <span data-ttu-id="3bd24-112">説明</span><span class="sxs-lookup"><span data-stu-id="3bd24-112">Description</span></span>
|:--------------------|:----------------------------|:-------------------------
| <span data-ttu-id="3bd24-113">id</span><span class="sxs-lookup"><span data-stu-id="3bd24-113">id</span></span>                  | <span data-ttu-id="3bd24-114">String</span><span class="sxs-lookup"><span data-stu-id="3bd24-114">String</span></span>                      | <span data-ttu-id="3bd24-p102">項目の全アクセス許可の中の、アクセス許可の一意の識別子です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3bd24-p102">The unique identifier of the permission among all permissions on the item. Read-only.</span></span>
| <span data-ttu-id="3bd24-117">grantedTo</span><span class="sxs-lookup"><span data-stu-id="3bd24-117">grantedTo</span></span>           | <span data-ttu-id="3bd24-118">[IdentitySet][]</span><span class="sxs-lookup"><span data-stu-id="3bd24-118">[IdentitySet][]</span></span>             | <span data-ttu-id="3bd24-p103">ユーザー タイプのアクセス許可、ユーザーとこのアクセス許可のアプリケーションの詳細。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3bd24-p103">For user type permissions, the details of the users & applications for this permission. Read-only.</span></span>
| <span data-ttu-id="3bd24-121">grantedToIdentities</span><span class="sxs-lookup"><span data-stu-id="3bd24-121">grantedToIdentities</span></span> | <span data-ttu-id="3bd24-122">コレクション (id[セット][])</span><span class="sxs-lookup"><span data-stu-id="3bd24-122">Collection([IdentitySet][])</span></span> | <span data-ttu-id="3bd24-123">リンクの種類のアクセス許可では、アクセス許可が付与されたユーザーの詳細。</span><span class="sxs-lookup"><span data-stu-id="3bd24-123">For link type permissions, the details of the users to whom permission was granted.</span></span> <span data-ttu-id="3bd24-124">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3bd24-124">Read-only.</span></span>
| <span data-ttu-id="3bd24-125">invitation</span><span class="sxs-lookup"><span data-stu-id="3bd24-125">invitation</span></span>          | <span data-ttu-id="3bd24-126">[SharingInvitation][]</span><span class="sxs-lookup"><span data-stu-id="3bd24-126">[SharingInvitation][]</span></span>       | <span data-ttu-id="3bd24-p105">このアクセス許可に任意に関連付けられた共有招待状の詳細情報です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3bd24-p105">Details of any associated sharing invitation for this permission. Read-only.</span></span>
| <span data-ttu-id="3bd24-129">inheritedFrom</span><span class="sxs-lookup"><span data-stu-id="3bd24-129">inheritedFrom</span></span>       | <span data-ttu-id="3bd24-130">[ItemReference][]</span><span class="sxs-lookup"><span data-stu-id="3bd24-130">[ItemReference][]</span></span>           | <span data-ttu-id="3bd24-p106">現在のアクセス許可が先祖から継承されている場合、その先祖への参照を提供します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3bd24-p106">Provides a reference to the ancestor of the current permission, if it is inherited from an ancestor. Read-only.</span></span>
| <span data-ttu-id="3bd24-133">link</span><span class="sxs-lookup"><span data-stu-id="3bd24-133">link</span></span>                | <span data-ttu-id="3bd24-134">[SharingLink][]</span><span class="sxs-lookup"><span data-stu-id="3bd24-134">[SharingLink][]</span></span>             | <span data-ttu-id="3bd24-p107">現在のアクセス許可がリンク タイプのアクセス許可である場合は、そのリンクの詳細を提供します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3bd24-p107">Provides the link details of the current permission, if it is a link type permissions. Read-only.</span></span>
| <span data-ttu-id="3bd24-137">roles</span><span class="sxs-lookup"><span data-stu-id="3bd24-137">roles</span></span>               | <span data-ttu-id="3bd24-138">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="3bd24-138">Collection(String)</span></span>          | <span data-ttu-id="3bd24-p108">`read` など、アクセス許可の種類。ロールの完全なリストは以下を参照してください。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3bd24-p108">The type of permission, e.g. `read`. See below for the full list of roles. Read-only.</span></span>
| <span data-ttu-id="3bd24-142">shareId</span><span class="sxs-lookup"><span data-stu-id="3bd24-142">shareId</span></span>             | <span data-ttu-id="3bd24-143">String</span><span class="sxs-lookup"><span data-stu-id="3bd24-143">String</span></span>                      | <span data-ttu-id="3bd24-144">共有**[API][]** を介してこの共有アイテムにアクセスするために使用できる一意のトークン。</span><span class="sxs-lookup"><span data-stu-id="3bd24-144">A unique token that can be used to access this shared item via the **[shares API][]**.</span></span> <span data-ttu-id="3bd24-145">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3bd24-145">Read-only.</span></span>
| <span data-ttu-id="3bd24-146">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3bd24-146">expirationDateTime</span></span>  | <span data-ttu-id="3bd24-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bd24-147">DateTimeOffset</span></span>              | <span data-ttu-id="3bd24-148">yyyy-mm-yyyy-mm-ddthh: mm: ssz の形式は、アクセス許可の有効期限を示します。</span><span class="sxs-lookup"><span data-stu-id="3bd24-148">A format of yyyy-MM-ddTHH:mm:ssZ of DateTimeOffset indicates the expiration time of the permission.</span></span> <span data-ttu-id="3bd24-149">MinValue は、このアクセス許可に有効期限が設定されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="3bd24-149">DateTime.MinValue indicates there is no expiration set for this permission.</span></span> <span data-ttu-id="3bd24-150">省略可能。</span><span class="sxs-lookup"><span data-stu-id="3bd24-150">Optional.</span></span>
| <span data-ttu-id="3bd24-151">hasPassword</span><span class="sxs-lookup"><span data-stu-id="3bd24-151">hasPassword</span></span>         | <span data-ttu-id="3bd24-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bd24-152">Boolean</span></span>                     | <span data-ttu-id="3bd24-153">これは、このアクセス許可に対してパスワードが設定されているかどうかを示します。これは応答でのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="3bd24-153">This indicates whether password is set for this permission, it's only showing in response.</span></span> <span data-ttu-id="3bd24-154">省略可能で、読み取り専用で、OneDrive 個人用のみです。</span><span class="sxs-lookup"><span data-stu-id="3bd24-154">Optional and Read-only and for OneDrive Personal only.</span></span>

### <a name="roles-enumeration-values"></a><span data-ttu-id="3bd24-155">Roles 列挙値</span><span class="sxs-lookup"><span data-stu-id="3bd24-155">Roles enumeration values</span></span>

| <span data-ttu-id="3bd24-156">値</span><span class="sxs-lookup"><span data-stu-id="3bd24-156">Value</span></span>        | <span data-ttu-id="3bd24-157">詳細</span><span class="sxs-lookup"><span data-stu-id="3bd24-157">Details</span></span>                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | <span data-ttu-id="3bd24-158">項目のメタデータと内容を読み取る機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="3bd24-158">Provides the ability to read the metadata and contents of the item.</span></span>            |
| `write`     | <span data-ttu-id="3bd24-159">項目のメタデータと内容の読み取りと変更の機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="3bd24-159">Provides the ability to read and modify the metadata and contents of the item.</span></span> |
| `sp.owner`  | <span data-ttu-id="3bd24-160">SharePoint および OneDrive for Business の場合、これは所有者ロールを表します。</span><span class="sxs-lookup"><span data-stu-id="3bd24-160">For SharePoint and OneDrive for Business this represents the owner role.</span></span>       |
| `sp.member` | <span data-ttu-id="3bd24-161">SharePoint および OneDrive for Business の場合、これはメンバー ロールを表します。</span><span class="sxs-lookup"><span data-stu-id="3bd24-161">For SharePoint and OneDrive for Business this represents the member role.</span></span>      |

<span data-ttu-id="3bd24-162">permission リソースは、_ファセット_ を使用して、リソースによって表されるアクセス許可の種類に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="3bd24-162">The permission resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="3bd24-163">共有リンクには、アイテムへのアクセスに必要な一意のトークンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3bd24-163">Sharing links contain a unique token required to access the item.</span></span>

<span data-ttu-id="3bd24-164">[**招待**][SharingInvitation] ファセットを持つアクセス許可は、特定のユーザーやグループをファイルへのアクセスへ招待することで追加されたアクセス許可を表します。</span><span class="sxs-lookup"><span data-stu-id="3bd24-164">Permissions with an [**invitation**][SharingInvitation] facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

## <a name="sharing-links"></a><span data-ttu-id="3bd24-165">共有リンク</span><span class="sxs-lookup"><span data-stu-id="3bd24-165">Sharing links</span></span>

<span data-ttu-id="3bd24-166">[**リンク**][SharingLink] ファセットのあるアクセス許可は、項目上に作成された共有リンクを表します。</span><span class="sxs-lookup"><span data-stu-id="3bd24-166">Permissions with a [**link**][SharingLink] facet represent sharing links created on the item.</span></span>
<span data-ttu-id="3bd24-167">最も一般的なアクセス許可の種類を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3bd24-167">These are the most common kinds of permissions.</span></span>
<span data-ttu-id="3bd24-168">共有リンクは、ファイルまたはフォルダーへのアクセスに使用できる一意の URL を提供します。</span><span class="sxs-lookup"><span data-stu-id="3bd24-168">Sharing links provide a unique URL that can be used to access a file or folder.</span></span>
<span data-ttu-id="3bd24-169">さまざまな方法でアクセスを許可するように設定できます。</span><span class="sxs-lookup"><span data-stu-id="3bd24-169">They can be set up to grant access in a variety of ways.</span></span>
<span data-ttu-id="3bd24-170">たとえば、 [createlink][] API を使用して、組織にサインインしているユーザーに対して機能するリンクを作成したり、サインインを必要とせずにすべてのユーザーに対して機能するリンクを作成したりできます。</span><span class="sxs-lookup"><span data-stu-id="3bd24-170">For example, you can use the [createLink][] API to create a link that works for anyone signed into your organization, or you can create a link that works for anyone, without needing to sign in.</span></span>
<span data-ttu-id="3bd24-171">[invite][] API を使用すると、社内にいるかどうかに関係なく、特定のユーザーに対してのみ機能するリンクを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="3bd24-171">You can use the [invite][] API to create a link that only works for specific people, whether they're in your company or not.</span></span>

<span data-ttu-id="3bd24-172">共有リンクの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3bd24-172">Here are some examples of sharing links.</span></span>

### <a name="view-link"></a><span data-ttu-id="3bd24-173">表示リンク</span><span class="sxs-lookup"><span data-stu-id="3bd24-173">View link</span></span>

<span data-ttu-id="3bd24-174">このビューリンクは、リンクを持つすべてのユーザーに読み取り専用アクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="3bd24-174">This view link provides read-only access to anyone with the link.</span></span>

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

### <a name="edit-link"></a><span data-ttu-id="3bd24-175">編集リンク</span><span class="sxs-lookup"><span data-stu-id="3bd24-175">Edit link</span></span>

<span data-ttu-id="3bd24-176">この編集リンクは、リンクを使用して組織内のすべてのユーザーに読み取り/書き込みアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="3bd24-176">This edit link provides read and write access to anyone in the organization with the link.</span></span>

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

### <a name="specific-people-link"></a><span data-ttu-id="3bd24-177">特定の人物リンク</span><span class="sxs-lookup"><span data-stu-id="3bd24-177">Specific people link</span></span>

<span data-ttu-id="3bd24-178">このリンクにより、 `grantedToIdentities`コレクション内の特定のユーザーに対する読み取りおよび書き込みアクセス権が提供されます。</span><span class="sxs-lookup"><span data-stu-id="3bd24-178">This link provides read and write access to the specific people in the `grantedToIdentities` collection.</span></span>

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

## <a name="sharing-invitations"></a><span data-ttu-id="3bd24-179">共有への招待</span><span class="sxs-lookup"><span data-stu-id="3bd24-179">Sharing invitations</span></span>

<span data-ttu-id="3bd24-180">[invite][] API によって送信されるアクセス許可には、[招待][sharinginvitation]ファセットに追加情報が含まれている場合があります。</span><span class="sxs-lookup"><span data-stu-id="3bd24-180">Permissions sent by the [invite][] API may have additional information in the [invitation][SharingInvitation] facet.</span></span>
<span data-ttu-id="3bd24-181">招待状が既知のアカウントに一致しない電子メールアドレスに送信された場合、招待が引き換えられるまで、 **grantedTo**プロパティは設定されません。これは、ユーザーが最初にリンクをクリックしてサインインするときに発生します。</span><span class="sxs-lookup"><span data-stu-id="3bd24-181">If an invitation was sent to an email address that doesn't match a known account, the **grantedTo** property may not be set until the invitation is redeemed, which occurs the first time the user clicks the link and signs in.</span></span>

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

<span data-ttu-id="3bd24-182">ユーザーによって共有の招待状が引き換えられると、**grantedTo** プロパティにはアクセス許可を引き換えたアカウントに関する情報が格納されます。</span><span class="sxs-lookup"><span data-stu-id="3bd24-182">After the sharing invitation has been redeemed by a user, the **grantedTo** property will contain the information about the account that redeemed the permissions:</span></span>

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

## <a name="methods"></a><span data-ttu-id="3bd24-183">メソッド</span><span class="sxs-lookup"><span data-stu-id="3bd24-183">Methods</span></span>

| <span data-ttu-id="3bd24-184">Method</span><span class="sxs-lookup"><span data-stu-id="3bd24-184">Method</span></span>                                                   | <span data-ttu-id="3bd24-185">REST パス</span><span class="sxs-lookup"><span data-stu-id="3bd24-185">REST Path</span></span>
|:---------------------------------------------------------|:-----------------------
| [<span data-ttu-id="3bd24-186">アクセス許可を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="3bd24-186">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="3bd24-187">アクセス許可を取得する</span><span class="sxs-lookup"><span data-stu-id="3bd24-187">Get permission</span></span>](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| <span data-ttu-id="3bd24-188">[リンクの作成][createlink]</span><span class="sxs-lookup"><span data-stu-id="3bd24-188">[Create link][createLink]</span></span>                                | `POST /drive/items/{item-id}/createLink`
| <span data-ttu-id="3bd24-189">[ユーザーを招待]する[invite]</span><span class="sxs-lookup"><span data-stu-id="3bd24-189">[Invite people][invite]</span></span>                                  | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="3bd24-190">更新する</span><span class="sxs-lookup"><span data-stu-id="3bd24-190">Update</span></span>](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="3bd24-191">削除</span><span class="sxs-lookup"><span data-stu-id="3bd24-191">Delete</span></span>](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`



[createLink]: ../api/driveitem-createlink.md
[IdentitySet]: identityset.md
[全員]: ../api/driveitem-invite.md
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
  "suppressions": []
}
-->
