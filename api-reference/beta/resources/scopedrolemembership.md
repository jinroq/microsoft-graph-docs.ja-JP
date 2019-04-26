---
title: scopedRoleMembership リソースの種類
description: スコープ指定された役割メンバーシップは、管理単位 (AU) に対してさらにスコープを設定する、ディレクトリロールのユーザーのメンバーシップを記述します。  これにより、テナント全体の会社 adminsistrator が、組織のサブセット (AU で定義されているサブセット) 内のユーザーとグループを管理するための管理者権限を委任できるようになります。
localization_priority: Normal
ms.openlocfilehash: 56a2514fa65033154b6ab69c497c90fde201c28e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343469"
---
# <a name="scopedrolemembership-resource-type"></a><span data-ttu-id="ac37e-104">scopedRoleMembership リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ac37e-104">scopedRoleMembership resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac37e-105">スコープ指定された役割メンバーシップは、管理単位 (AU) に対してさらにスコープを設定する、ディレクトリロールのユーザーのメンバーシップを記述します。</span><span class="sxs-lookup"><span data-stu-id="ac37e-105">A scoped-role membership describes a user's membership of a directory role, that is further scoped to an Administrative Unit (AU).</span></span>  <span data-ttu-id="ac37e-106">これにより、テナント全体の会社 adminsistrator が、組織のサブセット (AU で定義されているサブセット) 内のユーザーとグループを管理するための管理者権限を委任できるようになります。</span><span class="sxs-lookup"><span data-stu-id="ac37e-106">This provides a mechanism to allow a tenant-wide company adminsistrator to delegate administrative privileges to a user to manage users and groups in a subset of the organization (the subset being defined by an AU).</span></span>

## <a name="methods"></a><span data-ttu-id="ac37e-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ac37e-107">Methods</span></span>
<span data-ttu-id="ac37e-108">このリソースへの直接クエリはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac37e-108">Direct queries to this resource are not supported.</span></span>  <span data-ttu-id="ac37e-109">スコープ指定された役割のメンバーシップのクエリを実行する方法、およびスコープ付きの役割メンバーシップを追加および削除する方法については、「操作の[単位](administrativeunit.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ac37e-109">Please see the [adminstrative units](administrativeunit.md) topic to see information on how to query for scoped-role memberships, as well as adding and removing scoped-role memberships.</span></span> 

## <a name="properties"></a><span data-ttu-id="ac37e-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac37e-110">Properties</span></span>
| <span data-ttu-id="ac37e-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac37e-111">Property</span></span>   | <span data-ttu-id="ac37e-112">型</span><span class="sxs-lookup"><span data-stu-id="ac37e-112">Type</span></span> | <span data-ttu-id="ac37e-113">説明</span><span class="sxs-lookup"><span data-stu-id="ac37e-113">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ac37e-114">administrativeUnitId</span><span class="sxs-lookup"><span data-stu-id="ac37e-114">administrativeUnitId</span></span>|<span data-ttu-id="ac37e-115">string</span><span class="sxs-lookup"><span data-stu-id="ac37e-115">string</span></span>|<span data-ttu-id="ac37e-116">ディレクトリの役割のスコープが設定されている管理単位の一意の識別子</span><span class="sxs-lookup"><span data-stu-id="ac37e-116">Unique identifier for the administrative unit that the directory role is scoped to</span></span>|
|<span data-ttu-id="ac37e-117">id</span><span class="sxs-lookup"><span data-stu-id="ac37e-117">id</span></span>|<span data-ttu-id="ac37e-118">string</span><span class="sxs-lookup"><span data-stu-id="ac37e-118">string</span></span>| <span data-ttu-id="ac37e-119">スコープ指定された役割のメンバーシップの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="ac37e-119">Unique identifier for the scoped-role membership.</span></span> <span data-ttu-id="ac37e-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ac37e-120">Read-only.</span></span>|
|<span data-ttu-id="ac37e-121">roleId</span><span class="sxs-lookup"><span data-stu-id="ac37e-121">roleId</span></span>|<span data-ttu-id="ac37e-122">string</span><span class="sxs-lookup"><span data-stu-id="ac37e-122">string</span></span>| <span data-ttu-id="ac37e-123">メンバーが属しているディレクトリロールの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="ac37e-123">Unique identifier for the directory role that the member is in.</span></span>|
|<span data-ttu-id="ac37e-124">roleMemberInfo</span><span class="sxs-lookup"><span data-stu-id="ac37e-124">roleMemberInfo</span></span>|[<span data-ttu-id="ac37e-125">identity</span><span class="sxs-lookup"><span data-stu-id="ac37e-125">identity</span></span>](identity.md)| <span data-ttu-id="ac37e-126">役割メンバーの id 情報。</span><span class="sxs-lookup"><span data-stu-id="ac37e-126">Role member identity information.</span></span> <span data-ttu-id="ac37e-127">このスコープ指定された役割のメンバーであるユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="ac37e-127">Represents the user that is a member of this scoped-role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac37e-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ac37e-128">Relationships</span></span>
<span data-ttu-id="ac37e-129">なし</span><span class="sxs-lookup"><span data-stu-id="ac37e-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ac37e-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ac37e-130">JSON representation</span></span>

<span data-ttu-id="ac37e-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ac37e-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scopedRoleMembership"
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
  "suppressions": []
}
-->
