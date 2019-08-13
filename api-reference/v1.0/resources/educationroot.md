---
title: educationRoot リソースの種類
description: '`/education` 名前空間は、教育機関に固有の機能を公開します。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f15634242219ebfc56f0cc4c533661c55863a279
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327147"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="8fbad-103">educationRoot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8fbad-103">educationRoot resource type</span></span>

<span data-ttu-id="8fbad-104">`/education` 名前空間は、教育機関に固有の機能を公開します。</span><span class="sxs-lookup"><span data-stu-id="8fbad-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="8fbad-105">`/education` 名前空間の一部のオブジェクトは、Microsoft Graph の別の部分 (たとえば、[users](user.md)) にあります。</span><span class="sxs-lookup"><span data-stu-id="8fbad-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="8fbad-106">教育機関の名前空間は、これらのオブジェクトに教育機関固有のプロパティと機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="8fbad-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="8fbad-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="8fbad-107">Methods</span></span>

| <span data-ttu-id="8fbad-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="8fbad-108">Method</span></span>           | <span data-ttu-id="8fbad-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8fbad-109">Return Type</span></span>    |<span data-ttu-id="8fbad-110">説明</span><span class="sxs-lookup"><span data-stu-id="8fbad-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8fbad-111">Create educationClass</span><span class="sxs-lookup"><span data-stu-id="8fbad-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="8fbad-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="8fbad-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="8fbad-113">クラス コレクションに投稿して、新しい **educationClass** を作成します。</span><span class="sxs-lookup"><span data-stu-id="8fbad-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="8fbad-114">List classes</span><span class="sxs-lookup"><span data-stu-id="8fbad-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="8fbad-115">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8fbad-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="8fbad-116">**educationClass** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="8fbad-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="8fbad-117">Create educationSchool</span><span class="sxs-lookup"><span data-stu-id="8fbad-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="8fbad-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="8fbad-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="8fbad-119">学校コレクションに投稿して、新しい **educationSchool** を作成します。</span><span class="sxs-lookup"><span data-stu-id="8fbad-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="8fbad-120">List schools</span><span class="sxs-lookup"><span data-stu-id="8fbad-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="8fbad-121">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8fbad-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="8fbad-122">**educationSchool** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="8fbad-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="8fbad-123">Create educationUser</span><span class="sxs-lookup"><span data-stu-id="8fbad-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="8fbad-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="8fbad-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="8fbad-125">ユーザー コレクションに投稿して、新しい **educationUser** を作成します。</span><span class="sxs-lookup"><span data-stu-id="8fbad-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="8fbad-126">List users</span><span class="sxs-lookup"><span data-stu-id="8fbad-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="8fbad-127">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8fbad-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="8fbad-128">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="8fbad-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="8fbad-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8fbad-129">Properties</span></span>
<span data-ttu-id="8fbad-130">なし</span><span class="sxs-lookup"><span data-stu-id="8fbad-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="8fbad-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8fbad-131">Relationships</span></span>
| <span data-ttu-id="8fbad-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8fbad-132">Relationship</span></span> | <span data-ttu-id="8fbad-133">型</span><span class="sxs-lookup"><span data-stu-id="8fbad-133">Type</span></span>   |<span data-ttu-id="8fbad-134">説明</span><span class="sxs-lookup"><span data-stu-id="8fbad-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8fbad-135">classes</span><span class="sxs-lookup"><span data-stu-id="8fbad-135">classes</span></span>|<span data-ttu-id="8fbad-136">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8fbad-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="8fbad-137">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8fbad-137">Read-only.</span></span> <span data-ttu-id="8fbad-138">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="8fbad-138">Nullable.</span></span>|
|<span data-ttu-id="8fbad-139">me</span><span class="sxs-lookup"><span data-stu-id="8fbad-139">me</span></span>|[<span data-ttu-id="8fbad-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="8fbad-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="8fbad-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8fbad-141">Read-only.</span></span> <span data-ttu-id="8fbad-142">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="8fbad-142">Nullable.</span></span>|
|<span data-ttu-id="8fbad-143">schools</span><span class="sxs-lookup"><span data-stu-id="8fbad-143">schools</span></span>|<span data-ttu-id="8fbad-144">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8fbad-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="8fbad-p104">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="8fbad-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="8fbad-147">users</span><span class="sxs-lookup"><span data-stu-id="8fbad-147">users</span></span>|<span data-ttu-id="8fbad-148">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8fbad-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="8fbad-p105">読み取り専用。Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="8fbad-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8fbad-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8fbad-151">JSON representation</span></span>
<span data-ttu-id="8fbad-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8fbad-152">Here is a JSON representation of the resource.</span></span>

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


# <a name="httptabhttp"></a>[<span data-ttu-id="8fbad-153">プロトコル</span><span class="sxs-lookup"><span data-stu-id="8fbad-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_education"
}-->
```http
GET https://graph.microsoft.com/v1.0/education
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8fbad-154">C#</span><span class="sxs-lookup"><span data-stu-id="8fbad-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-education-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8fbad-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8fbad-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-education-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8fbad-156">目的-C</span><span class="sxs-lookup"><span data-stu-id="8fbad-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-education-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8fbad-157">Java</span><span class="sxs-lookup"><span data-stu-id="8fbad-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-education-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
