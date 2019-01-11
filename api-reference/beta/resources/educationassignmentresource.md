---
title: educationAssignmentResource リソースの種類
description: 割り当てに関連付けられているリソースを格納するラッパー オブジェクトを返します。 ラッパーが**distributeForStudentWork**プロパティを追加し、このリソースが、あることを示します
localization_priority: Normal
ms.openlocfilehash: 55d978ceb2a3df613ded09682bbdc42009f4e204
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868839"
---
# <a name="educationassignmentresource-resource-type"></a><span data-ttu-id="a2188-104">educationAssignmentResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a2188-104">educationAssignmentResource resource type</span></span>

> <span data-ttu-id="a2188-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a2188-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2188-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2188-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a2188-107">割り当てに関連付けられているリソースを格納するラッパー オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a2188-107">A wrapper object that stores the resources associated with an assignment.</span></span> <span data-ttu-id="a2188-108">ラッパーは、 **distributeForStudentWork**プロパティを追加し、このリソースを受講者の提出書類にコピーされることを示します。</span><span class="sxs-lookup"><span data-stu-id="a2188-108">The wrapper adds the **distributeForStudentWork** property and indicates that this resource will be copied to the student submission.</span></span>  <span data-ttu-id="a2188-109">オブジェクトはコピーされませんが、各受講者は、割り当てのリソースへのリンクが表示されます。</span><span class="sxs-lookup"><span data-stu-id="a2188-109">If the object is not copied, each student will see a link to the resource on the assignment.</span></span> <span data-ttu-id="a2188-110">受講者はこのリソースを更新できません。</span><span class="sxs-lookup"><span data-stu-id="a2188-110">The student will not be able to update this resource.</span></span> <span data-ttu-id="a2188-111">これは、受講者に次ことが何もに、先生からの配布資料です。</span><span class="sxs-lookup"><span data-stu-id="a2188-111">This is a handout from the teacher to the student with nothing to be turned in.</span></span> <span data-ttu-id="a2188-112">リソースが分散している場合は、各受講者がリソースの一覧で、データを送信このリソースのコピーが表示されます。</span><span class="sxs-lookup"><span data-stu-id="a2188-112">If the resource is distributed, each student will receive a copy of this resource in the resource list of their submission.</span></span> <span data-ttu-id="a2188-113">各受講者はそのコピーを変更し、グレーディングのために送信することになります。</span><span class="sxs-lookup"><span data-stu-id="a2188-113">Each student will be able to modify their copy and submit it for grading.</span></span>


## <a name="methods"></a><span data-ttu-id="a2188-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="a2188-114">Methods</span></span>

| <span data-ttu-id="a2188-115">メソッド</span><span class="sxs-lookup"><span data-stu-id="a2188-115">Method</span></span>           | <span data-ttu-id="a2188-116">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a2188-116">Return Type</span></span>    |<span data-ttu-id="a2188-117">説明</span><span class="sxs-lookup"><span data-stu-id="a2188-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a2188-118">EducationAssignmentResource を取得します。</span><span class="sxs-lookup"><span data-stu-id="a2188-118">Get educationAssignmentResource</span></span>](../api/educationassignmentresource-get.md) | [<span data-ttu-id="a2188-119">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="a2188-119">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="a2188-120">**EducationAssignmentResource**オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2188-120">Read properties and relationships of an **educationAssignmentResource** object.</span></span>|
|[<span data-ttu-id="a2188-121">Update</span><span class="sxs-lookup"><span data-stu-id="a2188-121">Update</span></span>](../api/educationassignmentresource-update.md) | [<span data-ttu-id="a2188-122">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="a2188-122">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="a2188-123">**EducationAssignmentResource**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="a2188-123">Update an **educationAssignmentResource** object.</span></span> |
|[<span data-ttu-id="a2188-124">Delete</span><span class="sxs-lookup"><span data-stu-id="a2188-124">Delete</span></span>](../api/educationassignmentresource-delete.md) | <span data-ttu-id="a2188-125">なし</span><span class="sxs-lookup"><span data-stu-id="a2188-125">None</span></span> |<span data-ttu-id="a2188-126">**EducationAssignmentResource**オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="a2188-126">Delete an **educationAssignmentResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a2188-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2188-127">Properties</span></span>
| <span data-ttu-id="a2188-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2188-128">Property</span></span>     | <span data-ttu-id="a2188-129">種類</span><span class="sxs-lookup"><span data-stu-id="a2188-129">Type</span></span>   |<span data-ttu-id="a2188-130">説明</span><span class="sxs-lookup"><span data-stu-id="a2188-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2188-131">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="a2188-131">distributeForStudentWork</span></span>|<span data-ttu-id="a2188-132">ブール型</span><span class="sxs-lookup"><span data-stu-id="a2188-132">Boolean</span></span>|<span data-ttu-id="a2188-133">受講生受講者の変更、および送信のため送信するたびにこのリソースをコピーするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a2188-133">Indicates whether this resource should be copied to each student submission for modification and submission.</span></span>|
|<span data-ttu-id="a2188-134">id</span><span class="sxs-lookup"><span data-stu-id="a2188-134">id</span></span>|<span data-ttu-id="a2188-135">String</span><span class="sxs-lookup"><span data-stu-id="a2188-135">String</span></span>| <span data-ttu-id="a2188-136">このリソースの ID です。</span><span class="sxs-lookup"><span data-stu-id="a2188-136">ID of this resource.</span></span> <span data-ttu-id="a2188-137">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a2188-137">Read-only.</span></span>|
|<span data-ttu-id="a2188-138">resource</span><span class="sxs-lookup"><span data-stu-id="a2188-138">resource</span></span>|[<span data-ttu-id="a2188-139">educationResource</span><span class="sxs-lookup"><span data-stu-id="a2188-139">educationResource</span></span>](educationresource.md)|<span data-ttu-id="a2188-140">リソースがこの割り当てに関連付けられているオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="a2188-140">Resource object that has been associated with this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2188-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a2188-141">Relationships</span></span>
<span data-ttu-id="a2188-142">なし。</span><span class="sxs-lookup"><span data-stu-id="a2188-142">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="a2188-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a2188-143">JSON representation</span></span>

<span data-ttu-id="a2188-144">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a2188-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentResource"
}-->

```json
{
  "distributeForStudentWork": true,
  "id": "String (identifier)",
  "resource": {"@odata.type": "microsoft.graph.educationResource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
