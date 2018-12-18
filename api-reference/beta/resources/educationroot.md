---
title: educationRoot リソースの種類
description: '`/education` 名前空間は、教育機関に固有の機能を公開します。 '
author: mmast-msft
ms.openlocfilehash: 2a9eac02552e62e7bfb889e9e87efe47fa5f88f9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307435"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="5a033-103">educationRoot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5a033-103">educationRoot resource type</span></span>

> <span data-ttu-id="5a033-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5a033-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a033-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a033-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5a033-106">`/education` 名前空間は、教育機関に固有の機能を公開します。</span><span class="sxs-lookup"><span data-stu-id="5a033-106">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="5a033-107">`/education` 名前空間の一部のオブジェクトは、Microsoft Graph の別の部分 (たとえば、[users](user.md)) にあります。</span><span class="sxs-lookup"><span data-stu-id="5a033-107">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="5a033-108">教育機関の名前空間は、これらのオブジェクトに教育機関固有のプロパティと機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="5a033-108">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="5a033-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="5a033-109">Methods</span></span>

| <span data-ttu-id="5a033-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="5a033-110">Method</span></span>           | <span data-ttu-id="5a033-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5a033-111">Return Type</span></span>    |<span data-ttu-id="5a033-112">説明</span><span class="sxs-lookup"><span data-stu-id="5a033-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5a033-113">Create educationClass</span><span class="sxs-lookup"><span data-stu-id="5a033-113">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="5a033-114">educationClass</span><span class="sxs-lookup"><span data-stu-id="5a033-114">educationClass</span></span>](educationclass.md)| <span data-ttu-id="5a033-115">クラス コレクションに投稿して、新しい **educationClass** を作成します。</span><span class="sxs-lookup"><span data-stu-id="5a033-115">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="5a033-116">List classes</span><span class="sxs-lookup"><span data-stu-id="5a033-116">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="5a033-117">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5a033-117">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="5a033-118">**educationClass** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="5a033-118">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="5a033-119">Create educationSchool</span><span class="sxs-lookup"><span data-stu-id="5a033-119">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="5a033-120">educationSchool</span><span class="sxs-lookup"><span data-stu-id="5a033-120">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="5a033-121">学校コレクションに投稿して、新しい **educationSchool** を作成します。</span><span class="sxs-lookup"><span data-stu-id="5a033-121">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="5a033-122">List schools</span><span class="sxs-lookup"><span data-stu-id="5a033-122">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="5a033-123">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5a033-123">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="5a033-124">**educationSchool** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="5a033-124">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="5a033-125">Create educationUser</span><span class="sxs-lookup"><span data-stu-id="5a033-125">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="5a033-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="5a033-126">educationUser</span></span>](educationuser.md)| <span data-ttu-id="5a033-127">ユーザー コレクションに投稿して、新しい **educationUser** を作成します。</span><span class="sxs-lookup"><span data-stu-id="5a033-127">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="5a033-128">List users</span><span class="sxs-lookup"><span data-stu-id="5a033-128">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="5a033-129">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5a033-129">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="5a033-130">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="5a033-130">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="5a033-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a033-131">Properties</span></span>
<span data-ttu-id="5a033-132">なし</span><span class="sxs-lookup"><span data-stu-id="5a033-132">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="5a033-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5a033-133">Relationships</span></span>
| <span data-ttu-id="5a033-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5a033-134">Relationship</span></span> | <span data-ttu-id="5a033-135">型</span><span class="sxs-lookup"><span data-stu-id="5a033-135">Type</span></span>   |<span data-ttu-id="5a033-136">説明</span><span class="sxs-lookup"><span data-stu-id="5a033-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a033-137">classes</span><span class="sxs-lookup"><span data-stu-id="5a033-137">classes</span></span>|<span data-ttu-id="5a033-138">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5a033-138">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="5a033-p103">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="5a033-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="5a033-141">me</span><span class="sxs-lookup"><span data-stu-id="5a033-141">me</span></span>|[<span data-ttu-id="5a033-142">educationUser</span><span class="sxs-lookup"><span data-stu-id="5a033-142">educationUser</span></span>](educationuser.md)| <span data-ttu-id="5a033-p104">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="5a033-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="5a033-145">schools</span><span class="sxs-lookup"><span data-stu-id="5a033-145">schools</span></span>|<span data-ttu-id="5a033-146">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5a033-146">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="5a033-p105">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="5a033-p105">Read-only. Nullable.</span></span>|
|<span data-ttu-id="5a033-149">users</span><span class="sxs-lookup"><span data-stu-id="5a033-149">users</span></span>|<span data-ttu-id="5a033-150">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5a033-150">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="5a033-p106">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="5a033-p106">Read-only. Nullable.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->