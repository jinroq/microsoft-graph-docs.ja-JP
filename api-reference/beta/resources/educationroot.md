---
title: educationRoot リソースの種類
description: '`/education` 名前空間は、教育機関に固有の機能を公開します。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 91f0162402b8c87042fab622710d314f27d6f4e0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507155"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="4d630-103">educationRoot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4d630-103">educationRoot resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d630-104">`/education` 名前空間は、教育機関に固有の機能を公開します。</span><span class="sxs-lookup"><span data-stu-id="4d630-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="4d630-105">`/education` 名前空間の一部のオブジェクトは、Microsoft Graph の別の部分 (たとえば、[users](user.md)) にあります。</span><span class="sxs-lookup"><span data-stu-id="4d630-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="4d630-106">教育機関の名前空間は、これらのオブジェクトに教育機関固有のプロパティと機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="4d630-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="4d630-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="4d630-107">Methods</span></span>

| <span data-ttu-id="4d630-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="4d630-108">Method</span></span>           | <span data-ttu-id="4d630-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4d630-109">Return Type</span></span>    |<span data-ttu-id="4d630-110">説明</span><span class="sxs-lookup"><span data-stu-id="4d630-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4d630-111">Create educationClass</span><span class="sxs-lookup"><span data-stu-id="4d630-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="4d630-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="4d630-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="4d630-113">クラス コレクションに投稿して、新しい **educationClass** を作成します。</span><span class="sxs-lookup"><span data-stu-id="4d630-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="4d630-114">List classes</span><span class="sxs-lookup"><span data-stu-id="4d630-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="4d630-115">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4d630-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="4d630-116">**educationClass** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="4d630-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="4d630-117">Create educationSchool</span><span class="sxs-lookup"><span data-stu-id="4d630-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="4d630-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="4d630-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="4d630-119">学校コレクションに投稿して、新しい **educationSchool** を作成します。</span><span class="sxs-lookup"><span data-stu-id="4d630-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="4d630-120">List schools</span><span class="sxs-lookup"><span data-stu-id="4d630-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="4d630-121">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4d630-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="4d630-122">**educationSchool** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="4d630-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="4d630-123">Create educationUser</span><span class="sxs-lookup"><span data-stu-id="4d630-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="4d630-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="4d630-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="4d630-125">ユーザー コレクションに投稿して、新しい **educationUser** を作成します。</span><span class="sxs-lookup"><span data-stu-id="4d630-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="4d630-126">List users</span><span class="sxs-lookup"><span data-stu-id="4d630-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="4d630-127">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4d630-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="4d630-128">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="4d630-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="4d630-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d630-129">Properties</span></span>
<span data-ttu-id="4d630-130">なし</span><span class="sxs-lookup"><span data-stu-id="4d630-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="4d630-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4d630-131">Relationships</span></span>
| <span data-ttu-id="4d630-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4d630-132">Relationship</span></span> | <span data-ttu-id="4d630-133">型</span><span class="sxs-lookup"><span data-stu-id="4d630-133">Type</span></span>   |<span data-ttu-id="4d630-134">説明</span><span class="sxs-lookup"><span data-stu-id="4d630-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d630-135">classes</span><span class="sxs-lookup"><span data-stu-id="4d630-135">classes</span></span>|<span data-ttu-id="4d630-136">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4d630-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="4d630-137">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4d630-137">Read-only.</span></span> <span data-ttu-id="4d630-138">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4d630-138">Nullable.</span></span>|
|<span data-ttu-id="4d630-139">me</span><span class="sxs-lookup"><span data-stu-id="4d630-139">me</span></span>|[<span data-ttu-id="4d630-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="4d630-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="4d630-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4d630-141">Read-only.</span></span> <span data-ttu-id="4d630-142">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4d630-142">Nullable.</span></span>|
|<span data-ttu-id="4d630-143">schools</span><span class="sxs-lookup"><span data-stu-id="4d630-143">schools</span></span>|<span data-ttu-id="4d630-144">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4d630-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="4d630-145">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4d630-145">Read-only.</span></span> <span data-ttu-id="4d630-146">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4d630-146">Nullable.</span></span>|
|<span data-ttu-id="4d630-147">users</span><span class="sxs-lookup"><span data-stu-id="4d630-147">users</span></span>|<span data-ttu-id="4d630-148">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4d630-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="4d630-p105">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4d630-p105">Read-only. Nullable.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationroot.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
