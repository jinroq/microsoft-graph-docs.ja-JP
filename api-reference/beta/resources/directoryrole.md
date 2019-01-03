---
title: directoryRole リソース型
description: Azure AD ディレクトリの役割を表します。 Azure AD ディレクトリの役割は、*管理者の役割*とも呼ばれます。 ディレクトリ (管理者) の役割の詳細については、Azure AD の管理者の役割の割り当てを参照してください。 Graph とには、ターゲットのロールのアクセス許可を付与するディレクトリのロールにユーザーを割り当てることができます。 ディレクトリのロールの読み取りや、そのメンバーにする必要があります最初でアクティブにするテナントです。 会社の管理者のディレクトリの役割のみが既定でアクティブにします。 その他の利用可能なディレクトリの役割を有効にするのにはディレクトリの役割の基になる directoryRoleTemplate の ID で POST 要求を送信します。 directoryObject から継承します。
ms.openlocfilehash: c3def9f75b62db1f07c648fed18f57f92f5c7f77
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068514"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="92271-110">directoryRole リソース型</span><span class="sxs-lookup"><span data-stu-id="92271-110">directoryRole resource type</span></span>

> <span data-ttu-id="92271-111">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="92271-111">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92271-112">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92271-112">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="92271-113">Azure AD ディレクトリの役割を表します。</span><span class="sxs-lookup"><span data-stu-id="92271-113">Represents an Azure AD directory role.</span></span> <span data-ttu-id="92271-114">Azure AD ディレクトリの役割は、*管理者の役割*とも呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="92271-114">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="92271-115">ディレクトリ (管理者) の役割の詳細については、 [Azure AD の管理者ロールの割り当て](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="92271-115">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="92271-116">Graph とには、ターゲットのロールのアクセス許可を付与するディレクトリのロールにユーザーを割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="92271-116">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="92271-117">ディレクトリのロールの読み取りや、そのメンバーにする必要があります最初でアクティブにするテナントです。</span><span class="sxs-lookup"><span data-stu-id="92271-117">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="92271-118">会社の管理者のディレクトリの役割のみが既定でアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="92271-118">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="92271-119">その他の利用可能なディレクトリの役割を有効にするのにはディレクトリの役割の基になる[directoryRoleTemplate](directoryroletemplate.md)の ID で POST 要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="92271-119">To activate other available directory roles, you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="92271-120">[directoryObject](directoryobject.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="92271-120">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="92271-121">ディレクトリの役割は、既定では、テナント全体に適用されます。</span><span class="sxs-lookup"><span data-stu-id="92271-121">By default, directory roles are scoped to be tenant-wide.</span></span>  <span data-ttu-id="92271-122">ただし、ディレクトリの役割 (現在のみ*のユーザー アカウントの管理者\*\*ヘルプデスクの管理者*) は[管理単位](administrativeunit.md)にスコープも可能性があります。</span><span class="sxs-lookup"><span data-stu-id="92271-122">However, directory roles (currently only the *user account admin* and *helpdesk admin*) may also be scoped to [administrative units](administrativeunit.md).</span></span>

<span data-ttu-id="92271-123">このリソースは以下をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="92271-123">This resource supports:</span></span>

- <span data-ttu-id="92271-124">[デルタ](../api/directoryrole-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。</span><span class="sxs-lookup"><span data-stu-id="92271-124">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="92271-125">メソッド</span><span class="sxs-lookup"><span data-stu-id="92271-125">Methods</span></span>

| <span data-ttu-id="92271-126">メソッド</span><span class="sxs-lookup"><span data-stu-id="92271-126">Method</span></span>       | <span data-ttu-id="92271-127">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="92271-127">Return Type</span></span>  |<span data-ttu-id="92271-128">説明</span><span class="sxs-lookup"><span data-stu-id="92271-128">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="92271-129">Get directoryRole</span><span class="sxs-lookup"><span data-stu-id="92271-129">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="92271-130">directoryRole</span><span class="sxs-lookup"><span data-stu-id="92271-130">directoryRole</span></span>](directoryrole.md) |<span data-ttu-id="92271-131">directoryRole オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="92271-131">Read properties and relationships of directoryRole object.</span></span>|
|[<span data-ttu-id="92271-132">directoryRoles を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="92271-132">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="92271-133">[directoryRole](directoryrole.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="92271-133">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="92271-134">テナントでアクティブになっているディレクトリ ロールを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="92271-134">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="92271-135">メンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="92271-135">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="92271-136">directoryObject</span><span class="sxs-lookup"><span data-stu-id="92271-136">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="92271-137">members ナビゲーション プロパティを送信することで、ユーザーをディレクトリ ロールに追加します。</span><span class="sxs-lookup"><span data-stu-id="92271-137">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="92271-138">List members</span><span class="sxs-lookup"><span data-stu-id="92271-138">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="92271-139">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="92271-139">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="92271-140">members ナビゲーション プロパティから、ディレクトリ ロールのメンバーであるユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="92271-140">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="92271-141">メンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="92271-141">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="92271-142">directoryObject</span><span class="sxs-lookup"><span data-stu-id="92271-142">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="92271-143">ディレクトリ ロールからユーザーを削除します。</span><span class="sxs-lookup"><span data-stu-id="92271-143">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="92271-144">スコープ ロールのメンバーの一覧</span><span class="sxs-lookup"><span data-stu-id="92271-144">List scoped-role members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="92271-145">[scopedRoleMembership](scopedrolemembership.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="92271-145">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="92271-146">スコープは、[管理単位](administrativeunit.md)、scopedRoleMembership リソースのコレクションをこのディレクトリのロールのメンバーを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="92271-146">List the members of this directory role that are scoped to [administrative units](administrativeunit.md), through the scopedRoleMembership resource collection.</span></span>|
|[<span data-ttu-id="92271-147">delta</span><span class="sxs-lookup"><span data-stu-id="92271-147">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="92271-148">directoryRole コレクション</span><span class="sxs-lookup"><span data-stu-id="92271-148">directoryRole collection</span></span>| <span data-ttu-id="92271-149">ディレクトリの役割の増分の変更を取得します。</span><span class="sxs-lookup"><span data-stu-id="92271-149">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="92271-150">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92271-150">Properties</span></span>
| <span data-ttu-id="92271-151">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92271-151">Property</span></span>   | <span data-ttu-id="92271-152">型</span><span class="sxs-lookup"><span data-stu-id="92271-152">Type</span></span> |<span data-ttu-id="92271-153">説明</span><span class="sxs-lookup"><span data-stu-id="92271-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92271-154">説明</span><span class="sxs-lookup"><span data-stu-id="92271-154">description</span></span>|<span data-ttu-id="92271-155">String</span><span class="sxs-lookup"><span data-stu-id="92271-155">String</span></span>|<span data-ttu-id="92271-p105">ディレクトリ ロールの説明。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="92271-p105">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="92271-158">displayName</span><span class="sxs-lookup"><span data-stu-id="92271-158">displayName</span></span>|<span data-ttu-id="92271-159">String</span><span class="sxs-lookup"><span data-stu-id="92271-159">String</span></span>|<span data-ttu-id="92271-p106">ディレクトリ ロールの表示名。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="92271-p106">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="92271-162">id</span><span class="sxs-lookup"><span data-stu-id="92271-162">id</span></span>|<span data-ttu-id="92271-163">文字列</span><span class="sxs-lookup"><span data-stu-id="92271-163">String</span></span>|<span data-ttu-id="92271-p107">ディレクトリ ロールの一意識別子。[directoryObject](directoryobject.md) から継承されます。キーであり、Null は許容されません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="92271-p107">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="92271-167">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="92271-167">roleTemplateId</span></span>|<span data-ttu-id="92271-168">String</span><span class="sxs-lookup"><span data-stu-id="92271-168">String</span></span>| <span data-ttu-id="92271-p108">このロールが基づいている [directoryRoleTemplate](directoryroletemplate.md) の **id**。このプロパティは、POST 操作でテナント内のディレクトリ ロールをアクティブ化するときに指定する必要があります。そのディレクトリ ロールがアクティブ化されると、このプロパティは読み取り専用になります。</span><span class="sxs-lookup"><span data-stu-id="92271-p108">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="92271-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="92271-172">Relationships</span></span>
| <span data-ttu-id="92271-173">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="92271-173">Relationship</span></span> | <span data-ttu-id="92271-174">型</span><span class="sxs-lookup"><span data-stu-id="92271-174">Type</span></span> |<span data-ttu-id="92271-175">説明</span><span class="sxs-lookup"><span data-stu-id="92271-175">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92271-176">members</span><span class="sxs-lookup"><span data-stu-id="92271-176">members</span></span>|<span data-ttu-id="92271-177">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="92271-177">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="92271-p109">このディレクトリ ロールのメンバーであるユーザー。HTTP メソッド: GET、POST、DELETE。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="92271-p109">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|
|<span data-ttu-id="92271-182">scopedMembers</span><span class="sxs-lookup"><span data-stu-id="92271-182">scopedMembers</span></span>|<span data-ttu-id="92271-183">[scopedRoleMembership](scopedrolemembership.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="92271-183">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="92271-184">[管理単位](administrativeunit.md)のスコープはこのディレクトリのロールのメンバーです。</span><span class="sxs-lookup"><span data-stu-id="92271-184">Members of this directory role that are scoped to [administrative units](administrativeunit.md).</span></span> <span data-ttu-id="92271-185">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="92271-185">Read-only.</span></span> <span data-ttu-id="92271-186">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="92271-186">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="92271-187">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="92271-187">JSON representation</span></span>

<span data-ttu-id="92271-188">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="92271-188">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRole"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "roleTemplateId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->