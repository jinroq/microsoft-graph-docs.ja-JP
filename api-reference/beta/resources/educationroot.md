---
title: educationRoot リソースの種類
description: '`/education` 名前空間は、教育機関に固有の機能を公開します。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 83879a2fe448e97f62dc592b42d1cbc1d3d5cf39
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334193"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="cbfc8-103">educationRoot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cbfc8-103">educationRoot resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbfc8-104">`/education` 名前空間は、教育機関に固有の機能を公開します。</span><span class="sxs-lookup"><span data-stu-id="cbfc8-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="cbfc8-105">`/education` 名前空間の一部のオブジェクトは、Microsoft Graph の別の部分 (たとえば、[users](user.md)) にあります。</span><span class="sxs-lookup"><span data-stu-id="cbfc8-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="cbfc8-106">教育機関の名前空間は、これらのオブジェクトに教育機関固有のプロパティと機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="cbfc8-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="cbfc8-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="cbfc8-107">Methods</span></span>

| <span data-ttu-id="cbfc8-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="cbfc8-108">Method</span></span>           | <span data-ttu-id="cbfc8-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cbfc8-109">Return Type</span></span>    |<span data-ttu-id="cbfc8-110">説明</span><span class="sxs-lookup"><span data-stu-id="cbfc8-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cbfc8-111">Create educationClass</span><span class="sxs-lookup"><span data-stu-id="cbfc8-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="cbfc8-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="cbfc8-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="cbfc8-113">クラス コレクションに投稿して、新しい **educationClass** を作成します。</span><span class="sxs-lookup"><span data-stu-id="cbfc8-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="cbfc8-114">List classes</span><span class="sxs-lookup"><span data-stu-id="cbfc8-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="cbfc8-115">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cbfc8-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="cbfc8-116">**educationClass** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="cbfc8-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="cbfc8-117">Create educationSchool</span><span class="sxs-lookup"><span data-stu-id="cbfc8-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="cbfc8-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="cbfc8-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="cbfc8-119">学校コレクションに投稿して、新しい **educationSchool** を作成します。</span><span class="sxs-lookup"><span data-stu-id="cbfc8-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="cbfc8-120">List schools</span><span class="sxs-lookup"><span data-stu-id="cbfc8-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="cbfc8-121">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cbfc8-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="cbfc8-122">**educationSchool** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="cbfc8-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="cbfc8-123">Create educationUser</span><span class="sxs-lookup"><span data-stu-id="cbfc8-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="cbfc8-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="cbfc8-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="cbfc8-125">ユーザー コレクションに投稿して、新しい **educationUser** を作成します。</span><span class="sxs-lookup"><span data-stu-id="cbfc8-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="cbfc8-126">List users</span><span class="sxs-lookup"><span data-stu-id="cbfc8-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="cbfc8-127">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cbfc8-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="cbfc8-128">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="cbfc8-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="cbfc8-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cbfc8-129">Properties</span></span>
<span data-ttu-id="cbfc8-130">なし</span><span class="sxs-lookup"><span data-stu-id="cbfc8-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="cbfc8-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cbfc8-131">Relationships</span></span>
| <span data-ttu-id="cbfc8-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cbfc8-132">Relationship</span></span> | <span data-ttu-id="cbfc8-133">型</span><span class="sxs-lookup"><span data-stu-id="cbfc8-133">Type</span></span>   |<span data-ttu-id="cbfc8-134">説明</span><span class="sxs-lookup"><span data-stu-id="cbfc8-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cbfc8-135">classes</span><span class="sxs-lookup"><span data-stu-id="cbfc8-135">classes</span></span>|<span data-ttu-id="cbfc8-136">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cbfc8-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="cbfc8-137">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cbfc8-137">Read-only.</span></span> <span data-ttu-id="cbfc8-138">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="cbfc8-138">Nullable.</span></span>|
|<span data-ttu-id="cbfc8-139">me</span><span class="sxs-lookup"><span data-stu-id="cbfc8-139">me</span></span>|[<span data-ttu-id="cbfc8-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="cbfc8-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="cbfc8-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cbfc8-141">Read-only.</span></span> <span data-ttu-id="cbfc8-142">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="cbfc8-142">Nullable.</span></span>|
|<span data-ttu-id="cbfc8-143">schools</span><span class="sxs-lookup"><span data-stu-id="cbfc8-143">schools</span></span>|<span data-ttu-id="cbfc8-144">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cbfc8-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="cbfc8-145">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cbfc8-145">Read-only.</span></span> <span data-ttu-id="cbfc8-146">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="cbfc8-146">Nullable.</span></span>|
|<span data-ttu-id="cbfc8-147">users</span><span class="sxs-lookup"><span data-stu-id="cbfc8-147">users</span></span>|<span data-ttu-id="cbfc8-148">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cbfc8-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="cbfc8-p105">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="cbfc8-p105">Read-only. Nullable.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
