---
title: educationAssignmentResource リソースの種類
description: 割り当てに関連付けられているリソースを格納するラッパーオブジェクト。 ラッパーは**distributeForStudentWork**プロパティを追加し、このリソースが
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 08a716edabc31c83a7fb3e358fbafd023d5fa784
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334411"
---
# <a name="educationassignmentresource-resource-type"></a><span data-ttu-id="945d9-104">educationAssignmentResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="945d9-104">educationAssignmentResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="945d9-105">割り当てに関連付けられているリソースを格納するラッパーオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="945d9-105">A wrapper object that stores the resources associated with an assignment.</span></span> <span data-ttu-id="945d9-106">ラッパーは**distributeForStudentWork**プロパティを追加し、このリソースが学生送信にコピーされることを示します。</span><span class="sxs-lookup"><span data-stu-id="945d9-106">The wrapper adds the **distributeForStudentWork** property and indicates that this resource will be copied to the student submission.</span></span>  <span data-ttu-id="945d9-107">オブジェクトがコピーされていない場合、各学生には割り当てのリソースへのリンクが表示されます。</span><span class="sxs-lookup"><span data-stu-id="945d9-107">If the object is not copied, each student will see a link to the resource on the assignment.</span></span> <span data-ttu-id="945d9-108">学生は、このリソースを更新できません。</span><span class="sxs-lookup"><span data-stu-id="945d9-108">The student will not be able to update this resource.</span></span> <span data-ttu-id="945d9-109">これは、教師から、何も有効にしていない学生への配布資料です。</span><span class="sxs-lookup"><span data-stu-id="945d9-109">This is a handout from the teacher to the student with nothing to be turned in.</span></span> <span data-ttu-id="945d9-110">リソースが分散されている場合、各学生は、提出物のリソースリストにこのリソースのコピーを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="945d9-110">If the resource is distributed, each student will receive a copy of this resource in the resource list of their submission.</span></span> <span data-ttu-id="945d9-111">各学生は、お客様のコピーを変更して、更新のために提出することができます。</span><span class="sxs-lookup"><span data-stu-id="945d9-111">Each student will be able to modify their copy and submit it for grading.</span></span>


## <a name="methods"></a><span data-ttu-id="945d9-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="945d9-112">Methods</span></span>

| <span data-ttu-id="945d9-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="945d9-113">Method</span></span>           | <span data-ttu-id="945d9-114">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="945d9-114">Return Type</span></span>    |<span data-ttu-id="945d9-115">説明</span><span class="sxs-lookup"><span data-stu-id="945d9-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="945d9-116">educationAssignmentResource を取得する</span><span class="sxs-lookup"><span data-stu-id="945d9-116">Get educationAssignmentResource</span></span>](../api/educationassignmentresource-get.md) | [<span data-ttu-id="945d9-117">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="945d9-117">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="945d9-118">**educationAssignmentResource**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="945d9-118">Read properties and relationships of an **educationAssignmentResource** object.</span></span>|
|[<span data-ttu-id="945d9-119">更新する</span><span class="sxs-lookup"><span data-stu-id="945d9-119">Update</span></span>](../api/educationassignmentresource-update.md) | [<span data-ttu-id="945d9-120">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="945d9-120">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="945d9-121">**educationAssignmentResource**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="945d9-121">Update an **educationAssignmentResource** object.</span></span> |
|[<span data-ttu-id="945d9-122">削除</span><span class="sxs-lookup"><span data-stu-id="945d9-122">Delete</span></span>](../api/educationassignmentresource-delete.md) | <span data-ttu-id="945d9-123">なし</span><span class="sxs-lookup"><span data-stu-id="945d9-123">None</span></span> |<span data-ttu-id="945d9-124">**educationAssignmentResource**オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="945d9-124">Delete an **educationAssignmentResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="945d9-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="945d9-125">Properties</span></span>
| <span data-ttu-id="945d9-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="945d9-126">Property</span></span>     | <span data-ttu-id="945d9-127">型</span><span class="sxs-lookup"><span data-stu-id="945d9-127">Type</span></span>   |<span data-ttu-id="945d9-128">説明</span><span class="sxs-lookup"><span data-stu-id="945d9-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="945d9-129">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="945d9-129">distributeForStudentWork</span></span>|<span data-ttu-id="945d9-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="945d9-130">Boolean</span></span>|<span data-ttu-id="945d9-131">このリソースを各学生送信にコピーして変更および提出する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="945d9-131">Indicates whether this resource should be copied to each student submission for modification and submission.</span></span>|
|<span data-ttu-id="945d9-132">id</span><span class="sxs-lookup"><span data-stu-id="945d9-132">id</span></span>|<span data-ttu-id="945d9-133">String</span><span class="sxs-lookup"><span data-stu-id="945d9-133">String</span></span>| <span data-ttu-id="945d9-134">このリソースの ID。</span><span class="sxs-lookup"><span data-stu-id="945d9-134">ID of this resource.</span></span> <span data-ttu-id="945d9-135">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="945d9-135">Read-only.</span></span>|
|<span data-ttu-id="945d9-136">リソース</span><span class="sxs-lookup"><span data-stu-id="945d9-136">resource</span></span>|[<span data-ttu-id="945d9-137">educationResource</span><span class="sxs-lookup"><span data-stu-id="945d9-137">educationResource</span></span>](educationresource.md)|<span data-ttu-id="945d9-138">この割り当てに関連付けられているリソースオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="945d9-138">Resource object that has been associated with this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="945d9-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="945d9-139">Relationships</span></span>
<span data-ttu-id="945d9-140">なし。</span><span class="sxs-lookup"><span data-stu-id="945d9-140">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="945d9-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="945d9-141">JSON representation</span></span>

<span data-ttu-id="945d9-142">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="945d9-142">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
