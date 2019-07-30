---
author: JeremyKelley
ms.author: JeremyKelley
title: permission リソースの種類
description: ドライブ項目に対して付与された共有アクセス許可を表すアクセス許可リソース
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e43889f3dcab5c887cffe58cfcc4ac632389f980
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932466"
---
# <a name="permission-resource-type"></a><span data-ttu-id="708bd-103">permission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="708bd-103">permission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="708bd-104">**Permission**リソースは、[ドライブ項目](driveitem.md)リソースに対して付与された共有アクセス許可に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="708bd-104">The **permission** resource provides information about a sharing permission granted for a [driveItem](driveitem.md) resource.</span></span>

<span data-ttu-id="708bd-105">共有アクセス許可にはさまざまなフォームがあります。</span><span class="sxs-lookup"><span data-stu-id="708bd-105">Sharing permissions have a number of different forms.</span></span>
<span data-ttu-id="708bd-106">**Permission**リソースは、リソースのファセットを使用して、これらのさまざまなフォームを表します。</span><span class="sxs-lookup"><span data-stu-id="708bd-106">The **permission** resource represents these different forms through facets on the resource.</span></span>

><span data-ttu-id="708bd-107">**注:** OneDrive for Business および SharePoint のドキュメントライブラリは、 **Inheritedfrom**プロパティを返しません。</span><span class="sxs-lookup"><span data-stu-id="708bd-107">**Note:** OneDrive for Business and SharePoint document libraries do not return the **inheritedFrom** property.</span></span>

## <a name="json-representation"></a><span data-ttu-id="708bd-108">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="708bd-108">JSON representation</span></span>

<span data-ttu-id="708bd-109">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="708bd-109">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="708bd-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="708bd-110">Properties</span></span>

| <span data-ttu-id="708bd-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="708bd-111">Property</span></span>            | <span data-ttu-id="708bd-112">型</span><span class="sxs-lookup"><span data-stu-id="708bd-112">Type</span></span>                        | <span data-ttu-id="708bd-113">説明</span><span class="sxs-lookup"><span data-stu-id="708bd-113">Description</span></span>
|:--------------------|:----------------------------|:-------------------------
| <span data-ttu-id="708bd-114">id</span><span class="sxs-lookup"><span data-stu-id="708bd-114">id</span></span>                  | <span data-ttu-id="708bd-115">String</span><span class="sxs-lookup"><span data-stu-id="708bd-115">String</span></span>                      | <span data-ttu-id="708bd-p102">項目の全アクセス許可の中の、アクセス許可の一意の識別子です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="708bd-p102">The unique identifier of the permission among all permissions on the item. Read-only.</span></span>
| <span data-ttu-id="708bd-118">grantedTo</span><span class="sxs-lookup"><span data-stu-id="708bd-118">grantedTo</span></span>           | <span data-ttu-id="708bd-119">[IdentitySet][]</span><span class="sxs-lookup"><span data-stu-id="708bd-119">[IdentitySet][]</span></span>             | <span data-ttu-id="708bd-p103">ユーザー タイプのアクセス許可、ユーザーとこのアクセス許可のアプリケーションの詳細。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="708bd-p103">For user type permissions, the details of the users & applications for this permission. Read-only.</span></span>
| <span data-ttu-id="708bd-122">grantedToIdentities</span><span class="sxs-lookup"><span data-stu-id="708bd-122">grantedToIdentities</span></span> | <span data-ttu-id="708bd-123">コレクション (id[セット][])</span><span class="sxs-lookup"><span data-stu-id="708bd-123">Collection([IdentitySet][])</span></span> | <span data-ttu-id="708bd-124">リンクの種類のアクセス許可では、アクセス許可が付与されたユーザーの詳細。</span><span class="sxs-lookup"><span data-stu-id="708bd-124">For link type permissions, the details of the users to whom permission was granted.</span></span> <span data-ttu-id="708bd-125">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="708bd-125">Read-only.</span></span>
| <span data-ttu-id="708bd-126">invitation</span><span class="sxs-lookup"><span data-stu-id="708bd-126">invitation</span></span>          | <span data-ttu-id="708bd-127">[SharingInvitation][]</span><span class="sxs-lookup"><span data-stu-id="708bd-127">[SharingInvitation][]</span></span>       | <span data-ttu-id="708bd-p105">このアクセス許可に任意に関連付けられた共有招待状の詳細情報です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="708bd-p105">Details of any associated sharing invitation for this permission. Read-only.</span></span>
| <span data-ttu-id="708bd-130">inheritedFrom</span><span class="sxs-lookup"><span data-stu-id="708bd-130">inheritedFrom</span></span>       | <span data-ttu-id="708bd-131">[ItemReference][]</span><span class="sxs-lookup"><span data-stu-id="708bd-131">[ItemReference][]</span></span>           | <span data-ttu-id="708bd-p106">現在のアクセス許可が先祖から継承されている場合、その先祖への参照を提供します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="708bd-p106">Provides a reference to the ancestor of the current permission, if it is inherited from an ancestor. Read-only.</span></span>
| <span data-ttu-id="708bd-134">link</span><span class="sxs-lookup"><span data-stu-id="708bd-134">link</span></span>                | <span data-ttu-id="708bd-135">[SharingLink][]</span><span class="sxs-lookup"><span data-stu-id="708bd-135">[SharingLink][]</span></span>             | <span data-ttu-id="708bd-p107">現在のアクセス許可がリンク タイプのアクセス許可である場合は、そのリンクの詳細を提供します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="708bd-p107">Provides the link details of the current permission, if it is a link type permissions. Read-only.</span></span>
| <span data-ttu-id="708bd-138">roles</span><span class="sxs-lookup"><span data-stu-id="708bd-138">roles</span></span>               | <span data-ttu-id="708bd-139">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="708bd-139">Collection(String)</span></span>          | <span data-ttu-id="708bd-p108">`read` など、アクセス許可の種類。ロールの完全なリストは以下を参照してください。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="708bd-p108">The type of permission, e.g. `read`. See below for the full list of roles. Read-only.</span></span>
| <span data-ttu-id="708bd-143">shareId</span><span class="sxs-lookup"><span data-stu-id="708bd-143">shareId</span></span>             | <span data-ttu-id="708bd-144">String</span><span class="sxs-lookup"><span data-stu-id="708bd-144">String</span></span>                      | <span data-ttu-id="708bd-145">共有**[API][]** を介してこの共有アイテムにアクセスするために使用できる一意のトークン。</span><span class="sxs-lookup"><span data-stu-id="708bd-145">A unique token that can be used to access this shared item via the **[shares API][]**.</span></span> <span data-ttu-id="708bd-146">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="708bd-146">Read-only.</span></span>
| <span data-ttu-id="708bd-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="708bd-147">expirationDateTime</span></span>  | <span data-ttu-id="708bd-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="708bd-148">DateTimeOffset</span></span>              | <span data-ttu-id="708bd-149">Yyyy-MM-Yyyy-mm-ddthh: mm: ssZ の形式は、アクセス許可の有効期限を示します。</span><span class="sxs-lookup"><span data-stu-id="708bd-149">A format of yyyy-MM-ddTHH:mm:ssZ of DateTimeOffset indicates the expiration time of the permission.</span></span> <span data-ttu-id="708bd-150">MinValue は、このアクセス許可に有効期限が設定されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="708bd-150">DateTime.MinValue indicates there is no expiration set for this permission.</span></span> <span data-ttu-id="708bd-151">省略可能。</span><span class="sxs-lookup"><span data-stu-id="708bd-151">Optional.</span></span>
| <span data-ttu-id="708bd-152">hasPassword</span><span class="sxs-lookup"><span data-stu-id="708bd-152">hasPassword</span></span>         | <span data-ttu-id="708bd-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="708bd-153">Boolean</span></span>                     | <span data-ttu-id="708bd-154">これは、このアクセス許可に対してパスワードが設定されているかどうかを示します。これは応答でのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="708bd-154">This indicates whether password is set for this permission, it's only showing in response.</span></span> <span data-ttu-id="708bd-155">省略可能で、読み取り専用で、OneDrive 個人用のみです。</span><span class="sxs-lookup"><span data-stu-id="708bd-155">Optional and Read-only and for OneDrive Personal only.</span></span>

### <a name="roles-enumeration-values"></a><span data-ttu-id="708bd-156">Roles 列挙値</span><span class="sxs-lookup"><span data-stu-id="708bd-156">Roles enumeration values</span></span>

| <span data-ttu-id="708bd-157">値</span><span class="sxs-lookup"><span data-stu-id="708bd-157">Value</span></span>        | <span data-ttu-id="708bd-158">詳細</span><span class="sxs-lookup"><span data-stu-id="708bd-158">Details</span></span>                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | <span data-ttu-id="708bd-159">項目のメタデータと内容を読み取る機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="708bd-159">Provides the ability to read the metadata and contents of the item.</span></span>            |
| `write`     | <span data-ttu-id="708bd-160">項目のメタデータと内容の読み取りと変更の機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="708bd-160">Provides the ability to read and modify the metadata and contents of the item.</span></span> |
| `sp.owner`  | <span data-ttu-id="708bd-161">SharePoint および OneDrive for Business の場合、これは所有者ロールを表します。</span><span class="sxs-lookup"><span data-stu-id="708bd-161">For SharePoint and OneDrive for Business this represents the owner role.</span></span>       |
| `sp.member` | <span data-ttu-id="708bd-162">SharePoint および OneDrive for Business の場合、これはメンバー ロールを表します。</span><span class="sxs-lookup"><span data-stu-id="708bd-162">For SharePoint and OneDrive for Business this represents the member role.</span></span>      |

<span data-ttu-id="708bd-163">permission リソースは、_ファセット_ を使用して、リソースによって表されるアクセス許可の種類に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="708bd-163">The permission resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="708bd-164">共有リンクには、アイテムへのアクセスに必要な一意のトークンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="708bd-164">Sharing links contain a unique token required to access the item.</span></span>

<span data-ttu-id="708bd-165">[**招待**][SharingInvitation] ファセットを持つアクセス許可は、特定のユーザーやグループをファイルへのアクセスへ招待することで追加されたアクセス許可を表します。</span><span class="sxs-lookup"><span data-stu-id="708bd-165">Permissions with an [**invitation**][SharingInvitation] facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

## <a name="sharing-links"></a><span data-ttu-id="708bd-166">共有リンク</span><span class="sxs-lookup"><span data-stu-id="708bd-166">Sharing links</span></span>

<span data-ttu-id="708bd-167">[**リンク**][SharingLink] ファセットのあるアクセス許可は、項目上に作成された共有リンクを表します。</span><span class="sxs-lookup"><span data-stu-id="708bd-167">Permissions with a [**link**][SharingLink] facet represent sharing links created on the item.</span></span>
<span data-ttu-id="708bd-168">最も一般的なアクセス許可の種類を次に示します。</span><span class="sxs-lookup"><span data-stu-id="708bd-168">These are the most common kinds of permissions.</span></span>
<span data-ttu-id="708bd-169">共有リンクは、ファイルまたはフォルダーへのアクセスに使用できる一意の URL を提供します。</span><span class="sxs-lookup"><span data-stu-id="708bd-169">Sharing links provide a unique URL that can be used to access a file or folder.</span></span>
<span data-ttu-id="708bd-170">さまざまな方法でアクセスを許可するように設定できます。</span><span class="sxs-lookup"><span data-stu-id="708bd-170">They can be set up to grant access in a variety of ways.</span></span>
<span data-ttu-id="708bd-171">たとえば、 [Createlink][] API を使用して、組織にサインインしているユーザーに対して機能するリンクを作成したり、サインインを必要とせずにすべてのユーザーに対して機能するリンクを作成したりできます。</span><span class="sxs-lookup"><span data-stu-id="708bd-171">For example, you can use the [createLink][] API to create a link that works for anyone signed into your organization, or you can create a link that works for anyone, without needing to sign in.</span></span>
<span data-ttu-id="708bd-172">[Invite][] API を使用すると、社内にいるかどうかに関係なく、特定のユーザーに対してのみ機能するリンクを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="708bd-172">You can use the [invite][] API to create a link that only works for specific people, whether they're in your company or not.</span></span>

<span data-ttu-id="708bd-173">共有リンクの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="708bd-173">Here are some examples of sharing links.</span></span>

### <a name="view-link"></a><span data-ttu-id="708bd-174">表示リンク</span><span class="sxs-lookup"><span data-stu-id="708bd-174">View link</span></span>

<span data-ttu-id="708bd-175">このビューリンクは、リンクを持つすべてのユーザーに読み取り専用アクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="708bd-175">This view link provides read-only access to anyone with the link.</span></span>

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

### <a name="edit-link"></a><span data-ttu-id="708bd-176">編集リンク</span><span class="sxs-lookup"><span data-stu-id="708bd-176">Edit link</span></span>

<span data-ttu-id="708bd-177">この編集リンクは、リンクを使用して組織内のすべてのユーザーに読み取り/書き込みアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="708bd-177">This edit link provides read and write access to anyone in the organization with the link.</span></span>

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

### <a name="existing-access-link"></a><span data-ttu-id="708bd-178">既存の access リンク</span><span class="sxs-lookup"><span data-stu-id="708bd-178">Existing access link</span></span>

<span data-ttu-id="708bd-179">このリンクでは、ユーザーに対して追加の権限は付与されません。</span><span class="sxs-lookup"><span data-stu-id="708bd-179">This link does not grant any additional privileges to the user.</span></span>

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-existing-link" } -->

```json
{
  "id": "00000000-0000-0000-0000-000000000000",
  "roles": ["read"],
  "link": {
    "scope": "existingAccess",
    "type": "view",
    "webUrl": "https://contoso.sharepoint.com/:w:/t/design/Shared%20Documents/SampleDoc.docx?d=w12345",
  },
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

### <a name="specific-people-link"></a><span data-ttu-id="708bd-180">特定の人物リンク</span><span class="sxs-lookup"><span data-stu-id="708bd-180">Specific people link</span></span>

<span data-ttu-id="708bd-181">このリンクにより、 `grantedToIdentities`コレクション内の特定のユーザーに対する読み取りおよび書き込みアクセス権が提供されます。</span><span class="sxs-lookup"><span data-stu-id="708bd-181">This link provides read and write access to the specific people in the `grantedToIdentities` collection.</span></span>

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

## <a name="sharing-invitations"></a><span data-ttu-id="708bd-182">共有への招待</span><span class="sxs-lookup"><span data-stu-id="708bd-182">Sharing invitations</span></span>

<span data-ttu-id="708bd-183">[Invite][]または[grant][] API によって送信されるアクセス許可は、既知のアカウントと一致しない電子メールアドレスの[招待][sharinginvitation]ファセットに追加情報を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="708bd-183">Permissions sent by the [invite][] or [grant][] API can have additional information in the [invitation][SharingInvitation] facet for email addresses that don't match a known account.</span></span> <span data-ttu-id="708bd-184">このような場合、招待リンクが引き換えられるまで、 **grantedTo**プロパティは設定されません。これは、ユーザーが最初にリンクをクリックしてサインインしたときに発生します。</span><span class="sxs-lookup"><span data-stu-id="708bd-184">In such cases, the **grantedTo** property might not be set until the invitation link is redeemed, which occurs the first time the user clicks the link and signs in.</span></span>

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

<span data-ttu-id="708bd-185">ユーザーによって共有の招待状が引き換えられると、**grantedTo** プロパティにはアクセス許可を引き換えたアカウントに関する情報が格納されます。</span><span class="sxs-lookup"><span data-stu-id="708bd-185">After the sharing invitation has been redeemed by a user, the **grantedTo** property will contain the information about the account that redeemed the permissions:</span></span>

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

## <a name="methods"></a><span data-ttu-id="708bd-186">メソッド</span><span class="sxs-lookup"><span data-stu-id="708bd-186">Methods</span></span>

| <span data-ttu-id="708bd-187">Method</span><span class="sxs-lookup"><span data-stu-id="708bd-187">Method</span></span>                                                   | <span data-ttu-id="708bd-188">REST パス</span><span class="sxs-lookup"><span data-stu-id="708bd-188">REST Path</span></span>
|:---------------------------------------------------------|:-----------------------
| [<span data-ttu-id="708bd-189">アクセス許可を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="708bd-189">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="708bd-190">アクセス許可を取得する</span><span class="sxs-lookup"><span data-stu-id="708bd-190">Get permission</span></span>](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| <span data-ttu-id="708bd-191">[リンクの作成][Createlink]</span><span class="sxs-lookup"><span data-stu-id="708bd-191">[Create link][createLink]</span></span>                                | `POST /drive/items/{item-id}/createLink`
| <span data-ttu-id="708bd-192">[ユーザーを招待]する[invite]</span><span class="sxs-lookup"><span data-stu-id="708bd-192">[Invite people][invite]</span></span>                                  | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="708bd-193">Update</span><span class="sxs-lookup"><span data-stu-id="708bd-193">Update</span></span>](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="708bd-194">Delete</span><span class="sxs-lookup"><span data-stu-id="708bd-194">Delete</span></span>](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`



[createLink]: ../api/driveitem-createlink.md
[付与]: ../api/permission-grant.md
[grant]: ../api/permission-grant.md
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
