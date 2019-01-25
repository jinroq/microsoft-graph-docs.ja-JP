---
title: educationRoot リソースの種類
description: '`/education` 名前空間は、教育機関に固有の機能を公開します。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 91f0162402b8c87042fab622710d314f27d6f4e0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523513"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="90990-103">educationRoot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="90990-103">educationRoot resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90990-104">`/education` 名前空間は、教育機関に固有の機能を公開します。</span><span class="sxs-lookup"><span data-stu-id="90990-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="90990-105">`/education` 名前空間の一部のオブジェクトは、Microsoft Graph の別の部分 (たとえば、[users](user.md)) にあります。</span><span class="sxs-lookup"><span data-stu-id="90990-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="90990-106">教育機関の名前空間は、これらのオブジェクトに教育機関固有のプロパティと機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="90990-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="90990-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="90990-107">Methods</span></span>

| <span data-ttu-id="90990-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="90990-108">Method</span></span>           | <span data-ttu-id="90990-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="90990-109">Return Type</span></span>    |<span data-ttu-id="90990-110">説明</span><span class="sxs-lookup"><span data-stu-id="90990-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="90990-111">Create educationClass</span><span class="sxs-lookup"><span data-stu-id="90990-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="90990-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="90990-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="90990-113">クラス コレクションに投稿して、新しい **educationClass** を作成します。</span><span class="sxs-lookup"><span data-stu-id="90990-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="90990-114">List classes</span><span class="sxs-lookup"><span data-stu-id="90990-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="90990-115">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="90990-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="90990-116">**educationClass** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="90990-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="90990-117">Create educationSchool</span><span class="sxs-lookup"><span data-stu-id="90990-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="90990-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="90990-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="90990-119">学校コレクションに投稿して、新しい **educationSchool** を作成します。</span><span class="sxs-lookup"><span data-stu-id="90990-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="90990-120">List schools</span><span class="sxs-lookup"><span data-stu-id="90990-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="90990-121">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="90990-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="90990-122">**educationSchool** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="90990-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="90990-123">Create educationUser</span><span class="sxs-lookup"><span data-stu-id="90990-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="90990-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="90990-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="90990-125">ユーザー コレクションに投稿して、新しい **educationUser** を作成します。</span><span class="sxs-lookup"><span data-stu-id="90990-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="90990-126">List users</span><span class="sxs-lookup"><span data-stu-id="90990-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="90990-127">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="90990-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="90990-128">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="90990-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="90990-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90990-129">Properties</span></span>
<span data-ttu-id="90990-130">なし</span><span class="sxs-lookup"><span data-stu-id="90990-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="90990-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="90990-131">Relationships</span></span>
| <span data-ttu-id="90990-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="90990-132">Relationship</span></span> | <span data-ttu-id="90990-133">型</span><span class="sxs-lookup"><span data-stu-id="90990-133">Type</span></span>   |<span data-ttu-id="90990-134">説明</span><span class="sxs-lookup"><span data-stu-id="90990-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90990-135">classes</span><span class="sxs-lookup"><span data-stu-id="90990-135">classes</span></span>|<span data-ttu-id="90990-136">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="90990-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="90990-p102">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="90990-p102">Read-only. Nullable.</span></span>|
|<span data-ttu-id="90990-139">me</span><span class="sxs-lookup"><span data-stu-id="90990-139">me</span></span>|[<span data-ttu-id="90990-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="90990-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="90990-p103">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="90990-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="90990-143">schools</span><span class="sxs-lookup"><span data-stu-id="90990-143">schools</span></span>|<span data-ttu-id="90990-144">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="90990-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="90990-p104">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="90990-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="90990-147">users</span><span class="sxs-lookup"><span data-stu-id="90990-147">users</span></span>|<span data-ttu-id="90990-148">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="90990-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="90990-p105">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="90990-p105">Read-only. Nullable.</span></span>|

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
