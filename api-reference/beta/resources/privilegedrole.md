---
title: privilegedRole リソースの種類
description: 次のように、Azure AD 管理者の役割を表します:**グローバル ・ アドミニストレーター、課金管理者、サービス管理者、ユーザー管理者、管理者のパスワード**などです。
localization_priority: Normal
ms.openlocfilehash: 75763e18731cb969623cc4df6360d50abc018b41
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860859"
---
# <a name="privilegedrole-resource-type"></a><span data-ttu-id="6d105-103">privilegedRole リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6d105-103">privilegedRole resource type</span></span>

> <span data-ttu-id="6d105-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6d105-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6d105-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6d105-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6d105-106">次のように、Azure AD 管理者の役割を表します:**グローバル ・ アドミニストレーター、課金管理者、サービス管理者、ユーザー管理者、管理者のパスワード**などです。</span><span class="sxs-lookup"><span data-stu-id="6d105-106">Represents an Azure AD administrator role, such as: **Global Administrator, Billing Administrator, Service Administrator, User Administrator, Password Administrator**, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="6d105-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="6d105-107">Methods</span></span>

| <span data-ttu-id="6d105-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="6d105-108">Method</span></span>           | <span data-ttu-id="6d105-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6d105-109">Return Type</span></span>    |<span data-ttu-id="6d105-110">説明</span><span class="sxs-lookup"><span data-stu-id="6d105-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6d105-111">PrivilegedRole オブジェクトのリスト</span><span class="sxs-lookup"><span data-stu-id="6d105-111">List privilegedRole objects</span></span>](../api/privilegedrole-list.md) | <span data-ttu-id="6d105-112">[privilegedRole](privilegedrole.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6d105-112">[privilegedRole](privilegedrole.md) collection</span></span>|<span data-ttu-id="6d105-113">PrivilegedRole のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="6d105-113">Get the collection of privilegedRole.</span></span>|
|[<span data-ttu-id="6d105-114">PrivilegedRole を取得します。</span><span class="sxs-lookup"><span data-stu-id="6d105-114">Get privilegedRole</span></span>](../api/privilegedrole-get.md) | [<span data-ttu-id="6d105-115">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="6d105-115">privilegedRole</span></span>](privilegedrole.md) |<span data-ttu-id="6d105-116">PrivilegedRole オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d105-116">Read properties and relationships of privilegedRole object.</span></span>|
|[<span data-ttu-id="6d105-117">リストの割り当て</span><span class="sxs-lookup"><span data-stu-id="6d105-117">List assignments</span></span>](../api/privilegedrole-list-assignments.md) |<span data-ttu-id="6d105-118">[privilegedRoleAssignment](privilegedroleassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6d105-118">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="6d105-119">このロールの割り当てオブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="6d105-119">Get a assignment object collection for this role.</span></span>|
|[<span data-ttu-id="6d105-120">selfActivate</span><span class="sxs-lookup"><span data-stu-id="6d105-120">selfActivate</span></span>](../api/privilegedrole-selfactivate.md)|[<span data-ttu-id="6d105-121">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6d105-121">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="6d105-122">割り当て済みのロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="6d105-122">Activate the assigned role.</span></span>|
|[<span data-ttu-id="6d105-123">selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="6d105-123">selfDeactivate</span></span>](../api/privilegedrole-selfdeactivate.md)|[<span data-ttu-id="6d105-124">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6d105-124">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="6d105-125">割り当て済みのロールを非アクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="6d105-125">Deactivate the assigned role.</span></span>|

## <a name="properties"></a><span data-ttu-id="6d105-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6d105-126">Properties</span></span>
| <span data-ttu-id="6d105-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6d105-127">Property</span></span>     | <span data-ttu-id="6d105-128">種類</span><span class="sxs-lookup"><span data-stu-id="6d105-128">Type</span></span>   |<span data-ttu-id="6d105-129">説明</span><span class="sxs-lookup"><span data-stu-id="6d105-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d105-130">ID</span><span class="sxs-lookup"><span data-stu-id="6d105-130">id</span></span>|<span data-ttu-id="6d105-131">文字列</span><span class="sxs-lookup"><span data-stu-id="6d105-131">string</span></span>|<span data-ttu-id="6d105-132">管理者の役割の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="6d105-132">The unique identifier for administrator role.</span></span> <span data-ttu-id="6d105-133">GUID の文字列し、特定の役割の Azure AD からロール テンプレートの id と同じ値を持ちます。</span><span class="sxs-lookup"><span data-stu-id="6d105-133">It is a GUID string and has the same value as the role template id from Azure AD for the given role.</span></span> <span data-ttu-id="6d105-134">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6d105-134">Read-only.</span></span>|
|<span data-ttu-id="6d105-135">name</span><span class="sxs-lookup"><span data-stu-id="6d105-135">name</span></span>|<span data-ttu-id="6d105-136">文字列</span><span class="sxs-lookup"><span data-stu-id="6d105-136">string</span></span>|<span data-ttu-id="6d105-137">ロール名です。</span><span class="sxs-lookup"><span data-stu-id="6d105-137">Role name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d105-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6d105-138">Relationships</span></span>
| <span data-ttu-id="6d105-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6d105-139">Relationship</span></span> | <span data-ttu-id="6d105-140">型</span><span class="sxs-lookup"><span data-stu-id="6d105-140">Type</span></span>   |<span data-ttu-id="6d105-141">説明</span><span class="sxs-lookup"><span data-stu-id="6d105-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d105-142">assignments</span><span class="sxs-lookup"><span data-stu-id="6d105-142">assignments</span></span>|<span data-ttu-id="6d105-143">[privilegedRoleAssignment](privilegedroleassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6d105-143">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="6d105-144">このロールの割り当て。</span><span class="sxs-lookup"><span data-stu-id="6d105-144">The assignments for this role.</span></span> <span data-ttu-id="6d105-145">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6d105-145">Read-only.</span></span> <span data-ttu-id="6d105-146">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="6d105-146">Nullable.</span></span>|
|<span data-ttu-id="6d105-147">settings</span><span class="sxs-lookup"><span data-stu-id="6d105-147">settings</span></span>|[<span data-ttu-id="6d105-148">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="6d105-148">privilegedRoleSettings</span></span>](privilegedrolesettings.md)| <span data-ttu-id="6d105-149">このロールの設定をします。</span><span class="sxs-lookup"><span data-stu-id="6d105-149">The settings for this role.</span></span> <span data-ttu-id="6d105-150">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6d105-150">Read-only.</span></span> <span data-ttu-id="6d105-151">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="6d105-151">Nullable.</span></span>|
|<span data-ttu-id="6d105-152">概要</span><span class="sxs-lookup"><span data-stu-id="6d105-152">summary</span></span>|[<span data-ttu-id="6d105-153">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="6d105-153">privilegedRoleSummary</span></span>](privilegedrolesummary.md)| <span data-ttu-id="6d105-154">この役割の概要情報です。</span><span class="sxs-lookup"><span data-stu-id="6d105-154">The summary information for this role.</span></span> <span data-ttu-id="6d105-155">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6d105-155">Read-only.</span></span> <span data-ttu-id="6d105-156">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="6d105-156">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6d105-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6d105-157">JSON representation</span></span>

<span data-ttu-id="6d105-158">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6d105-158">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRole"
}-->

```json
{
  "id": "string (identifier)",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
