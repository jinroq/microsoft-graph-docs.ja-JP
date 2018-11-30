---
title: directoryRole リソース型
description: Azure AD ディレクトリの役割を表します。 Azure AD ディレクトリの役割は、*管理者の役割*とも呼ばれます。 ディレクトリ (管理者) の役割の詳細については、Azure AD の管理者の役割の割り当てを参照してください。 Graph とには、ターゲットのロールのアクセス許可を付与するディレクトリのロールにユーザーを割り当てることができます。 ディレクトリのロールの読み取りや、そのメンバーにする必要があります最初でアクティブにするテナントです。 会社の管理者のディレクトリの役割のみが既定でアクティブにします。 ディレクトリの役割の基になる directoryRoleTemplate の ID で POST 要求を送信するその他の利用可能なディレクトリの役割をアクティブ化します。 directoryObject から継承します。
ms.openlocfilehash: 7087befbf18a569defda697e1e2c9eb9d7d34bb9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023484"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="bbdca-110">directoryRole リソース型</span><span class="sxs-lookup"><span data-stu-id="bbdca-110">directoryRole resource type</span></span>

<span data-ttu-id="bbdca-111">Azure AD ディレクトリの役割を表します。</span><span class="sxs-lookup"><span data-stu-id="bbdca-111">Represents an Azure AD directory role.</span></span> <span data-ttu-id="bbdca-112">Azure AD ディレクトリの役割は、*管理者の役割*とも呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="bbdca-112">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="bbdca-113">ディレクトリ (管理者) の役割の詳細については、 [Azure AD の管理者ロールの割り当て](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bbdca-113">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="bbdca-114">Graph とには、ターゲットのロールのアクセス許可を付与するディレクトリのロールにユーザーを割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="bbdca-114">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="bbdca-115">ディレクトリのロールの読み取りや、そのメンバーにする必要があります最初でアクティブにするテナントです。</span><span class="sxs-lookup"><span data-stu-id="bbdca-115">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="bbdca-116">会社の管理者のディレクトリの役割のみが既定でアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="bbdca-116">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="bbdca-117">ディレクトリの役割の基になる[directoryRoleTemplate](directoryroletemplate.md)の ID で POST 要求を送信するその他の利用可能なディレクトリの役割をアクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="bbdca-117">To activate other available directory roles you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="bbdca-118">[directoryObject](directoryobject.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="bbdca-118">Inherits from [directoryObject](directoryobject.md).</span></span>
<span data-ttu-id="bbdca-119">このリソースは以下をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="bbdca-119">This resource supports:</span></span>

- <span data-ttu-id="bbdca-120">[デルタ](../api/directoryrole-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。</span><span class="sxs-lookup"><span data-stu-id="bbdca-120">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="bbdca-121">メソッド</span><span class="sxs-lookup"><span data-stu-id="bbdca-121">Methods</span></span>

| <span data-ttu-id="bbdca-122">メソッド</span><span class="sxs-lookup"><span data-stu-id="bbdca-122">Method</span></span>       | <span data-ttu-id="bbdca-123">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bbdca-123">Return Type</span></span>  |<span data-ttu-id="bbdca-124">説明</span><span class="sxs-lookup"><span data-stu-id="bbdca-124">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bbdca-125">Get directoryRole</span><span class="sxs-lookup"><span data-stu-id="bbdca-125">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="bbdca-126">directoryRole</span><span class="sxs-lookup"><span data-stu-id="bbdca-126">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="bbdca-127">directoryRole オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bbdca-127">Read properties and relationships of directoryRole object.</span></span> |
|[<span data-ttu-id="bbdca-128">directoryRoles を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="bbdca-128">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="bbdca-129">[directoryRole](directoryrole.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bbdca-129">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="bbdca-130">テナントでアクティブになっているディレクトリ ロールを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="bbdca-130">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="bbdca-131">メンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="bbdca-131">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="bbdca-132">directoryObject</span><span class="sxs-lookup"><span data-stu-id="bbdca-132">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="bbdca-133">members ナビゲーション プロパティを送信することで、ユーザーをディレクトリ ロールに追加します。</span><span class="sxs-lookup"><span data-stu-id="bbdca-133">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="bbdca-134">List members</span><span class="sxs-lookup"><span data-stu-id="bbdca-134">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="bbdca-135">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bbdca-135">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="bbdca-136">members ナビゲーション プロパティから、ディレクトリ ロールのメンバーであるユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="bbdca-136">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="bbdca-137">メンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="bbdca-137">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="bbdca-138">directoryObject</span><span class="sxs-lookup"><span data-stu-id="bbdca-138">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="bbdca-139">ディレクトリ ロールからユーザーを削除します。</span><span class="sxs-lookup"><span data-stu-id="bbdca-139">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="bbdca-140">Activate directoryRole</span><span class="sxs-lookup"><span data-stu-id="bbdca-140">Activate directoryRole</span></span>](../api/directoryrole-post-directoryroles.md) |[<span data-ttu-id="bbdca-141">directoryRole</span><span class="sxs-lookup"><span data-stu-id="bbdca-141">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="bbdca-142">ディレクトリ ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="bbdca-142">Activate a directory role.</span></span>|
|[<span data-ttu-id="bbdca-143">delta</span><span class="sxs-lookup"><span data-stu-id="bbdca-143">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="bbdca-144">directoryRole コレクション</span><span class="sxs-lookup"><span data-stu-id="bbdca-144">directoryRole collection</span></span>| <span data-ttu-id="bbdca-145">ディレクトリの役割の増分の変更を取得します。</span><span class="sxs-lookup"><span data-stu-id="bbdca-145">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="bbdca-146">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bbdca-146">Properties</span></span>
| <span data-ttu-id="bbdca-147">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bbdca-147">Property</span></span>   | <span data-ttu-id="bbdca-148">型</span><span class="sxs-lookup"><span data-stu-id="bbdca-148">Type</span></span> | <span data-ttu-id="bbdca-149">説明</span><span class="sxs-lookup"><span data-stu-id="bbdca-149">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="bbdca-150">説明</span><span class="sxs-lookup"><span data-stu-id="bbdca-150">description</span></span>|<span data-ttu-id="bbdca-151">String</span><span class="sxs-lookup"><span data-stu-id="bbdca-151">String</span></span>|<span data-ttu-id="bbdca-p103">ディレクトリ ロールの説明。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="bbdca-p103">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="bbdca-154">displayName</span><span class="sxs-lookup"><span data-stu-id="bbdca-154">displayName</span></span>|<span data-ttu-id="bbdca-155">String</span><span class="sxs-lookup"><span data-stu-id="bbdca-155">String</span></span>|<span data-ttu-id="bbdca-p104">ディレクトリ ロールの表示名。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="bbdca-p104">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="bbdca-158">id</span><span class="sxs-lookup"><span data-stu-id="bbdca-158">id</span></span>|<span data-ttu-id="bbdca-159">文字列</span><span class="sxs-lookup"><span data-stu-id="bbdca-159">String</span></span>|<span data-ttu-id="bbdca-p105">ディレクトリ ロールの一意識別子。[directoryObject](directoryobject.md) から継承されます。キーであり、Null は許容されません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bbdca-p105">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="bbdca-163">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="bbdca-163">roleTemplateId</span></span>|<span data-ttu-id="bbdca-164">String</span><span class="sxs-lookup"><span data-stu-id="bbdca-164">String</span></span>| <span data-ttu-id="bbdca-p106">このロールが基づいている [directoryRoleTemplate](directoryroletemplate.md) の **id**。このプロパティは、POST 操作でテナント内のディレクトリ ロールをアクティブ化するときに指定する必要があります。そのディレクトリ ロールがアクティブ化されると、このプロパティは読み取り専用になります。</span><span class="sxs-lookup"><span data-stu-id="bbdca-p106">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="bbdca-168">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bbdca-168">Relationships</span></span>
| <span data-ttu-id="bbdca-169">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bbdca-169">Relationship</span></span> | <span data-ttu-id="bbdca-170">型</span><span class="sxs-lookup"><span data-stu-id="bbdca-170">Type</span></span> |<span data-ttu-id="bbdca-171">説明</span><span class="sxs-lookup"><span data-stu-id="bbdca-171">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bbdca-172">members</span><span class="sxs-lookup"><span data-stu-id="bbdca-172">members</span></span>|<span data-ttu-id="bbdca-173">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bbdca-173">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="bbdca-p107">このディレクトリ ロールのメンバーであるユーザー。HTTP メソッド: GET、POST、DELETE。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="bbdca-p107">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bbdca-178">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bbdca-178">JSON representation</span></span>

<span data-ttu-id="bbdca-179">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="bbdca-179">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.directoryRole",
  "@odata.annotations": [
    {
      "capabilities": {
        "toppable": false
      }
    }
  ]
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
