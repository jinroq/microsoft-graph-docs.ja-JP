---
title: educationRoot リソースの種類
description: '`/education` 名前空間は、教育機関に固有の機能を公開します。 '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: cb3f84c3417b2007485cabfa1a1078660f025f5e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840524"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="ccf4d-103">educationRoot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ccf4d-103">educationRoot resource type</span></span>

<span data-ttu-id="ccf4d-104">`/education` 名前空間は、教育機関に固有の機能を公開します。</span><span class="sxs-lookup"><span data-stu-id="ccf4d-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="ccf4d-105">`/education` 名前空間の一部のオブジェクトは、Microsoft Graph の別の部分 (たとえば、[users](user.md)) にあります。</span><span class="sxs-lookup"><span data-stu-id="ccf4d-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="ccf4d-106">教育機関の名前空間は、これらのオブジェクトに教育機関固有のプロパティと機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="ccf4d-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="ccf4d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ccf4d-107">Methods</span></span>

| <span data-ttu-id="ccf4d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ccf4d-108">Method</span></span>           | <span data-ttu-id="ccf4d-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ccf4d-109">Return Type</span></span>    |<span data-ttu-id="ccf4d-110">説明</span><span class="sxs-lookup"><span data-stu-id="ccf4d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ccf4d-111">Create educationClass</span><span class="sxs-lookup"><span data-stu-id="ccf4d-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="ccf4d-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="ccf4d-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="ccf4d-113">クラス コレクションに投稿して、新しい **educationClass** を作成します。</span><span class="sxs-lookup"><span data-stu-id="ccf4d-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="ccf4d-114">List classes</span><span class="sxs-lookup"><span data-stu-id="ccf4d-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="ccf4d-115">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ccf4d-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="ccf4d-116">**educationClass** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="ccf4d-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="ccf4d-117">Create educationSchool</span><span class="sxs-lookup"><span data-stu-id="ccf4d-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="ccf4d-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="ccf4d-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="ccf4d-119">学校コレクションに投稿して、新しい **educationSchool** を作成します。</span><span class="sxs-lookup"><span data-stu-id="ccf4d-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="ccf4d-120">List schools</span><span class="sxs-lookup"><span data-stu-id="ccf4d-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="ccf4d-121">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ccf4d-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="ccf4d-122">**educationSchool** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="ccf4d-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="ccf4d-123">Create educationUser</span><span class="sxs-lookup"><span data-stu-id="ccf4d-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="ccf4d-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="ccf4d-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="ccf4d-125">ユーザー コレクションに投稿して、新しい **educationUser** を作成します。</span><span class="sxs-lookup"><span data-stu-id="ccf4d-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="ccf4d-126">List users</span><span class="sxs-lookup"><span data-stu-id="ccf4d-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="ccf4d-127">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ccf4d-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="ccf4d-128">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="ccf4d-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="ccf4d-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ccf4d-129">Properties</span></span>
<span data-ttu-id="ccf4d-130">なし</span><span class="sxs-lookup"><span data-stu-id="ccf4d-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="ccf4d-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ccf4d-131">Relationships</span></span>
| <span data-ttu-id="ccf4d-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ccf4d-132">Relationship</span></span> | <span data-ttu-id="ccf4d-133">型</span><span class="sxs-lookup"><span data-stu-id="ccf4d-133">Type</span></span>   |<span data-ttu-id="ccf4d-134">説明</span><span class="sxs-lookup"><span data-stu-id="ccf4d-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ccf4d-135">classes</span><span class="sxs-lookup"><span data-stu-id="ccf4d-135">classes</span></span>|<span data-ttu-id="ccf4d-136">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ccf4d-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="ccf4d-p102">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ccf4d-p102">Read-only. Nullable.</span></span>|
|<span data-ttu-id="ccf4d-139">me</span><span class="sxs-lookup"><span data-stu-id="ccf4d-139">me</span></span>|[<span data-ttu-id="ccf4d-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="ccf4d-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="ccf4d-p103">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ccf4d-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="ccf4d-143">schools</span><span class="sxs-lookup"><span data-stu-id="ccf4d-143">schools</span></span>|<span data-ttu-id="ccf4d-144">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ccf4d-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="ccf4d-p104">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ccf4d-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="ccf4d-147">users</span><span class="sxs-lookup"><span data-stu-id="ccf4d-147">users</span></span>|<span data-ttu-id="ccf4d-148">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ccf4d-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="ccf4d-p105">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ccf4d-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ccf4d-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ccf4d-151">JSON representation</span></span>
<span data-ttu-id="ccf4d-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ccf4d-152">Here is a JSON representation of the resource.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
