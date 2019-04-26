---
title: scopedRoleMembership リソースの種類
description: スコープ指定された役割メンバーシップは、管理単位 (AU) に対してさらにスコープを設定する、ディレクトリロールのユーザーのメンバーシップを記述します。  これにより、テナント全体の会社 adminsistrator が、組織のサブセット (AU で定義されているサブセット) 内のユーザーとグループを管理するための管理者権限を委任できるようになります。
localization_priority: Normal
ms.openlocfilehash: 2d51ad696487e7daafb9b0f4fcef0934e4f6d6e2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562980"
---
# <a name="scopedrolemembership-resource-type"></a><span data-ttu-id="cf336-104">scopedRoleMembership リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cf336-104">scopedRoleMembership resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf336-105">スコープ指定された役割メンバーシップは、管理単位 (AU) に対してさらにスコープを設定する、ディレクトリロールのユーザーのメンバーシップを記述します。</span><span class="sxs-lookup"><span data-stu-id="cf336-105">A scoped-role membership describes a user's membership of a directory role, that is further scoped to an Administrative Unit (AU).</span></span>  <span data-ttu-id="cf336-106">これにより、テナント全体の会社 adminsistrator が、組織のサブセット (AU で定義されているサブセット) 内のユーザーとグループを管理するための管理者権限を委任できるようになります。</span><span class="sxs-lookup"><span data-stu-id="cf336-106">This provides a mechanism to allow a tenant-wide company adminsistrator to delegate administrative privileges to a user to manage users and groups in a subset of the organization (the subset being defined by an AU).</span></span>

## <a name="methods"></a><span data-ttu-id="cf336-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="cf336-107">Methods</span></span>
<span data-ttu-id="cf336-108">このリソースへの直接クエリはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf336-108">Direct queries to this resource are not supported.</span></span>  <span data-ttu-id="cf336-109">スコープ指定された役割のメンバーシップのクエリを実行する方法、およびスコープ付きの役割メンバーシップを追加および削除する方法については、「操作の[単位](administrativeunit.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cf336-109">Please see the [adminstrative units](administrativeunit.md) topic to see information on how to query for scoped-role memberships, as well as adding and removing scoped-role memberships.</span></span> 

## <a name="properties"></a><span data-ttu-id="cf336-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf336-110">Properties</span></span>
| <span data-ttu-id="cf336-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf336-111">Property</span></span>   | <span data-ttu-id="cf336-112">型</span><span class="sxs-lookup"><span data-stu-id="cf336-112">Type</span></span> | <span data-ttu-id="cf336-113">説明</span><span class="sxs-lookup"><span data-stu-id="cf336-113">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="cf336-114">administrativeUnitId</span><span class="sxs-lookup"><span data-stu-id="cf336-114">administrativeUnitId</span></span>|<span data-ttu-id="cf336-115">string</span><span class="sxs-lookup"><span data-stu-id="cf336-115">string</span></span>|<span data-ttu-id="cf336-116">ディレクトリの役割のスコープが設定されている管理単位の一意の識別子</span><span class="sxs-lookup"><span data-stu-id="cf336-116">Unique identifier for the administrative unit that the directory role is scoped to</span></span>|
|<span data-ttu-id="cf336-117">id</span><span class="sxs-lookup"><span data-stu-id="cf336-117">id</span></span>|<span data-ttu-id="cf336-118">string</span><span class="sxs-lookup"><span data-stu-id="cf336-118">string</span></span>| <span data-ttu-id="cf336-119">スコープ指定された役割のメンバーシップの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="cf336-119">Unique identifier for the scoped-role membership.</span></span> <span data-ttu-id="cf336-120">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="cf336-120">Read-only.</span></span>|
|<span data-ttu-id="cf336-121">roleId</span><span class="sxs-lookup"><span data-stu-id="cf336-121">roleId</span></span>|<span data-ttu-id="cf336-122">string</span><span class="sxs-lookup"><span data-stu-id="cf336-122">string</span></span>| <span data-ttu-id="cf336-123">メンバーが属しているディレクトリロールの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="cf336-123">Unique identifier for the directory role that the member is in.</span></span>|
|<span data-ttu-id="cf336-124">roleMemberInfo</span><span class="sxs-lookup"><span data-stu-id="cf336-124">roleMemberInfo</span></span>|[<span data-ttu-id="cf336-125">identity</span><span class="sxs-lookup"><span data-stu-id="cf336-125">identity</span></span>](identity.md)| <span data-ttu-id="cf336-126">役割メンバーの id 情報。</span><span class="sxs-lookup"><span data-stu-id="cf336-126">Role member identity information.</span></span> <span data-ttu-id="cf336-127">このスコープ指定された役割のメンバーであるユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="cf336-127">Represents the user that is a member of this scoped-role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf336-128">関係</span><span class="sxs-lookup"><span data-stu-id="cf336-128">Relationships</span></span>
<span data-ttu-id="cf336-129">なし</span><span class="sxs-lookup"><span data-stu-id="cf336-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="cf336-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cf336-130">JSON representation</span></span>

<span data-ttu-id="cf336-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cf336-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scopedrolemembership"
}-->

```json
{
  "administrativeUnitId": "string",
  "id": "string (identifier)",
  "roleId": "string",
  "roleMemberInfo": {"@odata.type": "microsoft.graph.identity"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scopedRoleMembership resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/scopedrolemembership.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
