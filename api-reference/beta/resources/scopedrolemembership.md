---
title: scopedRoleMembership リソースの種類
description: スコープ ロール メンバーシップでは、スコープ管理単位 (AU) には、さらに、ディレクトリのロールのユーザーのメンバーシップについて説明します。  これは、ユーザーおよび組織の一部のグループ (、AU で定義されるサブセット) を管理するユーザーに管理者特権を委任するテナント規模の企業の adminsistrator を許可するためのメカニズムを提供します。
ms.openlocfilehash: bd635a5b1b06b98657ba24c397e2f67afb76fa8f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069796"
---
# <a name="scopedrolemembership-resource-type"></a><span data-ttu-id="66f3d-104">scopedRoleMembership リソースの種類</span><span class="sxs-lookup"><span data-stu-id="66f3d-104">scopedRoleMembership resource type</span></span>

> <span data-ttu-id="66f3d-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="66f3d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66f3d-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66f3d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="66f3d-107">スコープ ロール メンバーシップでは、スコープ管理単位 (AU) には、さらに、ディレクトリのロールのユーザーのメンバーシップについて説明します。</span><span class="sxs-lookup"><span data-stu-id="66f3d-107">A scoped-role membership describes a user's membership of a directory role, that is further scoped to an Administrative Unit (AU).</span></span>  <span data-ttu-id="66f3d-108">これは、ユーザーおよび組織の一部のグループ (、AU で定義されるサブセット) を管理するユーザーに管理者特権を委任するテナント規模の企業の adminsistrator を許可するためのメカニズムを提供します。</span><span class="sxs-lookup"><span data-stu-id="66f3d-108">This provides a mechanism to allow a tenant-wide company adminsistrator to delegate administrative privileges to a user to manage users and groups in a subset of the organization (the subset being defined by an AU).</span></span>

## <a name="methods"></a><span data-ttu-id="66f3d-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="66f3d-109">Methods</span></span>
<span data-ttu-id="66f3d-110">このリソースへの直接のクエリはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66f3d-110">Direct queries to this resource are not supported.</span></span>  <span data-ttu-id="66f3d-111">スコープ ロール メンバーシップの追加と削除と同様にスコープ ロールのメンバーシップを照会する方法についての情報を表示する[単位数の管理](administrativeunit.md)トピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="66f3d-111">Please see the [adminstrative units](administrativeunit.md) topic to see information on how to query for scoped-role memberships, as well as adding and removing scoped-role memberships.</span></span> 

## <a name="properties"></a><span data-ttu-id="66f3d-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66f3d-112">Properties</span></span>
| <span data-ttu-id="66f3d-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66f3d-113">Property</span></span>   | <span data-ttu-id="66f3d-114">型</span><span class="sxs-lookup"><span data-stu-id="66f3d-114">Type</span></span> | <span data-ttu-id="66f3d-115">説明</span><span class="sxs-lookup"><span data-stu-id="66f3d-115">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="66f3d-116">administrativeUnitId</span><span class="sxs-lookup"><span data-stu-id="66f3d-116">administrativeUnitId</span></span>|<span data-ttu-id="66f3d-117">文字列</span><span class="sxs-lookup"><span data-stu-id="66f3d-117">string</span></span>|<span data-ttu-id="66f3d-118">ディレクトリの役割のスコープは、管理単位の一意の識別子</span><span class="sxs-lookup"><span data-stu-id="66f3d-118">Unique identifier for the administrative unit that the directory role is scoped to</span></span>|
|<span data-ttu-id="66f3d-119">ID</span><span class="sxs-lookup"><span data-stu-id="66f3d-119">id</span></span>|<span data-ttu-id="66f3d-120">文字列</span><span class="sxs-lookup"><span data-stu-id="66f3d-120">string</span></span>| <span data-ttu-id="66f3d-121">スコープ ロール メンバーシップの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="66f3d-121">Unique identifier for the scoped-role membership.</span></span> <span data-ttu-id="66f3d-122">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="66f3d-122">Read-only.</span></span>|
|<span data-ttu-id="66f3d-123">roleId</span><span class="sxs-lookup"><span data-stu-id="66f3d-123">roleId</span></span>|<span data-ttu-id="66f3d-124">文字列</span><span class="sxs-lookup"><span data-stu-id="66f3d-124">string</span></span>| <span data-ttu-id="66f3d-125">メンバーが含まれるディレクトリの役割の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="66f3d-125">Unique identifier for the directory role that the member is in.</span></span>|
|<span data-ttu-id="66f3d-126">roleMemberInfo</span><span class="sxs-lookup"><span data-stu-id="66f3d-126">roleMemberInfo</span></span>|[<span data-ttu-id="66f3d-127">identity</span><span class="sxs-lookup"><span data-stu-id="66f3d-127">identity</span></span>](identity.md)| <span data-ttu-id="66f3d-128">ロール メンバーの識別情報です。</span><span class="sxs-lookup"><span data-stu-id="66f3d-128">Role member identity information.</span></span> <span data-ttu-id="66f3d-129">このスコープの役割のメンバーであるユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="66f3d-129">Represents the user that is a member of this scoped-role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66f3d-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="66f3d-130">Relationships</span></span>
<span data-ttu-id="66f3d-131">なし</span><span class="sxs-lookup"><span data-stu-id="66f3d-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="66f3d-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="66f3d-132">JSON representation</span></span>

<span data-ttu-id="66f3d-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="66f3d-133">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "scopedRoleMembership resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->