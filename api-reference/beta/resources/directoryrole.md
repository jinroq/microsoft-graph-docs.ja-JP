---
title: directoryRole リソース型
description: Azure AD ディレクトリ ロールを表します。 Azure AD ディレクトリ ロールは、*管理者ロール*と呼ばれることもあります。 ディレクトリ (管理者) ロールの詳細については、「Azure Active Directory での管理者ロールの割り当て」を参照してください。 Microsoft Graph では、ユーザーにディレクトリ ロールを割り当てることで、ターゲット ロールのアクセス許可をユーザーに付与できます。 ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。 既定では、会社の管理者 (Company Administrators) ディレクトリ ロールのみがアクティブ化されています。 他の利用可能なディレクトリロールをアクティブにするには、ディレクトリロールの基になる directoryroletemplate の ID を持つ POST 要求を送信します。 directoryObject から継承します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 30b22313da70c33bffc0b759f9b474f4deac2ac1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535274"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="ff57e-110">directoryRole リソース型</span><span class="sxs-lookup"><span data-stu-id="ff57e-110">directoryRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff57e-111">Azure AD ディレクトリ ロールを表します。</span><span class="sxs-lookup"><span data-stu-id="ff57e-111">Represents an Azure AD directory role.</span></span> <span data-ttu-id="ff57e-112">Azure AD ディレクトリ ロールは、*管理者ロール*と呼ばれることもあります。</span><span class="sxs-lookup"><span data-stu-id="ff57e-112">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="ff57e-113">ディレクトリ (管理者) ロールの詳細については、「[Azure Active Directory での管理者ロールの割り当て](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff57e-113">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="ff57e-114">Microsoft Graph では、ユーザーにディレクトリ ロールを割り当てることで、ターゲット ロールのアクセス許可をユーザーに付与できます。</span><span class="sxs-lookup"><span data-stu-id="ff57e-114">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="ff57e-115">ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="ff57e-115">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="ff57e-116">既定では、会社の管理者 (Company Administrators) ディレクトリ ロールのみがアクティブ化されています。</span><span class="sxs-lookup"><span data-stu-id="ff57e-116">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="ff57e-117">他の利用可能なディレクトリロールをアクティブにするには、ディレクトリロールの基になる[directoryroletemplate](directoryroletemplate.md)の ID を持つ POST 要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="ff57e-117">To activate other available directory roles, you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="ff57e-118">[directoryObject](directoryobject.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="ff57e-118">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="ff57e-119">既定では、ディレクトリの役割のスコープはテナント全体になります。</span><span class="sxs-lookup"><span data-stu-id="ff57e-119">By default, directory roles are scoped to be tenant-wide.</span></span>  <span data-ttu-id="ff57e-120">ただし、ディレクトリの役割 (現時点では、*ユーザーアカウント管理*者と*ヘルプデスク管理者*のみ) の範囲を[管理単位](administrativeunit.md)に設定することもできます。</span><span class="sxs-lookup"><span data-stu-id="ff57e-120">However, directory roles (currently only the *user account admin* and *helpdesk admin*) may also be scoped to [administrative units](administrativeunit.md).</span></span>

<span data-ttu-id="ff57e-121">このリソースは以下をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="ff57e-121">This resource supports:</span></span>

- <span data-ttu-id="ff57e-122">[デルタ](../api/directoryrole-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。</span><span class="sxs-lookup"><span data-stu-id="ff57e-122">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="ff57e-123">メソッド</span><span class="sxs-lookup"><span data-stu-id="ff57e-123">Methods</span></span>

| <span data-ttu-id="ff57e-124">メソッド</span><span class="sxs-lookup"><span data-stu-id="ff57e-124">Method</span></span>       | <span data-ttu-id="ff57e-125">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ff57e-125">Return Type</span></span>  |<span data-ttu-id="ff57e-126">説明</span><span class="sxs-lookup"><span data-stu-id="ff57e-126">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ff57e-127">Get directoryRole</span><span class="sxs-lookup"><span data-stu-id="ff57e-127">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="ff57e-128">directoryRole</span><span class="sxs-lookup"><span data-stu-id="ff57e-128">directoryRole</span></span>](directoryrole.md) |<span data-ttu-id="ff57e-129">directoryRole オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ff57e-129">Read properties and relationships of directoryRole object.</span></span>|
|[<span data-ttu-id="ff57e-130">directoryroles を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ff57e-130">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="ff57e-131">[directoryRole](directoryrole.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ff57e-131">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="ff57e-132">テナントでアクティブになっているディレクトリ ロールを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="ff57e-132">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="ff57e-133">メンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="ff57e-133">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="ff57e-134">directoryObject</span><span class="sxs-lookup"><span data-stu-id="ff57e-134">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="ff57e-135">members ナビゲーション プロパティを送信することで、ユーザーをディレクトリ ロールに追加します。</span><span class="sxs-lookup"><span data-stu-id="ff57e-135">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="ff57e-136">List members</span><span class="sxs-lookup"><span data-stu-id="ff57e-136">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="ff57e-137">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="ff57e-137">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="ff57e-138">members ナビゲーション プロパティから、ディレクトリ ロールのメンバーであるユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="ff57e-138">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="ff57e-139">Remove a member</span><span class="sxs-lookup"><span data-stu-id="ff57e-139">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="ff57e-140">directoryObject</span><span class="sxs-lookup"><span data-stu-id="ff57e-140">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="ff57e-141">ディレクトリロールからユーザーを削除します。</span><span class="sxs-lookup"><span data-stu-id="ff57e-141">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="ff57e-142">スコープが指定された役割のメンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ff57e-142">List scoped-role members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="ff57e-143">[scopedRoleMembership](scopedrolemembership.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ff57e-143">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="ff57e-144">scopedRoleMembership リソースコレクションを使用して、[管理単位](administrativeunit.md)にスコープが設定されているこのディレクトリロールのメンバーを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="ff57e-144">List the members of this directory role that are scoped to [administrative units](administrativeunit.md), through the scopedRoleMembership resource collection.</span></span>|
|[<span data-ttu-id="ff57e-145">delta</span><span class="sxs-lookup"><span data-stu-id="ff57e-145">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="ff57e-146">directoryRole コレクション</span><span class="sxs-lookup"><span data-stu-id="ff57e-146">directoryRole collection</span></span>| <span data-ttu-id="ff57e-147">ディレクトリロールの増分の変更を取得します。</span><span class="sxs-lookup"><span data-stu-id="ff57e-147">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="ff57e-148">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff57e-148">Properties</span></span>
| <span data-ttu-id="ff57e-149">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff57e-149">Property</span></span>   | <span data-ttu-id="ff57e-150">型</span><span class="sxs-lookup"><span data-stu-id="ff57e-150">Type</span></span> |<span data-ttu-id="ff57e-151">説明</span><span class="sxs-lookup"><span data-stu-id="ff57e-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff57e-152">description</span><span class="sxs-lookup"><span data-stu-id="ff57e-152">description</span></span>|<span data-ttu-id="ff57e-153">String</span><span class="sxs-lookup"><span data-stu-id="ff57e-153">String</span></span>|<span data-ttu-id="ff57e-p104">ディレクトリ ロールの説明。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="ff57e-p104">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="ff57e-156">displayName</span><span class="sxs-lookup"><span data-stu-id="ff57e-156">displayName</span></span>|<span data-ttu-id="ff57e-157">String</span><span class="sxs-lookup"><span data-stu-id="ff57e-157">String</span></span>|<span data-ttu-id="ff57e-p105">ディレクトリ ロールの表示名。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="ff57e-p105">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="ff57e-160">id</span><span class="sxs-lookup"><span data-stu-id="ff57e-160">id</span></span>|<span data-ttu-id="ff57e-161">String</span><span class="sxs-lookup"><span data-stu-id="ff57e-161">String</span></span>|<span data-ttu-id="ff57e-p106">ディレクトリ ロールの一意識別子。[directoryObject](directoryobject.md) から継承されます。キーであり、Null は許容されません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ff57e-p106">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="ff57e-165">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="ff57e-165">roleTemplateId</span></span>|<span data-ttu-id="ff57e-166">String</span><span class="sxs-lookup"><span data-stu-id="ff57e-166">String</span></span>| <span data-ttu-id="ff57e-p107">このロールが基づいている **directoryRoleTemplate** の [id](directoryroletemplate.md)。このプロパティは、POST 操作でテナント内のディレクトリ ロールをアクティブ化するときに指定する必要があります。そのディレクトリ ロールがアクティブ化されると、このプロパティは読み取り専用になります。</span><span class="sxs-lookup"><span data-stu-id="ff57e-p107">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ff57e-170">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ff57e-170">Relationships</span></span>
| <span data-ttu-id="ff57e-171">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ff57e-171">Relationship</span></span> | <span data-ttu-id="ff57e-172">型</span><span class="sxs-lookup"><span data-stu-id="ff57e-172">Type</span></span> |<span data-ttu-id="ff57e-173">説明</span><span class="sxs-lookup"><span data-stu-id="ff57e-173">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff57e-174">members</span><span class="sxs-lookup"><span data-stu-id="ff57e-174">members</span></span>|<span data-ttu-id="ff57e-175">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ff57e-175">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="ff57e-p108">このディレクトリ ロールのメンバーであるユーザー。HTTP メソッド: GET、POST、DELETE。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ff57e-p108">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|
|<span data-ttu-id="ff57e-180">scopedMembers</span><span class="sxs-lookup"><span data-stu-id="ff57e-180">scopedMembers</span></span>|<span data-ttu-id="ff57e-181">[scopedRoleMembership](scopedrolemembership.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ff57e-181">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="ff57e-182">[管理単位](administrativeunit.md)にスコープ設定されたこのディレクトリロールのメンバ。</span><span class="sxs-lookup"><span data-stu-id="ff57e-182">Members of this directory role that are scoped to [administrative units](administrativeunit.md).</span></span> <span data-ttu-id="ff57e-183">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="ff57e-183">Read-only.</span></span> <span data-ttu-id="ff57e-184">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ff57e-184">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff57e-185">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ff57e-185">JSON representation</span></span>

<span data-ttu-id="ff57e-186">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="ff57e-186">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryrole.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
