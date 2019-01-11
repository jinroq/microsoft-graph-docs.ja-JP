---
title: educationRoot リソースの種類
description: '`/education` 名前空間は、教育機関に固有の機能を公開します。 '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: c268c7b910bd9f6f14763f3a7b5445af0ac12826
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890658"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="cbeb0-103">educationRoot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cbeb0-103">educationRoot resource type</span></span>

> <span data-ttu-id="cbeb0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cbeb0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cbeb0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cbeb0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cbeb0-106">`/education` 名前空間は、教育機関に固有の機能を公開します。</span><span class="sxs-lookup"><span data-stu-id="cbeb0-106">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="cbeb0-107">`/education` 名前空間の一部のオブジェクトは、Microsoft Graph の別の部分 (たとえば、[users](user.md)) にあります。</span><span class="sxs-lookup"><span data-stu-id="cbeb0-107">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="cbeb0-108">教育機関の名前空間は、これらのオブジェクトに教育機関固有のプロパティと機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="cbeb0-108">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="cbeb0-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="cbeb0-109">Methods</span></span>

| <span data-ttu-id="cbeb0-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="cbeb0-110">Method</span></span>           | <span data-ttu-id="cbeb0-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cbeb0-111">Return Type</span></span>    |<span data-ttu-id="cbeb0-112">説明</span><span class="sxs-lookup"><span data-stu-id="cbeb0-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cbeb0-113">Create educationClass</span><span class="sxs-lookup"><span data-stu-id="cbeb0-113">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="cbeb0-114">educationClass</span><span class="sxs-lookup"><span data-stu-id="cbeb0-114">educationClass</span></span>](educationclass.md)| <span data-ttu-id="cbeb0-115">クラス コレクションに投稿して、新しい **educationClass** を作成します。</span><span class="sxs-lookup"><span data-stu-id="cbeb0-115">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="cbeb0-116">List classes</span><span class="sxs-lookup"><span data-stu-id="cbeb0-116">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="cbeb0-117">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cbeb0-117">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="cbeb0-118">**educationClass** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="cbeb0-118">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="cbeb0-119">Create educationSchool</span><span class="sxs-lookup"><span data-stu-id="cbeb0-119">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="cbeb0-120">educationSchool</span><span class="sxs-lookup"><span data-stu-id="cbeb0-120">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="cbeb0-121">学校コレクションに投稿して、新しい **educationSchool** を作成します。</span><span class="sxs-lookup"><span data-stu-id="cbeb0-121">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="cbeb0-122">List schools</span><span class="sxs-lookup"><span data-stu-id="cbeb0-122">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="cbeb0-123">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cbeb0-123">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="cbeb0-124">**educationSchool** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="cbeb0-124">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="cbeb0-125">Create educationUser</span><span class="sxs-lookup"><span data-stu-id="cbeb0-125">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="cbeb0-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="cbeb0-126">educationUser</span></span>](educationuser.md)| <span data-ttu-id="cbeb0-127">ユーザー コレクションに投稿して、新しい **educationUser** を作成します。</span><span class="sxs-lookup"><span data-stu-id="cbeb0-127">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="cbeb0-128">List users</span><span class="sxs-lookup"><span data-stu-id="cbeb0-128">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="cbeb0-129">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cbeb0-129">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="cbeb0-130">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="cbeb0-130">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="cbeb0-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cbeb0-131">Properties</span></span>
<span data-ttu-id="cbeb0-132">なし</span><span class="sxs-lookup"><span data-stu-id="cbeb0-132">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="cbeb0-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cbeb0-133">Relationships</span></span>
| <span data-ttu-id="cbeb0-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cbeb0-134">Relationship</span></span> | <span data-ttu-id="cbeb0-135">型</span><span class="sxs-lookup"><span data-stu-id="cbeb0-135">Type</span></span>   |<span data-ttu-id="cbeb0-136">説明</span><span class="sxs-lookup"><span data-stu-id="cbeb0-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cbeb0-137">classes</span><span class="sxs-lookup"><span data-stu-id="cbeb0-137">classes</span></span>|<span data-ttu-id="cbeb0-138">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cbeb0-138">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="cbeb0-p103">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="cbeb0-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="cbeb0-141">me</span><span class="sxs-lookup"><span data-stu-id="cbeb0-141">me</span></span>|[<span data-ttu-id="cbeb0-142">educationUser</span><span class="sxs-lookup"><span data-stu-id="cbeb0-142">educationUser</span></span>](educationuser.md)| <span data-ttu-id="cbeb0-p104">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="cbeb0-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="cbeb0-145">schools</span><span class="sxs-lookup"><span data-stu-id="cbeb0-145">schools</span></span>|<span data-ttu-id="cbeb0-146">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cbeb0-146">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="cbeb0-p105">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="cbeb0-p105">Read-only. Nullable.</span></span>|
|<span data-ttu-id="cbeb0-149">users</span><span class="sxs-lookup"><span data-stu-id="cbeb0-149">users</span></span>|<span data-ttu-id="cbeb0-150">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cbeb0-150">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="cbeb0-p106">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="cbeb0-p106">Read-only. Nullable.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
