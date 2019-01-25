---
title: educationSubmissionResource リソースの種類
description: '提出書類に使用するリソースのラッパーです。 ラッパーは、この課題からコピーされた場合、割り当てリソースにポインターを追加します。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ef231de49d3871ec877c279b4e77585343e1a85e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522078"
---
# <a name="educationsubmissionresource-resource-type"></a><span data-ttu-id="d3248-104">educationSubmissionResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d3248-104">educationSubmissionResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3248-105">提出書類に使用するリソースのラッパーです。</span><span class="sxs-lookup"><span data-stu-id="d3248-105">A wrapper around a resource for use on a submission.</span></span> <span data-ttu-id="d3248-106">ラッパーは、この課題からコピーされた場合、割り当てリソースにポインターを追加します。</span><span class="sxs-lookup"><span data-stu-id="d3248-106">The wrapper adds a pointer to the assignment resource if this was copied from the assignment.</span></span>  


## <a name="methods"></a><span data-ttu-id="d3248-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="d3248-107">Methods</span></span>

| <span data-ttu-id="d3248-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d3248-108">Method</span></span>           | <span data-ttu-id="d3248-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d3248-109">Return Type</span></span>    |<span data-ttu-id="d3248-110">説明</span><span class="sxs-lookup"><span data-stu-id="d3248-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d3248-111">EducationSubmissionResource を取得します。</span><span class="sxs-lookup"><span data-stu-id="d3248-111">Get educationSubmissionResource</span></span>](../api/educationsubmissionresource-get.md) | [<span data-ttu-id="d3248-112">educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="d3248-112">educationSubmissionResource</span></span>](educationsubmissionresource.md) |<span data-ttu-id="d3248-113">**EducationSubmissionResource**オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d3248-113">Read properties and relationships of an **educationSubmissionResource** object.</span></span>|
|[<span data-ttu-id="d3248-114">Delete</span><span class="sxs-lookup"><span data-stu-id="d3248-114">Delete</span></span>](../api/educationsubmissionresource-delete.md) | <span data-ttu-id="d3248-115">なし</span><span class="sxs-lookup"><span data-stu-id="d3248-115">None</span></span> |<span data-ttu-id="d3248-116">**EducationSubmissionResource**オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="d3248-116">Delete an **educationSubmissionResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d3248-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3248-117">Properties</span></span>
| <span data-ttu-id="d3248-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3248-118">Property</span></span>     | <span data-ttu-id="d3248-119">型</span><span class="sxs-lookup"><span data-stu-id="d3248-119">Type</span></span>   |<span data-ttu-id="d3248-120">説明</span><span class="sxs-lookup"><span data-stu-id="d3248-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3248-121">assignmentResourceUrl</span><span class="sxs-lookup"><span data-stu-id="d3248-121">assignmentResourceUrl</span></span>|<span data-ttu-id="d3248-122">String</span><span class="sxs-lookup"><span data-stu-id="d3248-122">String</span></span>|<span data-ttu-id="d3248-123">このリソースのコピー元の割り当てへのポインター。</span><span class="sxs-lookup"><span data-stu-id="d3248-123">Pointer to the assignment from which this resource was copied.</span></span> <span data-ttu-id="d3248-124">これが null の場合、受講者は、リソースをアップロードします。</span><span class="sxs-lookup"><span data-stu-id="d3248-124">If this is null, the student uploaded the resource.</span></span>|
|<span data-ttu-id="d3248-125">id</span><span class="sxs-lookup"><span data-stu-id="d3248-125">id</span></span>|<span data-ttu-id="d3248-126">String</span><span class="sxs-lookup"><span data-stu-id="d3248-126">String</span></span>| <span data-ttu-id="d3248-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d3248-127">Read-only.</span></span>|
|<span data-ttu-id="d3248-128">リソース</span><span class="sxs-lookup"><span data-stu-id="d3248-128">resource</span></span>|[<span data-ttu-id="d3248-129">educationResource</span><span class="sxs-lookup"><span data-stu-id="d3248-129">educationResource</span></span>](educationresource.md)|<span data-ttu-id="d3248-130">Resource オブジェクト</span><span class="sxs-lookup"><span data-stu-id="d3248-130">Resource object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3248-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d3248-131">Relationships</span></span>
<span data-ttu-id="d3248-132">なし</span><span class="sxs-lookup"><span data-stu-id="d3248-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d3248-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d3248-133">JSON representation</span></span>

<span data-ttu-id="d3248-134">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d3248-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmissionResource"
}-->

```json
{
  "assignmentResourceUrl": "String",
  "id": "String (identifier)",
  "resource": {"@odata.type": "microsoft.graph.educationResource"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmissionResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsubmissionresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
