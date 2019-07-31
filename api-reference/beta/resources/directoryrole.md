---
title: directoryRole リソース型
description: Azure AD ディレクトリ ロールを表します。 Azure AD ディレクトリ ロールは、*管理者ロール*と呼ばれることもあります。 ディレクトリ (管理者) ロールの詳細については、「 Azure AD での管理者ロールの割り当て」を参照してください。 Microsoft Graph では、ユーザーにディレクトリ ロールを割り当てることで、ターゲット ロールのアクセス許可をユーザーに付与できます。 ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。 既定では、会社の管理者 (Company Administrators) ディレクトリ ロールのみがアクティブ化されています。 他の利用可能なディレクトリロールをアクティブにするには、ディレクトリロールの基になる directoryRoleTemplate の ID を持つ POST 要求を送信します。 directoryObject から継承します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fef7bdae0d10333c6a538cccb5d30d022daac901
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973825"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="9c09a-110">directoryRole リソース型</span><span class="sxs-lookup"><span data-stu-id="9c09a-110">directoryRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c09a-111">Azure AD ディレクトリ ロールを表します。</span><span class="sxs-lookup"><span data-stu-id="9c09a-111">Represents an Azure AD directory role.</span></span> <span data-ttu-id="9c09a-112">Azure AD ディレクトリ ロールは、*管理者ロール*と呼ばれることもあります。</span><span class="sxs-lookup"><span data-stu-id="9c09a-112">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="9c09a-113">ディレクトリ (管理者) ロールの詳細については、「[Azure Active Directory での管理者ロールの割り当て](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9c09a-113">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="9c09a-114">Microsoft Graph では、ユーザーにディレクトリ ロールを割り当てることで、ターゲット ロールのアクセス許可をユーザーに付与できます。</span><span class="sxs-lookup"><span data-stu-id="9c09a-114">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="9c09a-115">ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="9c09a-115">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="9c09a-116">既定では、会社の管理者 (Company Administrators) ディレクトリ ロールのみがアクティブ化されています。</span><span class="sxs-lookup"><span data-stu-id="9c09a-116">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="9c09a-117">他の利用可能なディレクトリロールをアクティブにするには、ディレクトリロールの基になる[Directoryroletemplate](directoryroletemplate.md)の ID を持つ POST 要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="9c09a-117">To activate other available directory roles, you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="9c09a-118">[directoryObject](directoryobject.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="9c09a-118">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="9c09a-119">既定では、ディレクトリの役割のスコープはテナント全体になります。</span><span class="sxs-lookup"><span data-stu-id="9c09a-119">By default, directory roles are scoped to be tenant-wide.</span></span>  <span data-ttu-id="9c09a-120">ただし、ディレクトリの役割 (現時点では、*ユーザーアカウント管理*者と*ヘルプデスク管理者*のみ) の範囲を[管理単位](administrativeunit.md)に設定することもできます。</span><span class="sxs-lookup"><span data-stu-id="9c09a-120">However, directory roles (currently only the *user account admin* and *helpdesk admin*) may also be scoped to [administrative units](administrativeunit.md).</span></span>

<span data-ttu-id="9c09a-121">このリソースは以下をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="9c09a-121">This resource supports:</span></span>

- <span data-ttu-id="9c09a-122">[デルタ](../api/directoryrole-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。</span><span class="sxs-lookup"><span data-stu-id="9c09a-122">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="9c09a-123">メソッド</span><span class="sxs-lookup"><span data-stu-id="9c09a-123">Methods</span></span>

| <span data-ttu-id="9c09a-124">メソッド</span><span class="sxs-lookup"><span data-stu-id="9c09a-124">Method</span></span>       | <span data-ttu-id="9c09a-125">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9c09a-125">Return Type</span></span>  |<span data-ttu-id="9c09a-126">説明</span><span class="sxs-lookup"><span data-stu-id="9c09a-126">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9c09a-127">Get directoryRole</span><span class="sxs-lookup"><span data-stu-id="9c09a-127">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="9c09a-128">directoryRole</span><span class="sxs-lookup"><span data-stu-id="9c09a-128">directoryRole</span></span>](directoryrole.md) |<span data-ttu-id="9c09a-129">directoryRole オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="9c09a-129">Read properties and relationships of directoryRole object.</span></span>|
|[<span data-ttu-id="9c09a-130">directoryRoles を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="9c09a-130">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="9c09a-131">[directoryRole](directoryrole.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9c09a-131">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="9c09a-132">テナントでアクティブになっているディレクトリ ロールを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="9c09a-132">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="9c09a-133">メンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="9c09a-133">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="9c09a-134">directoryObject</span><span class="sxs-lookup"><span data-stu-id="9c09a-134">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="9c09a-135">members ナビゲーション プロパティを送信することで、ユーザーをディレクトリ ロールに追加します。</span><span class="sxs-lookup"><span data-stu-id="9c09a-135">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="9c09a-136">List members</span><span class="sxs-lookup"><span data-stu-id="9c09a-136">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="9c09a-137">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9c09a-137">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="9c09a-138">members ナビゲーション プロパティから、ディレクトリ ロールのメンバーであるユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="9c09a-138">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="9c09a-139">メンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="9c09a-139">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="9c09a-140">directoryObject</span><span class="sxs-lookup"><span data-stu-id="9c09a-140">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="9c09a-141">ディレクトリ ロールからユーザーを削除します。</span><span class="sxs-lookup"><span data-stu-id="9c09a-141">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="9c09a-142">スコープが指定された役割のメンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="9c09a-142">List scoped-role members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="9c09a-143">[scopedRoleMembership](scopedrolemembership.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9c09a-143">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="9c09a-144">ScopedRoleMembership リソースコレクションを使用して、[管理単位](administrativeunit.md)にスコープが設定されているこのディレクトリロールのメンバーを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="9c09a-144">List the members of this directory role that are scoped to [administrative units](administrativeunit.md), through the scopedRoleMembership resource collection.</span></span>|
|[<span data-ttu-id="9c09a-145">デルタ</span><span class="sxs-lookup"><span data-stu-id="9c09a-145">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="9c09a-146">directoryRole コレクション</span><span class="sxs-lookup"><span data-stu-id="9c09a-146">directoryRole collection</span></span>| <span data-ttu-id="9c09a-147">ディレクトリ ルールの増分の変更を取得します。</span><span class="sxs-lookup"><span data-stu-id="9c09a-147">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="9c09a-148">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9c09a-148">Properties</span></span>
| <span data-ttu-id="9c09a-149">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9c09a-149">Property</span></span>   | <span data-ttu-id="9c09a-150">型</span><span class="sxs-lookup"><span data-stu-id="9c09a-150">Type</span></span> |<span data-ttu-id="9c09a-151">説明</span><span class="sxs-lookup"><span data-stu-id="9c09a-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c09a-152">description</span><span class="sxs-lookup"><span data-stu-id="9c09a-152">description</span></span>|<span data-ttu-id="9c09a-153">String</span><span class="sxs-lookup"><span data-stu-id="9c09a-153">String</span></span>|<span data-ttu-id="9c09a-p104">ディレクトリ ロールの説明。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="9c09a-p104">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="9c09a-156">displayName</span><span class="sxs-lookup"><span data-stu-id="9c09a-156">displayName</span></span>|<span data-ttu-id="9c09a-157">文字列</span><span class="sxs-lookup"><span data-stu-id="9c09a-157">String</span></span>|<span data-ttu-id="9c09a-p105">ディレクトリ ロールの表示名。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="9c09a-p105">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="9c09a-160">id</span><span class="sxs-lookup"><span data-stu-id="9c09a-160">id</span></span>|<span data-ttu-id="9c09a-161">文字列</span><span class="sxs-lookup"><span data-stu-id="9c09a-161">String</span></span>|<span data-ttu-id="9c09a-p106">ディレクトリ ロールの一意識別子。[directoryObject](directoryobject.md) から継承されます。キーであり、Null は許容されません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9c09a-p106">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="9c09a-165">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="9c09a-165">roleTemplateId</span></span>|<span data-ttu-id="9c09a-166">String</span><span class="sxs-lookup"><span data-stu-id="9c09a-166">String</span></span>| <span data-ttu-id="9c09a-p107">このロールが基づいている [directoryRoleTemplate](directoryroletemplate.md) の **id**。このプロパティは、POST 操作でテナント内のディレクトリ ロールをアクティブ化するときに指定する必要があります。そのディレクトリ ロールがアクティブ化されると、このプロパティは読み取り専用になります。</span><span class="sxs-lookup"><span data-stu-id="9c09a-p107">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9c09a-170">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9c09a-170">Relationships</span></span>
| <span data-ttu-id="9c09a-171">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9c09a-171">Relationship</span></span> | <span data-ttu-id="9c09a-172">型</span><span class="sxs-lookup"><span data-stu-id="9c09a-172">Type</span></span> |<span data-ttu-id="9c09a-173">説明</span><span class="sxs-lookup"><span data-stu-id="9c09a-173">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c09a-174">members</span><span class="sxs-lookup"><span data-stu-id="9c09a-174">members</span></span>|<span data-ttu-id="9c09a-175">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9c09a-175">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="9c09a-p108">このディレクトリ ロールのメンバーであるユーザー。HTTP メソッド: GET、POST、DELETE。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="9c09a-p108">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|
|<span data-ttu-id="9c09a-180">scopedMembers</span><span class="sxs-lookup"><span data-stu-id="9c09a-180">scopedMembers</span></span>|<span data-ttu-id="9c09a-181">[scopedRoleMembership](scopedrolemembership.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9c09a-181">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="9c09a-182">[管理単位](administrativeunit.md)にスコープ設定されたこのディレクトリロールのメンバ。</span><span class="sxs-lookup"><span data-stu-id="9c09a-182">Members of this directory role that are scoped to [administrative units](administrativeunit.md).</span></span> <span data-ttu-id="9c09a-183">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9c09a-183">Read-only.</span></span> <span data-ttu-id="9c09a-184">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="9c09a-184">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9c09a-185">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9c09a-185">JSON representation</span></span>

<span data-ttu-id="9c09a-186">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="9c09a-186">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
