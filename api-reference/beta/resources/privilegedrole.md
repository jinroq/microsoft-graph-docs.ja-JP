---
title: privilegedRole リソースの種類
description: Azure AD 管理者の役割 (**全体管理者、課金管理者、サービス管理者、ユーザー管理者、パスワード管理者**など) を表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 98e5cd2c53b398339e8db65bec520a16f72d8f39
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965748"
---
# <a name="privilegedrole-resource-type"></a><span data-ttu-id="1e760-103">privilegedRole リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1e760-103">privilegedRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e760-104">Azure AD 管理者の役割 (**全体管理者、課金管理者、サービス管理者、ユーザー管理者、パスワード管理者**など) を表します。</span><span class="sxs-lookup"><span data-stu-id="1e760-104">Represents an Azure AD administrator role, such as: **Global Administrator, Billing Administrator, Service Administrator, User Administrator, Password Administrator**, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="1e760-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="1e760-105">Methods</span></span>

| <span data-ttu-id="1e760-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="1e760-106">Method</span></span>           | <span data-ttu-id="1e760-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1e760-107">Return Type</span></span>    |<span data-ttu-id="1e760-108">説明</span><span class="sxs-lookup"><span data-stu-id="1e760-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1e760-109">PrivilegedRole オブジェクトを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1e760-109">List privilegedRole objects</span></span>](../api/privilegedrole-list.md) | <span data-ttu-id="1e760-110">[privilegedRole](privilegedrole.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1e760-110">[privilegedRole](privilegedrole.md) collection</span></span>|<span data-ttu-id="1e760-111">PrivilegedRole のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="1e760-111">Get the collection of privilegedRole.</span></span>|
|[<span data-ttu-id="1e760-112">privilegedRole を取得する</span><span class="sxs-lookup"><span data-stu-id="1e760-112">Get privilegedRole</span></span>](../api/privilegedrole-get.md) | [<span data-ttu-id="1e760-113">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="1e760-113">privilegedRole</span></span>](privilegedrole.md) |<span data-ttu-id="1e760-114">PrivilegedRole オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1e760-114">Read properties and relationships of privilegedRole object.</span></span>|
|[<span data-ttu-id="1e760-115">割り当てを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1e760-115">List assignments</span></span>](../api/privilegedrole-list-assignments.md) |<span data-ttu-id="1e760-116">[privilegedRoleAssignment](privilegedroleassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1e760-116">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="1e760-117">このロールの割り当てオブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="1e760-117">Get a assignment object collection for this role.</span></span>|
|[<span data-ttu-id="1e760-118">selfActivate</span><span class="sxs-lookup"><span data-stu-id="1e760-118">selfActivate</span></span>](../api/privilegedrole-selfactivate.md)|[<span data-ttu-id="1e760-119">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="1e760-119">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="1e760-120">割り当てられた役割をアクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="1e760-120">Activate the assigned role.</span></span>|
|[<span data-ttu-id="1e760-121">selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="1e760-121">selfDeactivate</span></span>](../api/privilegedrole-selfdeactivate.md)|[<span data-ttu-id="1e760-122">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="1e760-122">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="1e760-123">割り当てられた役割を非アクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="1e760-123">Deactivate the assigned role.</span></span>|

## <a name="properties"></a><span data-ttu-id="1e760-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e760-124">Properties</span></span>
| <span data-ttu-id="1e760-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e760-125">Property</span></span>     | <span data-ttu-id="1e760-126">型</span><span class="sxs-lookup"><span data-stu-id="1e760-126">Type</span></span>   |<span data-ttu-id="1e760-127">説明</span><span class="sxs-lookup"><span data-stu-id="1e760-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e760-128">id</span><span class="sxs-lookup"><span data-stu-id="1e760-128">id</span></span>|<span data-ttu-id="1e760-129">string</span><span class="sxs-lookup"><span data-stu-id="1e760-129">string</span></span>|<span data-ttu-id="1e760-130">管理者の役割の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="1e760-130">The unique identifier for administrator role.</span></span> <span data-ttu-id="1e760-131">これは GUID 文字列であり、指定された役割に対して Azure AD からのロールテンプレート id と同じ値を持ちます。</span><span class="sxs-lookup"><span data-stu-id="1e760-131">It is a GUID string and has the same value as the role template id from Azure AD for the given role.</span></span> <span data-ttu-id="1e760-132">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="1e760-132">Read-only.</span></span>|
|<span data-ttu-id="1e760-133">name</span><span class="sxs-lookup"><span data-stu-id="1e760-133">name</span></span>|<span data-ttu-id="1e760-134">string</span><span class="sxs-lookup"><span data-stu-id="1e760-134">string</span></span>|<span data-ttu-id="1e760-135">役割名。</span><span class="sxs-lookup"><span data-stu-id="1e760-135">Role name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e760-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1e760-136">Relationships</span></span>
| <span data-ttu-id="1e760-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1e760-137">Relationship</span></span> | <span data-ttu-id="1e760-138">型</span><span class="sxs-lookup"><span data-stu-id="1e760-138">Type</span></span>   |<span data-ttu-id="1e760-139">説明</span><span class="sxs-lookup"><span data-stu-id="1e760-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e760-140">assignments</span><span class="sxs-lookup"><span data-stu-id="1e760-140">assignments</span></span>|<span data-ttu-id="1e760-141">[privilegedRoleAssignment](privilegedroleassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1e760-141">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="1e760-142">この役割の割り当て。</span><span class="sxs-lookup"><span data-stu-id="1e760-142">The assignments for this role.</span></span> <span data-ttu-id="1e760-143">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1e760-143">Read-only.</span></span> <span data-ttu-id="1e760-144">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="1e760-144">Nullable.</span></span>|
|<span data-ttu-id="1e760-145">settings</span><span class="sxs-lookup"><span data-stu-id="1e760-145">settings</span></span>|[<span data-ttu-id="1e760-146">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="1e760-146">privilegedRoleSettings</span></span>](privilegedrolesettings.md)| <span data-ttu-id="1e760-147">この役割の設定。</span><span class="sxs-lookup"><span data-stu-id="1e760-147">The settings for this role.</span></span> <span data-ttu-id="1e760-148">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1e760-148">Read-only.</span></span> <span data-ttu-id="1e760-149">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="1e760-149">Nullable.</span></span>|
|<span data-ttu-id="1e760-150">summary</span><span class="sxs-lookup"><span data-stu-id="1e760-150">summary</span></span>|[<span data-ttu-id="1e760-151">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="1e760-151">privilegedRoleSummary</span></span>](privilegedrolesummary.md)| <span data-ttu-id="1e760-152">このロールの概要情報。</span><span class="sxs-lookup"><span data-stu-id="1e760-152">The summary information for this role.</span></span> <span data-ttu-id="1e760-153">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1e760-153">Read-only.</span></span> <span data-ttu-id="1e760-154">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="1e760-154">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1e760-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1e760-155">JSON representation</span></span>

<span data-ttu-id="1e760-156">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1e760-156">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
