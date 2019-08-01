---
title: educationRoot リソースの種類
description: '`/education` 名前空間は、教育機関に固有の機能を公開します。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0742621ccf5261c3d4e3d9de5d185aa7e0ec3dfa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030528"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="899dd-103">educationRoot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="899dd-103">educationRoot resource type</span></span>

<span data-ttu-id="899dd-104">`/education` 名前空間は、教育機関に固有の機能を公開します。</span><span class="sxs-lookup"><span data-stu-id="899dd-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="899dd-105">`/education` 名前空間の一部のオブジェクトは、Microsoft Graph の別の部分 (たとえば、[users](user.md)) にあります。</span><span class="sxs-lookup"><span data-stu-id="899dd-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="899dd-106">教育機関の名前空間は、これらのオブジェクトに教育機関固有のプロパティと機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="899dd-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="899dd-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="899dd-107">Methods</span></span>

| <span data-ttu-id="899dd-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="899dd-108">Method</span></span>           | <span data-ttu-id="899dd-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="899dd-109">Return Type</span></span>    |<span data-ttu-id="899dd-110">説明</span><span class="sxs-lookup"><span data-stu-id="899dd-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="899dd-111">Create educationClass</span><span class="sxs-lookup"><span data-stu-id="899dd-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="899dd-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="899dd-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="899dd-113">クラス コレクションに投稿して、新しい **educationClass** を作成します。</span><span class="sxs-lookup"><span data-stu-id="899dd-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="899dd-114">List classes</span><span class="sxs-lookup"><span data-stu-id="899dd-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="899dd-115">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="899dd-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="899dd-116">**educationClass** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="899dd-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="899dd-117">Create educationSchool</span><span class="sxs-lookup"><span data-stu-id="899dd-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="899dd-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="899dd-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="899dd-119">学校コレクションに投稿して、新しい **educationSchool** を作成します。</span><span class="sxs-lookup"><span data-stu-id="899dd-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="899dd-120">List schools</span><span class="sxs-lookup"><span data-stu-id="899dd-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="899dd-121">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="899dd-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="899dd-122">**educationSchool** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="899dd-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="899dd-123">Create educationUser</span><span class="sxs-lookup"><span data-stu-id="899dd-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="899dd-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="899dd-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="899dd-125">ユーザー コレクションに投稿して、新しい **educationUser** を作成します。</span><span class="sxs-lookup"><span data-stu-id="899dd-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="899dd-126">List users</span><span class="sxs-lookup"><span data-stu-id="899dd-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="899dd-127">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="899dd-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="899dd-128">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="899dd-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="899dd-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="899dd-129">Properties</span></span>
<span data-ttu-id="899dd-130">なし</span><span class="sxs-lookup"><span data-stu-id="899dd-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="899dd-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="899dd-131">Relationships</span></span>
| <span data-ttu-id="899dd-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="899dd-132">Relationship</span></span> | <span data-ttu-id="899dd-133">型</span><span class="sxs-lookup"><span data-stu-id="899dd-133">Type</span></span>   |<span data-ttu-id="899dd-134">説明</span><span class="sxs-lookup"><span data-stu-id="899dd-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="899dd-135">classes</span><span class="sxs-lookup"><span data-stu-id="899dd-135">classes</span></span>|<span data-ttu-id="899dd-136">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="899dd-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="899dd-137">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="899dd-137">Read-only.</span></span> <span data-ttu-id="899dd-138">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="899dd-138">Nullable.</span></span>|
|<span data-ttu-id="899dd-139">me</span><span class="sxs-lookup"><span data-stu-id="899dd-139">me</span></span>|[<span data-ttu-id="899dd-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="899dd-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="899dd-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="899dd-141">Read-only.</span></span> <span data-ttu-id="899dd-142">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="899dd-142">Nullable.</span></span>|
|<span data-ttu-id="899dd-143">schools</span><span class="sxs-lookup"><span data-stu-id="899dd-143">schools</span></span>|<span data-ttu-id="899dd-144">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="899dd-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="899dd-p104">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="899dd-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="899dd-147">users</span><span class="sxs-lookup"><span data-stu-id="899dd-147">users</span></span>|<span data-ttu-id="899dd-148">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="899dd-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="899dd-p105">読み取り専用。Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="899dd-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="899dd-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="899dd-151">JSON representation</span></span>
<span data-ttu-id="899dd-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="899dd-152">Here is a JSON representation of the resource.</span></span>

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


# <a name="httptabhttp"></a>[<span data-ttu-id="899dd-153">プロトコル</span><span class="sxs-lookup"><span data-stu-id="899dd-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_education"
}-->
```http
GET https://graph.microsoft.com/v1.0/education
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="899dd-154">C#</span><span class="sxs-lookup"><span data-stu-id="899dd-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-education-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="899dd-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="899dd-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-education-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="899dd-156">目的-C</span><span class="sxs-lookup"><span data-stu-id="899dd-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-education-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="899dd-157">Java</span><span class="sxs-lookup"><span data-stu-id="899dd-157">Java</span></span>](#tab/java)
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
