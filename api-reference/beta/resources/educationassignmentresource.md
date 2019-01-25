---
title: educationAssignmentResource リソースの種類
description: 割り当てに関連付けられているリソースを格納するラッパー オブジェクトを返します。 ラッパーが**distributeForStudentWork**プロパティを追加し、このリソースが、あることを示します
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 4d05cf5307e77dc6a7ac438c1bd4f4af4e73784e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529230"
---
# <a name="educationassignmentresource-resource-type"></a><span data-ttu-id="60fc1-104">educationAssignmentResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="60fc1-104">educationAssignmentResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60fc1-105">割り当てに関連付けられているリソースを格納するラッパー オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="60fc1-105">A wrapper object that stores the resources associated with an assignment.</span></span> <span data-ttu-id="60fc1-106">ラッパーは、 **distributeForStudentWork**プロパティを追加し、このリソースを受講者の提出書類にコピーされることを示します。</span><span class="sxs-lookup"><span data-stu-id="60fc1-106">The wrapper adds the **distributeForStudentWork** property and indicates that this resource will be copied to the student submission.</span></span>  <span data-ttu-id="60fc1-107">オブジェクトはコピーされませんが、各受講者は、割り当てのリソースへのリンクが表示されます。</span><span class="sxs-lookup"><span data-stu-id="60fc1-107">If the object is not copied, each student will see a link to the resource on the assignment.</span></span> <span data-ttu-id="60fc1-108">受講者はこのリソースを更新できません。</span><span class="sxs-lookup"><span data-stu-id="60fc1-108">The student will not be able to update this resource.</span></span> <span data-ttu-id="60fc1-109">これは、受講者に次ことが何もに、先生からの配布資料です。</span><span class="sxs-lookup"><span data-stu-id="60fc1-109">This is a handout from the teacher to the student with nothing to be turned in.</span></span> <span data-ttu-id="60fc1-110">リソースが分散している場合は、各受講者がリソースの一覧で、データを送信このリソースのコピーが表示されます。</span><span class="sxs-lookup"><span data-stu-id="60fc1-110">If the resource is distributed, each student will receive a copy of this resource in the resource list of their submission.</span></span> <span data-ttu-id="60fc1-111">各受講者はそのコピーを変更し、グレーディングのために送信することになります。</span><span class="sxs-lookup"><span data-stu-id="60fc1-111">Each student will be able to modify their copy and submit it for grading.</span></span>


## <a name="methods"></a><span data-ttu-id="60fc1-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="60fc1-112">Methods</span></span>

| <span data-ttu-id="60fc1-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="60fc1-113">Method</span></span>           | <span data-ttu-id="60fc1-114">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="60fc1-114">Return Type</span></span>    |<span data-ttu-id="60fc1-115">説明</span><span class="sxs-lookup"><span data-stu-id="60fc1-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="60fc1-116">EducationAssignmentResource を取得します。</span><span class="sxs-lookup"><span data-stu-id="60fc1-116">Get educationAssignmentResource</span></span>](../api/educationassignmentresource-get.md) | [<span data-ttu-id="60fc1-117">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="60fc1-117">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="60fc1-118">**EducationAssignmentResource**オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="60fc1-118">Read properties and relationships of an **educationAssignmentResource** object.</span></span>|
|[<span data-ttu-id="60fc1-119">Update</span><span class="sxs-lookup"><span data-stu-id="60fc1-119">Update</span></span>](../api/educationassignmentresource-update.md) | [<span data-ttu-id="60fc1-120">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="60fc1-120">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="60fc1-121">**EducationAssignmentResource**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="60fc1-121">Update an **educationAssignmentResource** object.</span></span> |
|[<span data-ttu-id="60fc1-122">Delete</span><span class="sxs-lookup"><span data-stu-id="60fc1-122">Delete</span></span>](../api/educationassignmentresource-delete.md) | <span data-ttu-id="60fc1-123">なし</span><span class="sxs-lookup"><span data-stu-id="60fc1-123">None</span></span> |<span data-ttu-id="60fc1-124">**EducationAssignmentResource**オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="60fc1-124">Delete an **educationAssignmentResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="60fc1-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60fc1-125">Properties</span></span>
| <span data-ttu-id="60fc1-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60fc1-126">Property</span></span>     | <span data-ttu-id="60fc1-127">型</span><span class="sxs-lookup"><span data-stu-id="60fc1-127">Type</span></span>   |<span data-ttu-id="60fc1-128">説明</span><span class="sxs-lookup"><span data-stu-id="60fc1-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60fc1-129">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="60fc1-129">distributeForStudentWork</span></span>|<span data-ttu-id="60fc1-130">ブール値</span><span class="sxs-lookup"><span data-stu-id="60fc1-130">Boolean</span></span>|<span data-ttu-id="60fc1-131">受講生受講者の変更、および送信のため送信するたびにこのリソースをコピーするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="60fc1-131">Indicates whether this resource should be copied to each student submission for modification and submission.</span></span>|
|<span data-ttu-id="60fc1-132">id</span><span class="sxs-lookup"><span data-stu-id="60fc1-132">id</span></span>|<span data-ttu-id="60fc1-133">String</span><span class="sxs-lookup"><span data-stu-id="60fc1-133">String</span></span>| <span data-ttu-id="60fc1-134">このリソースの ID です。</span><span class="sxs-lookup"><span data-stu-id="60fc1-134">ID of this resource.</span></span> <span data-ttu-id="60fc1-135">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="60fc1-135">Read-only.</span></span>|
|<span data-ttu-id="60fc1-136">リソース</span><span class="sxs-lookup"><span data-stu-id="60fc1-136">resource</span></span>|[<span data-ttu-id="60fc1-137">educationResource</span><span class="sxs-lookup"><span data-stu-id="60fc1-137">educationResource</span></span>](educationresource.md)|<span data-ttu-id="60fc1-138">リソースがこの割り当てに関連付けられているオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="60fc1-138">Resource object that has been associated with this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60fc1-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="60fc1-139">Relationships</span></span>
<span data-ttu-id="60fc1-140">なし。</span><span class="sxs-lookup"><span data-stu-id="60fc1-140">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="60fc1-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="60fc1-141">JSON representation</span></span>

<span data-ttu-id="60fc1-142">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="60fc1-142">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
