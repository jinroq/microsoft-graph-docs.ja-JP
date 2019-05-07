---
title: educationRoot リソースの種類
description: '`/education` 名前空間は、教育機関に固有の機能を公開します。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 4ca794bb3fe2d2012cecd1719368df022f44c0ea
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33601831"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="fbc0b-103">educationRoot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fbc0b-103">educationRoot resource type</span></span>

<span data-ttu-id="fbc0b-104">`/education` 名前空間は、教育機関に固有の機能を公開します。</span><span class="sxs-lookup"><span data-stu-id="fbc0b-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="fbc0b-105">`/education` 名前空間の一部のオブジェクトは、Microsoft Graph の別の部分 (たとえば、[users](user.md)) にあります。</span><span class="sxs-lookup"><span data-stu-id="fbc0b-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="fbc0b-106">教育機関の名前空間は、これらのオブジェクトに教育機関固有のプロパティと機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="fbc0b-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="fbc0b-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="fbc0b-107">Methods</span></span>

| <span data-ttu-id="fbc0b-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="fbc0b-108">Method</span></span>           | <span data-ttu-id="fbc0b-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fbc0b-109">Return Type</span></span>    |<span data-ttu-id="fbc0b-110">説明</span><span class="sxs-lookup"><span data-stu-id="fbc0b-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fbc0b-111">Create educationClass</span><span class="sxs-lookup"><span data-stu-id="fbc0b-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="fbc0b-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="fbc0b-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="fbc0b-113">クラス コレクションに投稿して、新しい **educationClass** を作成します。</span><span class="sxs-lookup"><span data-stu-id="fbc0b-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="fbc0b-114">List classes</span><span class="sxs-lookup"><span data-stu-id="fbc0b-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="fbc0b-115">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fbc0b-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="fbc0b-116">**educationClass** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="fbc0b-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="fbc0b-117">Create educationSchool</span><span class="sxs-lookup"><span data-stu-id="fbc0b-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="fbc0b-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="fbc0b-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="fbc0b-119">学校コレクションに投稿して、新しい **educationSchool** を作成します。</span><span class="sxs-lookup"><span data-stu-id="fbc0b-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="fbc0b-120">List schools</span><span class="sxs-lookup"><span data-stu-id="fbc0b-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="fbc0b-121">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fbc0b-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="fbc0b-122">**educationSchool** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="fbc0b-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="fbc0b-123">Create educationUser</span><span class="sxs-lookup"><span data-stu-id="fbc0b-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="fbc0b-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="fbc0b-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="fbc0b-125">ユーザー コレクションに投稿して、新しい **educationUser** を作成します。</span><span class="sxs-lookup"><span data-stu-id="fbc0b-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="fbc0b-126">List users</span><span class="sxs-lookup"><span data-stu-id="fbc0b-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="fbc0b-127">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fbc0b-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="fbc0b-128">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="fbc0b-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="fbc0b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fbc0b-129">Properties</span></span>
<span data-ttu-id="fbc0b-130">なし</span><span class="sxs-lookup"><span data-stu-id="fbc0b-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="fbc0b-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fbc0b-131">Relationships</span></span>
| <span data-ttu-id="fbc0b-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fbc0b-132">Relationship</span></span> | <span data-ttu-id="fbc0b-133">型</span><span class="sxs-lookup"><span data-stu-id="fbc0b-133">Type</span></span>   |<span data-ttu-id="fbc0b-134">説明</span><span class="sxs-lookup"><span data-stu-id="fbc0b-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fbc0b-135">classes</span><span class="sxs-lookup"><span data-stu-id="fbc0b-135">classes</span></span>|<span data-ttu-id="fbc0b-136">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fbc0b-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="fbc0b-137">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="fbc0b-137">Read-only.</span></span> <span data-ttu-id="fbc0b-138">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="fbc0b-138">Nullable.</span></span>|
|<span data-ttu-id="fbc0b-139">me</span><span class="sxs-lookup"><span data-stu-id="fbc0b-139">me</span></span>|[<span data-ttu-id="fbc0b-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="fbc0b-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="fbc0b-141">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="fbc0b-141">Read-only.</span></span> <span data-ttu-id="fbc0b-142">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="fbc0b-142">Nullable.</span></span>|
|<span data-ttu-id="fbc0b-143">schools</span><span class="sxs-lookup"><span data-stu-id="fbc0b-143">schools</span></span>|<span data-ttu-id="fbc0b-144">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fbc0b-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="fbc0b-p104">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="fbc0b-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="fbc0b-147">users</span><span class="sxs-lookup"><span data-stu-id="fbc0b-147">users</span></span>|<span data-ttu-id="fbc0b-148">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fbc0b-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="fbc0b-p105">読み取り専用。Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="fbc0b-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fbc0b-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fbc0b-151">JSON representation</span></span>
<span data-ttu-id="fbc0b-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fbc0b-152">Here is a JSON representation of the resource.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="fbc0b-153">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="fbc0b-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fbc0b-154">Visual</span><span class="sxs-lookup"><span data-stu-id="fbc0b-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_education-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fbc0b-155">Java</span><span class="sxs-lookup"><span data-stu-id="fbc0b-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_education-Javascript-snippets.md)]

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
    "Error: /api-reference/v1.0/resources/educationroot.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/resources/educationroot.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
