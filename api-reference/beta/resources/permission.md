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
# <a name="permission-resource-type"></a><span data-ttu-id="aa0df-102">リソースのアクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aa0df-102">permission resource type</span></span>

> <span data-ttu-id="aa0df-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="aa0df-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa0df-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aa0df-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aa0df-105">**アクセス許可**リソースは、 [driveItem](driveitem.md)リソースの共有権限に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="aa0df-105">The **permission** resource provides information about a sharing permission granted for a [driveItem](driveitem.md) resource.</span></span>

<span data-ttu-id="aa0df-106">共有アクセス許可にはさまざまなフォームがあります。</span><span class="sxs-lookup"><span data-stu-id="aa0df-106">Sharing permissions have a number of different forms.</span></span>
<span data-ttu-id="aa0df-107">**アクセス許可**リソースは、リソースの面でこれらの異なる形式を表します。</span><span class="sxs-lookup"><span data-stu-id="aa0df-107">The **permission** resource represents these different forms through facets on the resource.</span></span>

><span data-ttu-id="aa0df-108">**注:** ビジネスと SharePoint のドキュメント ライブラリの OneDrive では、 **inheritedFrom**プロパティは返されません。</span><span class="sxs-lookup"><span data-stu-id="aa0df-108">**Note:** OneDrive for Business and SharePoint document libraries do not return the **inheritedFrom** property.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa0df-109">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aa0df-109">JSON representation</span></span>

<span data-ttu-id="aa0df-110">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="aa0df-110">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="aa0df-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa0df-111">Properties</span></span>

| <span data-ttu-id="aa0df-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa0df-112">Property</span></span>            | <span data-ttu-id="aa0df-113">型</span><span class="sxs-lookup"><span data-stu-id="aa0df-113">Type</span></span>                        | <span data-ttu-id="aa0df-114">説明</span><span class="sxs-lookup"><span data-stu-id="aa0df-114">Description</span></span>
|:--------------------|:----------------------------|:-------------------------
| <span data-ttu-id="aa0df-115">id</span><span class="sxs-lookup"><span data-stu-id="aa0df-115">id</span></span>                  | <span data-ttu-id="aa0df-116">String</span><span class="sxs-lookup"><span data-stu-id="aa0df-116">String</span></span>                      | <span data-ttu-id="aa0df-p103">項目の全アクセス許可の中の、アクセス許可の一意の識別子です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="aa0df-p103">The unique identifier of the permission among all permissions on the item. Read-only.</span></span>
| <span data-ttu-id="aa0df-119">grantedTo</span><span class="sxs-lookup"><span data-stu-id="aa0df-119">grantedTo</span></span>           | <span data-ttu-id="aa0df-120">[IdentitySet][]</span><span class="sxs-lookup"><span data-stu-id="aa0df-120">[IdentitySet][]</span></span>             | <span data-ttu-id="aa0df-p104">ユーザー タイプのアクセス許可、ユーザーとこのアクセス許可のアプリケーションの詳細。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="aa0df-p104">For user type permissions, the details of the users & applications for this permission. Read-only.</span></span>
| <span data-ttu-id="aa0df-123">grantedToIdentities</span><span class="sxs-lookup"><span data-stu-id="aa0df-123">grantedToIdentities</span></span> | <span data-ttu-id="aa0df-124">コレクション ([IdentitySet][])</span><span class="sxs-lookup"><span data-stu-id="aa0df-124">Collection([IdentitySet][])</span></span> | <span data-ttu-id="aa0df-125">リンクの種類のアクセス許可のアクセス許可の付与先ユーザーの詳細です。</span><span class="sxs-lookup"><span data-stu-id="aa0df-125">For link type permissions, the details of the users to whom permission was granted.</span></span> <span data-ttu-id="aa0df-126">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="aa0df-126">Read-only.</span></span>
| <span data-ttu-id="aa0df-127">invitation</span><span class="sxs-lookup"><span data-stu-id="aa0df-127">invitation</span></span>          | <span data-ttu-id="aa0df-128">[SharingInvitation][]</span><span class="sxs-lookup"><span data-stu-id="aa0df-128">[SharingInvitation][]</span></span>       | <span data-ttu-id="aa0df-p106">このアクセス許可に任意に関連付けられた共有招待状の詳細情報です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="aa0df-p106">Details of any associated sharing invitation for this permission. Read-only.</span></span>
| <span data-ttu-id="aa0df-131">inheritedFrom</span><span class="sxs-lookup"><span data-stu-id="aa0df-131">inheritedFrom</span></span>       | <span data-ttu-id="aa0df-132">[ItemReference][]</span><span class="sxs-lookup"><span data-stu-id="aa0df-132">[ItemReference][]</span></span>           | <span data-ttu-id="aa0df-p107">現在のアクセス許可が先祖から継承されている場合、その先祖への参照を提供します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="aa0df-p107">Provides a reference to the ancestor of the current permission, if it is inherited from an ancestor. Read-only.</span></span>
| <span data-ttu-id="aa0df-135">link</span><span class="sxs-lookup"><span data-stu-id="aa0df-135">link</span></span>                | <span data-ttu-id="aa0df-136">[SharingLink][]</span><span class="sxs-lookup"><span data-stu-id="aa0df-136">[SharingLink][]</span></span>             | <span data-ttu-id="aa0df-p108">現在のアクセス許可がリンク タイプのアクセス許可である場合は、そのリンクの詳細を提供します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="aa0df-p108">Provides the link details of the current permission, if it is a link type permissions. Read-only.</span></span>
| <span data-ttu-id="aa0df-139">roles</span><span class="sxs-lookup"><span data-stu-id="aa0df-139">roles</span></span>               | <span data-ttu-id="aa0df-140">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="aa0df-140">Collection(String)</span></span>          | <span data-ttu-id="aa0df-p109">`read` など、アクセス許可の種類。ロールの完全なリストは以下を参照してください。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="aa0df-p109">The type of permission, e.g. `read`. See below for the full list of roles. Read-only.</span></span>
| <span data-ttu-id="aa0df-144">shareId</span><span class="sxs-lookup"><span data-stu-id="aa0df-144">shareId</span></span>             | <span data-ttu-id="aa0df-145">String</span><span class="sxs-lookup"><span data-stu-id="aa0df-145">String</span></span>                      | <span data-ttu-id="aa0df-146">この**[API の共有][]** を使用して共有アイテムにアクセスするために使用できる一意なトークンです。</span><span class="sxs-lookup"><span data-stu-id="aa0df-146">A unique token that can be used to access this shared item via the **[shares API][]**.</span></span> <span data-ttu-id="aa0df-147">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="aa0df-147">Read-only.</span></span>
| <span data-ttu-id="aa0df-148">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="aa0df-148">expirationDateTime</span></span>  | <span data-ttu-id="aa0df-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa0df-149">DateTimeOffset</span></span>              | <span data-ttu-id="aa0df-150">Yyyy の形式で MM の DateTimeOffset の ddTHH:mm:ssZ は、アクセス許可の有効期限を示します。</span><span class="sxs-lookup"><span data-stu-id="aa0df-150">A format of yyyy-MM-ddTHH:mm:ssZ of DateTimeOffset indicates the expiration time of the permission.</span></span> <span data-ttu-id="aa0df-151">DateTime.MinValue を示しますがこのアクセス許可の有効期限が設定されていません。</span><span class="sxs-lookup"><span data-stu-id="aa0df-151">DateTime.MinValue indicates there is no expiration set for this permission.</span></span> <span data-ttu-id="aa0df-152">省略可能。</span><span class="sxs-lookup"><span data-stu-id="aa0df-152">Optional.</span></span>
| <span data-ttu-id="aa0df-153">hasPassword</span><span class="sxs-lookup"><span data-stu-id="aa0df-153">hasPassword</span></span>         | <span data-ttu-id="aa0df-154">ブール値</span><span class="sxs-lookup"><span data-stu-id="aa0df-154">Boolean</span></span>                     | <span data-ttu-id="aa0df-155">これは、応答でのみ表示されてパスワードがこのアクセス許可の設定があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="aa0df-155">This indicates whether password is set for this permission, it's only showing in response.</span></span> <span data-ttu-id="aa0df-156">オプションおよび読み取り専用であり、OneDrive 個人のみです。</span><span class="sxs-lookup"><span data-stu-id="aa0df-156">Optional and Read-only and for OneDrive Personal only.</span></span>

### <a name="roles-enumeration-values"></a><span data-ttu-id="aa0df-157">ロールの列挙値</span><span class="sxs-lookup"><span data-stu-id="aa0df-157">Roles enumeration values</span></span>

| <span data-ttu-id="aa0df-158">値</span><span class="sxs-lookup"><span data-stu-id="aa0df-158">Value</span></span>        | <span data-ttu-id="aa0df-159">詳細</span><span class="sxs-lookup"><span data-stu-id="aa0df-159">Details</span></span>                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | <span data-ttu-id="aa0df-160">項目のメタデータと内容を読み取る機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="aa0df-160">Provides the ability to read the metadata and contents of the item.</span></span>            |
| `write`     | <span data-ttu-id="aa0df-161">項目のメタデータと内容の読み取りと変更の機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="aa0df-161">Provides the ability to read and modify the metadata and contents of the item.</span></span> |
| `sp.owner`  | <span data-ttu-id="aa0df-162">SharePoint および OneDrive for Business の場合、これは所有者ロールを表します。</span><span class="sxs-lookup"><span data-stu-id="aa0df-162">For SharePoint and OneDrive for Business this represents the owner role.</span></span>       |
| `sp.member` | <span data-ttu-id="aa0df-163">SharePoint および OneDrive for Business の場合、これはメンバー ロールを表します。</span><span class="sxs-lookup"><span data-stu-id="aa0df-163">For SharePoint and OneDrive for Business this represents the member role.</span></span>      |

<span data-ttu-id="aa0df-164">permission リソースは、_ファセット_ を使用して、リソースによって表されるアクセス許可の種類に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="aa0df-164">The permission resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="aa0df-165">共有リンクには、アイテムにアクセスするために必要な一意のトークンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="aa0df-165">Sharing links contain a unique token required to access the item.</span></span>

<span data-ttu-id="aa0df-166">[**招待**][SharingInvitation] ファセットを持つアクセス許可は、特定のユーザーやグループをファイルへのアクセスへ招待することで追加されたアクセス許可を表します。</span><span class="sxs-lookup"><span data-stu-id="aa0df-166">Permissions with an [**invitation**][SharingInvitation] facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

## <a name="sharing-links"></a><span data-ttu-id="aa0df-167">共有リンク</span><span class="sxs-lookup"><span data-stu-id="aa0df-167">Sharing links</span></span>

<span data-ttu-id="aa0df-168">[**リンク**][SharingLink]のファセットは、項目を作成したリンクを共有にアクセスを許可します。</span><span class="sxs-lookup"><span data-stu-id="aa0df-168">Permissions with a [**link**][SharingLink] facet represent sharing links created on the item.</span></span>
<span data-ttu-id="aa0df-169">これらは、最も一般的な種類のアクセス許可です。</span><span class="sxs-lookup"><span data-stu-id="aa0df-169">These are the most common kinds of permissions.</span></span>
<span data-ttu-id="aa0df-170">共有リンクでは、ファイルまたはフォルダーへのアクセスに使用できる一意な URL を提供します。</span><span class="sxs-lookup"><span data-stu-id="aa0df-170">Sharing links provide a unique URL that can be used to access a file or folder.</span></span>
<span data-ttu-id="aa0df-171">それらは、さまざまな方法でアクセスを許可するを設定できます。</span><span class="sxs-lookup"><span data-stu-id="aa0df-171">They can be set up to grant access in a variety of ways.</span></span>
<span data-ttu-id="aa0df-172">[CreateLink][] API を使用するには、組織にサインインしてすべてのユーザーに対して機能するリンクを作成するなど、サインインすることがなく、すべてのユーザーに適合するリンクを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="aa0df-172">For example, you can use the [createLink][] API to create a link that works for anyone signed into your organization, or you can create a link that works for anyone, without needing to sign in.</span></span>
<span data-ttu-id="aa0df-173">[招待][]API を使用するか、会社にいるかどうかは、特定のユーザーに対してのみ機能するリンクを作成します。</span><span class="sxs-lookup"><span data-stu-id="aa0df-173">You can use the [invite][] API to create a link that only works for specific people, whether they're in your company or not.</span></span>

<span data-ttu-id="aa0df-174">リンクを共有するためのいくつかの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="aa0df-174">Here are some examples of sharing links.</span></span>

### <a name="view-link"></a><span data-ttu-id="aa0df-175">ビューのリンク</span><span class="sxs-lookup"><span data-stu-id="aa0df-175">View link</span></span>

<span data-ttu-id="aa0df-176">このビューのリンクは、リンクを使用してすべてのユーザーに読み取り専用アクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="aa0df-176">This view link provides read-only access to anyone with the link.</span></span>

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

### <a name="edit-link"></a><span data-ttu-id="aa0df-177">編集リンク</span><span class="sxs-lookup"><span data-stu-id="aa0df-177">Edit link</span></span>

<span data-ttu-id="aa0df-178">この [編集] リンクは、リンクを使用して組織内のすべてのユーザーに読み取りおよび書き込みアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="aa0df-178">This edit link provides read and write access to anyone in the organization with the link.</span></span>

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

### <a name="specific-people-link"></a><span data-ttu-id="aa0df-179">特定の人のリンク</span><span class="sxs-lookup"><span data-stu-id="aa0df-179">Specific people link</span></span>

<span data-ttu-id="aa0df-180">このリンクで特定のユーザーに読み取りおよび書き込みアクセスを提供する、`grantedToIdentities`コレクションです。</span><span class="sxs-lookup"><span data-stu-id="aa0df-180">This link provides read and write access to the specific people in the `grantedToIdentities` collection.</span></span>

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

## <a name="sharing-invitations"></a><span data-ttu-id="aa0df-181">共有への招待</span><span class="sxs-lookup"><span data-stu-id="aa0df-181">Sharing invitations</span></span>

<span data-ttu-id="aa0df-182">[招待][]API によって送信されたアクセス許可は、[招待][SharingInvitation]ファセットの追加情報があります。</span><span class="sxs-lookup"><span data-stu-id="aa0df-182">Permissions sent by the [invite][] API may have additional information in the [invitation][SharingInvitation] facet.</span></span>
<span data-ttu-id="aa0df-183">招待状は、既知のアカウントに一致しない電子メール アドレスに送信された、招待は、償還、最初にユーザーがリンクをクリックして、サインインが行われるまで、 **grantedTo**プロパティが設定できません。</span><span class="sxs-lookup"><span data-stu-id="aa0df-183">If an invitation was sent to an email address that doesn't match a known account, the **grantedTo** property may not be set until the invitation is redeemed, which occurs the first time the user clicks the link and signs in.</span></span>

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

<span data-ttu-id="aa0df-184">ユーザーによって共有の招待状が引き換えられると、**grantedTo** プロパティにはアクセス許可を引き換えたアカウントに関する情報が格納されます。</span><span class="sxs-lookup"><span data-stu-id="aa0df-184">After the sharing invitation has been redeemed by a user, the **grantedTo** property will contain the information about the account that redeemed the permissions:</span></span>

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

## <a name="methods"></a><span data-ttu-id="aa0df-185">メソッド</span><span class="sxs-lookup"><span data-stu-id="aa0df-185">Methods</span></span>

| <span data-ttu-id="aa0df-186">メソッド</span><span class="sxs-lookup"><span data-stu-id="aa0df-186">Method</span></span>                                                   | <span data-ttu-id="aa0df-187">REST パス</span><span class="sxs-lookup"><span data-stu-id="aa0df-187">REST Path</span></span>
|:---------------------------------------------------------|:-----------------------
| [<span data-ttu-id="aa0df-188">アクセス許可を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="aa0df-188">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="aa0df-189">アクセス許可を取得する</span><span class="sxs-lookup"><span data-stu-id="aa0df-189">Get permission</span></span>](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| <span data-ttu-id="aa0df-190">[[作成] リンク][createLink]</span><span class="sxs-lookup"><span data-stu-id="aa0df-190">[Create link][createLink]</span></span>                                | `POST /drive/items/{item-id}/createLink`
| <span data-ttu-id="aa0df-191">[人を招待][招待]</span><span class="sxs-lookup"><span data-stu-id="aa0df-191">[Invite people][invite]</span></span>                                  | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="aa0df-192">Update</span><span class="sxs-lookup"><span data-stu-id="aa0df-192">Update</span></span>](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="aa0df-193">削除</span><span class="sxs-lookup"><span data-stu-id="aa0df-193">Delete</span></span>](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`



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
<!-- {
  "type": "#page.annotation",
  "description": "The permission object provides information about permissions and roles and sharing information.",
  "keywords": "sharing,permissions,read,write,acl",
  "section": "documentation",
  "tocPath": "Resources/Permission"
} -->
