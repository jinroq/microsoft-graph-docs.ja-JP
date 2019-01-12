---
title: educationRoot リソースの種類
description: '`/education` 名前空間は、教育機関に固有の機能を公開します。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5b9f17cf82c6839a95f1fd81405aa675e0f4d6ba
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943201"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="23c59-103">educationRoot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="23c59-103">educationRoot resource type</span></span>

<span data-ttu-id="23c59-104">`/education` 名前空間は、教育機関に固有の機能を公開します。</span><span class="sxs-lookup"><span data-stu-id="23c59-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="23c59-105">`/education` 名前空間の一部のオブジェクトは、Microsoft Graph の別の部分 (たとえば、[users](user.md)) にあります。</span><span class="sxs-lookup"><span data-stu-id="23c59-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="23c59-106">教育機関の名前空間は、これらのオブジェクトに教育機関固有のプロパティと機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="23c59-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="23c59-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="23c59-107">Methods</span></span>

| <span data-ttu-id="23c59-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="23c59-108">Method</span></span>           | <span data-ttu-id="23c59-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="23c59-109">Return Type</span></span>    |<span data-ttu-id="23c59-110">説明</span><span class="sxs-lookup"><span data-stu-id="23c59-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="23c59-111">Create educationClass</span><span class="sxs-lookup"><span data-stu-id="23c59-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="23c59-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="23c59-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="23c59-113">クラス コレクションに投稿して、新しい **educationClass** を作成します。</span><span class="sxs-lookup"><span data-stu-id="23c59-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="23c59-114">List classes</span><span class="sxs-lookup"><span data-stu-id="23c59-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="23c59-115">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="23c59-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="23c59-116">**educationClass** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="23c59-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="23c59-117">Create educationSchool</span><span class="sxs-lookup"><span data-stu-id="23c59-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="23c59-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="23c59-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="23c59-119">学校コレクションに投稿して、新しい **educationSchool** を作成します。</span><span class="sxs-lookup"><span data-stu-id="23c59-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="23c59-120">List schools</span><span class="sxs-lookup"><span data-stu-id="23c59-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="23c59-121">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="23c59-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="23c59-122">**educationSchool** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="23c59-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="23c59-123">Create educationUser</span><span class="sxs-lookup"><span data-stu-id="23c59-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="23c59-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="23c59-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="23c59-125">ユーザー コレクションに投稿して、新しい **educationUser** を作成します。</span><span class="sxs-lookup"><span data-stu-id="23c59-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="23c59-126">List users</span><span class="sxs-lookup"><span data-stu-id="23c59-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="23c59-127">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="23c59-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="23c59-128">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="23c59-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="23c59-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23c59-129">Properties</span></span>
<span data-ttu-id="23c59-130">なし</span><span class="sxs-lookup"><span data-stu-id="23c59-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="23c59-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="23c59-131">Relationships</span></span>
| <span data-ttu-id="23c59-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="23c59-132">Relationship</span></span> | <span data-ttu-id="23c59-133">型</span><span class="sxs-lookup"><span data-stu-id="23c59-133">Type</span></span>   |<span data-ttu-id="23c59-134">説明</span><span class="sxs-lookup"><span data-stu-id="23c59-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23c59-135">classes</span><span class="sxs-lookup"><span data-stu-id="23c59-135">classes</span></span>|<span data-ttu-id="23c59-136">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="23c59-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="23c59-p102">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="23c59-p102">Read-only. Nullable.</span></span>|
|<span data-ttu-id="23c59-139">me</span><span class="sxs-lookup"><span data-stu-id="23c59-139">me</span></span>|[<span data-ttu-id="23c59-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="23c59-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="23c59-p103">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="23c59-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="23c59-143">schools</span><span class="sxs-lookup"><span data-stu-id="23c59-143">schools</span></span>|<span data-ttu-id="23c59-144">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="23c59-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="23c59-p104">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="23c59-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="23c59-147">users</span><span class="sxs-lookup"><span data-stu-id="23c59-147">users</span></span>|<span data-ttu-id="23c59-148">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="23c59-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="23c59-p105">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="23c59-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="23c59-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="23c59-151">JSON representation</span></span>
<span data-ttu-id="23c59-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="23c59-152">Here is a JSON representation of the resource.</span></span>

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
