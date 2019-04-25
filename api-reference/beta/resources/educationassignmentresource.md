---
title: educationAssignmentResource リソースの種類
description: 割り当てに関連付けられているリソースを格納するラッパーオブジェクト。 ラッパーは**distributeForStudentWork**プロパティを追加し、このリソースが
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 4d05cf5307e77dc6a7ac438c1bd4f4af4e73784e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542986"
---
# <a name="educationassignmentresource-resource-type"></a><span data-ttu-id="48f2b-104">educationAssignmentResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="48f2b-104">educationAssignmentResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48f2b-105">割り当てに関連付けられているリソースを格納するラッパーオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="48f2b-105">A wrapper object that stores the resources associated with an assignment.</span></span> <span data-ttu-id="48f2b-106">ラッパーは**distributeForStudentWork**プロパティを追加し、このリソースが学生送信にコピーされることを示します。</span><span class="sxs-lookup"><span data-stu-id="48f2b-106">The wrapper adds the **distributeForStudentWork** property and indicates that this resource will be copied to the student submission.</span></span>  <span data-ttu-id="48f2b-107">オブジェクトがコピーされていない場合、各学生には割り当てのリソースへのリンクが表示されます。</span><span class="sxs-lookup"><span data-stu-id="48f2b-107">If the object is not copied, each student will see a link to the resource on the assignment.</span></span> <span data-ttu-id="48f2b-108">学生は、このリソースを更新できません。</span><span class="sxs-lookup"><span data-stu-id="48f2b-108">The student will not be able to update this resource.</span></span> <span data-ttu-id="48f2b-109">これは、教師から、何も有効にしていない学生への配布資料です。</span><span class="sxs-lookup"><span data-stu-id="48f2b-109">This is a handout from the teacher to the student with nothing to be turned in.</span></span> <span data-ttu-id="48f2b-110">リソースが分散されている場合、各学生は、提出物のリソースリストにこのリソースのコピーを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="48f2b-110">If the resource is distributed, each student will receive a copy of this resource in the resource list of their submission.</span></span> <span data-ttu-id="48f2b-111">各学生は、お客様のコピーを変更して、更新のために提出することができます。</span><span class="sxs-lookup"><span data-stu-id="48f2b-111">Each student will be able to modify their copy and submit it for grading.</span></span>


## <a name="methods"></a><span data-ttu-id="48f2b-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="48f2b-112">Methods</span></span>

| <span data-ttu-id="48f2b-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="48f2b-113">Method</span></span>           | <span data-ttu-id="48f2b-114">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="48f2b-114">Return Type</span></span>    |<span data-ttu-id="48f2b-115">説明</span><span class="sxs-lookup"><span data-stu-id="48f2b-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="48f2b-116">educationAssignmentResource を取得する</span><span class="sxs-lookup"><span data-stu-id="48f2b-116">Get educationAssignmentResource</span></span>](../api/educationassignmentresource-get.md) | [<span data-ttu-id="48f2b-117">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="48f2b-117">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="48f2b-118">**educationAssignmentResource**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="48f2b-118">Read properties and relationships of an **educationAssignmentResource** object.</span></span>|
|[<span data-ttu-id="48f2b-119">更新</span><span class="sxs-lookup"><span data-stu-id="48f2b-119">Update</span></span>](../api/educationassignmentresource-update.md) | [<span data-ttu-id="48f2b-120">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="48f2b-120">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="48f2b-121">**educationAssignmentResource**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="48f2b-121">Update an **educationAssignmentResource** object.</span></span> |
|[<span data-ttu-id="48f2b-122">削除</span><span class="sxs-lookup"><span data-stu-id="48f2b-122">Delete</span></span>](../api/educationassignmentresource-delete.md) | <span data-ttu-id="48f2b-123">なし</span><span class="sxs-lookup"><span data-stu-id="48f2b-123">None</span></span> |<span data-ttu-id="48f2b-124">**educationAssignmentResource**オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="48f2b-124">Delete an **educationAssignmentResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="48f2b-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48f2b-125">Properties</span></span>
| <span data-ttu-id="48f2b-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48f2b-126">Property</span></span>     | <span data-ttu-id="48f2b-127">型</span><span class="sxs-lookup"><span data-stu-id="48f2b-127">Type</span></span>   |<span data-ttu-id="48f2b-128">説明</span><span class="sxs-lookup"><span data-stu-id="48f2b-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48f2b-129">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="48f2b-129">distributeForStudentWork</span></span>|<span data-ttu-id="48f2b-130">ブール値</span><span class="sxs-lookup"><span data-stu-id="48f2b-130">Boolean</span></span>|<span data-ttu-id="48f2b-131">このリソースを各学生送信にコピーして変更および提出する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="48f2b-131">Indicates whether this resource should be copied to each student submission for modification and submission.</span></span>|
|<span data-ttu-id="48f2b-132">id</span><span class="sxs-lookup"><span data-stu-id="48f2b-132">id</span></span>|<span data-ttu-id="48f2b-133">String</span><span class="sxs-lookup"><span data-stu-id="48f2b-133">String</span></span>| <span data-ttu-id="48f2b-134">このリソースの ID。</span><span class="sxs-lookup"><span data-stu-id="48f2b-134">ID of this resource.</span></span> <span data-ttu-id="48f2b-135">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="48f2b-135">Read-only.</span></span>|
|<span data-ttu-id="48f2b-136">リソース</span><span class="sxs-lookup"><span data-stu-id="48f2b-136">resource</span></span>|[<span data-ttu-id="48f2b-137">educationResource</span><span class="sxs-lookup"><span data-stu-id="48f2b-137">educationResource</span></span>](educationresource.md)|<span data-ttu-id="48f2b-138">この割り当てに関連付けられているリソースオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="48f2b-138">Resource object that has been associated with this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48f2b-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="48f2b-139">Relationships</span></span>
<span data-ttu-id="48f2b-140">なし。</span><span class="sxs-lookup"><span data-stu-id="48f2b-140">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="48f2b-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="48f2b-141">JSON representation</span></span>

<span data-ttu-id="48f2b-142">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="48f2b-142">The following is a JSON representation of the resource.</span></span>

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
