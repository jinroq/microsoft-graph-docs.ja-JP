---
title: educationRoot リソースの種類
description: '`/education` 名前空間は、教育機関に固有の機能を公開します。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 69835ca7e3c7a45864382eab9d1b362034873a60
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277911"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="fb746-103">educationRoot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fb746-103">educationRoot resource type</span></span>

<span data-ttu-id="fb746-104">`/education` 名前空間は、教育機関に固有の機能を公開します。</span><span class="sxs-lookup"><span data-stu-id="fb746-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="fb746-105">`/education` 名前空間の一部のオブジェクトは、Microsoft Graph の別の部分 (たとえば、[users](user.md)) にあります。</span><span class="sxs-lookup"><span data-stu-id="fb746-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="fb746-106">教育機関の名前空間は、これらのオブジェクトに教育機関固有のプロパティと機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="fb746-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="fb746-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="fb746-107">Methods</span></span>

| <span data-ttu-id="fb746-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="fb746-108">Method</span></span>           | <span data-ttu-id="fb746-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fb746-109">Return Type</span></span>    |<span data-ttu-id="fb746-110">説明</span><span class="sxs-lookup"><span data-stu-id="fb746-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fb746-111">Create educationClass</span><span class="sxs-lookup"><span data-stu-id="fb746-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="fb746-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="fb746-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="fb746-113">クラス コレクションに投稿して、新しい **educationClass** を作成します。</span><span class="sxs-lookup"><span data-stu-id="fb746-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="fb746-114">List classes</span><span class="sxs-lookup"><span data-stu-id="fb746-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="fb746-115">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fb746-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="fb746-116">**educationClass** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="fb746-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="fb746-117">Create educationSchool</span><span class="sxs-lookup"><span data-stu-id="fb746-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="fb746-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="fb746-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="fb746-119">学校コレクションに投稿して、新しい **educationSchool** を作成します。</span><span class="sxs-lookup"><span data-stu-id="fb746-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="fb746-120">List schools</span><span class="sxs-lookup"><span data-stu-id="fb746-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="fb746-121">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fb746-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="fb746-122">**educationSchool** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="fb746-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="fb746-123">Create educationUser</span><span class="sxs-lookup"><span data-stu-id="fb746-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="fb746-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="fb746-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="fb746-125">ユーザー コレクションに投稿して、新しい **educationUser** を作成します。</span><span class="sxs-lookup"><span data-stu-id="fb746-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="fb746-126">List users</span><span class="sxs-lookup"><span data-stu-id="fb746-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="fb746-127">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fb746-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="fb746-128">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="fb746-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="fb746-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fb746-129">Properties</span></span>
<span data-ttu-id="fb746-130">なし</span><span class="sxs-lookup"><span data-stu-id="fb746-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="fb746-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fb746-131">Relationships</span></span>
| <span data-ttu-id="fb746-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fb746-132">Relationship</span></span> | <span data-ttu-id="fb746-133">型</span><span class="sxs-lookup"><span data-stu-id="fb746-133">Type</span></span>   |<span data-ttu-id="fb746-134">説明</span><span class="sxs-lookup"><span data-stu-id="fb746-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb746-135">classes</span><span class="sxs-lookup"><span data-stu-id="fb746-135">classes</span></span>|<span data-ttu-id="fb746-136">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fb746-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="fb746-137">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fb746-137">Read-only.</span></span> <span data-ttu-id="fb746-138">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="fb746-138">Nullable.</span></span>|
|<span data-ttu-id="fb746-139">me</span><span class="sxs-lookup"><span data-stu-id="fb746-139">me</span></span>|[<span data-ttu-id="fb746-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="fb746-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="fb746-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fb746-141">Read-only.</span></span> <span data-ttu-id="fb746-142">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="fb746-142">Nullable.</span></span>|
|<span data-ttu-id="fb746-143">schools</span><span class="sxs-lookup"><span data-stu-id="fb746-143">schools</span></span>|<span data-ttu-id="fb746-144">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fb746-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="fb746-p104">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="fb746-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="fb746-147">users</span><span class="sxs-lookup"><span data-stu-id="fb746-147">users</span></span>|<span data-ttu-id="fb746-148">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fb746-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="fb746-p105">読み取り専用。Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="fb746-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fb746-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fb746-151">JSON representation</span></span>
<span data-ttu-id="fb746-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fb746-152">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationRoot"
}-->

```json
{
}
```

<!-- {
  "blockType": "request",
  "name": "get_education"
}-->
```http
GET https://graph.microsoft.com/v1.0/education
```

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRoot"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fb746-153">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="fb746-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fb746-154">C#</span><span class="sxs-lookup"><span data-stu-id="fb746-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_education-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fb746-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="fb746-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_education-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="fb746-156">目的-C</span><span class="sxs-lookup"><span data-stu-id="fb746-156">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_education-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/resources/educationroot.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/resources/educationroot.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/resources/educationroot.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
