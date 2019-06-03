---
title: directoryRole リソース型
description: Azure AD ディレクトリ ロールを表します。 Azure AD ディレクトリ ロールは、*管理者ロール*と呼ばれることもあります。 ディレクトリ (管理者) ロールの詳細については、「 Azure AD での管理者ロールの割り当て」を参照してください。 Microsoft Graph では、ユーザーにディレクトリ ロールを割り当てることで、ターゲット ロールのアクセス許可をユーザーに付与できます。 ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。 既定では、会社の管理者 (Company Administrators) ディレクトリ ロールのみがアクティブ化されています。 その他の使用可能なディレクトリ ロールをアクティブ化するには、directoryRoleTemplate の ID を使用して POST 要求を送信します。 directoryObject から継承します。
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 89387858ac9c22fba5897460b82a2b040c40eb75
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34658016"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="27211-110">directoryRole リソース型</span><span class="sxs-lookup"><span data-stu-id="27211-110">directoryRole resource type</span></span>

<span data-ttu-id="27211-111">Azure AD ディレクトリ ロールを表します。</span><span class="sxs-lookup"><span data-stu-id="27211-111">Represents an Azure AD directory role.</span></span> <span data-ttu-id="27211-112">Azure AD ディレクトリ ロールは、*管理者ロール*と呼ばれることもあります。</span><span class="sxs-lookup"><span data-stu-id="27211-112">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="27211-113">ディレクトリ (管理者) ロールの詳細については、「[Azure Active Directory での管理者ロールの割り当て](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="27211-113">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="27211-114">Microsoft Graph では、ユーザーにディレクトリ ロールを割り当てることで、ターゲット ロールのアクセス許可をユーザーに付与できます。</span><span class="sxs-lookup"><span data-stu-id="27211-114">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="27211-115">ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="27211-115">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="27211-116">既定では、会社の管理者 (Company Administrators) ディレクトリ ロールのみがアクティブ化されています。</span><span class="sxs-lookup"><span data-stu-id="27211-116">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="27211-117">その他の使用可能なディレクトリ ロールをアクティブ化するには、[directoryRoleTemplate](directoryroletemplate.md) の ID を使用して POST 要求を送信します。この ID は、ディレクトリ ロールに基づきます。</span><span class="sxs-lookup"><span data-stu-id="27211-117">To activate other available directory roles you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="27211-118">[directoryObject](directoryobject.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="27211-118">Inherits from [directoryObject](directoryobject.md).</span></span>
<span data-ttu-id="27211-119">このリソースは以下をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="27211-119">This resource supports:</span></span>

- <span data-ttu-id="27211-120">[デルタ](../api/directoryrole-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。</span><span class="sxs-lookup"><span data-stu-id="27211-120">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="27211-121">メソッド</span><span class="sxs-lookup"><span data-stu-id="27211-121">Methods</span></span>

| <span data-ttu-id="27211-122">メソッド</span><span class="sxs-lookup"><span data-stu-id="27211-122">Method</span></span>       | <span data-ttu-id="27211-123">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="27211-123">Return Type</span></span>  |<span data-ttu-id="27211-124">説明</span><span class="sxs-lookup"><span data-stu-id="27211-124">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="27211-125">Get directoryRole</span><span class="sxs-lookup"><span data-stu-id="27211-125">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="27211-126">directoryRole</span><span class="sxs-lookup"><span data-stu-id="27211-126">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="27211-127">directoryRole オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="27211-127">Read properties and relationships of directoryRole object.</span></span> |
|[<span data-ttu-id="27211-128">directoryRoles を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="27211-128">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="27211-129">[directoryRole](directoryrole.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="27211-129">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="27211-130">テナントでアクティブになっているディレクトリ ロールを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="27211-130">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="27211-131">メンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="27211-131">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="27211-132">directoryObject</span><span class="sxs-lookup"><span data-stu-id="27211-132">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="27211-133">members ナビゲーション プロパティを送信することで、ユーザーをディレクトリ ロールに追加します。</span><span class="sxs-lookup"><span data-stu-id="27211-133">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="27211-134">List members</span><span class="sxs-lookup"><span data-stu-id="27211-134">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="27211-135">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="27211-135">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="27211-136">members ナビゲーション プロパティから、ディレクトリ ロールのメンバーであるユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="27211-136">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="27211-137">メンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="27211-137">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="27211-138">directoryObject</span><span class="sxs-lookup"><span data-stu-id="27211-138">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="27211-139">ディレクトリ ロールからユーザーを削除します。</span><span class="sxs-lookup"><span data-stu-id="27211-139">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="27211-140">Activate directoryRole</span><span class="sxs-lookup"><span data-stu-id="27211-140">Activate directoryRole</span></span>](../api/directoryrole-post-directoryroles.md) |[<span data-ttu-id="27211-141">directoryRole</span><span class="sxs-lookup"><span data-stu-id="27211-141">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="27211-142">ディレクトリ ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="27211-142">Activate a directory role.</span></span>|
|[<span data-ttu-id="27211-143">デルタ</span><span class="sxs-lookup"><span data-stu-id="27211-143">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="27211-144">directoryRole コレクション</span><span class="sxs-lookup"><span data-stu-id="27211-144">directoryRole collection</span></span>| <span data-ttu-id="27211-145">ディレクトリ ルールの増分の変更を取得します。</span><span class="sxs-lookup"><span data-stu-id="27211-145">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="27211-146">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27211-146">Properties</span></span>
| <span data-ttu-id="27211-147">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27211-147">Property</span></span>   | <span data-ttu-id="27211-148">型</span><span class="sxs-lookup"><span data-stu-id="27211-148">Type</span></span> | <span data-ttu-id="27211-149">説明</span><span class="sxs-lookup"><span data-stu-id="27211-149">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="27211-150">description</span><span class="sxs-lookup"><span data-stu-id="27211-150">description</span></span>|<span data-ttu-id="27211-151">String</span><span class="sxs-lookup"><span data-stu-id="27211-151">String</span></span>|<span data-ttu-id="27211-p103">ディレクトリ ロールの説明。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="27211-p103">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="27211-154">displayName</span><span class="sxs-lookup"><span data-stu-id="27211-154">displayName</span></span>|<span data-ttu-id="27211-155">String</span><span class="sxs-lookup"><span data-stu-id="27211-155">String</span></span>|<span data-ttu-id="27211-p104">ディレクトリ ロールの表示名。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="27211-p104">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="27211-158">id</span><span class="sxs-lookup"><span data-stu-id="27211-158">id</span></span>|<span data-ttu-id="27211-159">String</span><span class="sxs-lookup"><span data-stu-id="27211-159">String</span></span>|<span data-ttu-id="27211-p105">ディレクトリ ロールの一意識別子。[directoryObject](directoryobject.md) から継承されます。キーであり、Null は許容されません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="27211-p105">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="27211-163">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="27211-163">roleTemplateId</span></span>|<span data-ttu-id="27211-164">String</span><span class="sxs-lookup"><span data-stu-id="27211-164">String</span></span>| <span data-ttu-id="27211-p106">このロールが基づいている [directoryRoleTemplate](directoryroletemplate.md) の **id**。このプロパティは、POST 操作でテナント内のディレクトリ ロールをアクティブ化するときに指定する必要があります。そのディレクトリ ロールがアクティブ化されると、このプロパティは読み取り専用になります。</span><span class="sxs-lookup"><span data-stu-id="27211-p106">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="27211-168">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="27211-168">Relationships</span></span>
| <span data-ttu-id="27211-169">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="27211-169">Relationship</span></span> | <span data-ttu-id="27211-170">型</span><span class="sxs-lookup"><span data-stu-id="27211-170">Type</span></span> |<span data-ttu-id="27211-171">説明</span><span class="sxs-lookup"><span data-stu-id="27211-171">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27211-172">members</span><span class="sxs-lookup"><span data-stu-id="27211-172">members</span></span>|<span data-ttu-id="27211-173">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="27211-173">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="27211-p107">このディレクトリ ロールのメンバーであるユーザー。HTTP メソッド: GET、POST、DELETE。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="27211-p107">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27211-178">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="27211-178">JSON representation</span></span>

<span data-ttu-id="27211-179">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="27211-179">Here is a JSON representation of the resource</span></span>

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
