---
title: educationSubmissionResource リソースの種類
description: '提出物で使用するためにリソースをラップするラッパー。 ラッパーは、割り当てからコピーされた場合、割り当てリソースへのポインターを追加します。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 48f4549354603346e39b5e1f6f387b207e2f14ef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972483"
---
# <a name="educationsubmissionresource-resource-type"></a><span data-ttu-id="f2cac-104">educationSubmissionResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f2cac-104">educationSubmissionResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2cac-105">提出物で使用するためにリソースをラップするラッパー。</span><span class="sxs-lookup"><span data-stu-id="f2cac-105">A wrapper around a resource for use on a submission.</span></span> <span data-ttu-id="f2cac-106">ラッパーは、割り当てからコピーされた場合、割り当てリソースへのポインターを追加します。</span><span class="sxs-lookup"><span data-stu-id="f2cac-106">The wrapper adds a pointer to the assignment resource if this was copied from the assignment.</span></span>  


## <a name="methods"></a><span data-ttu-id="f2cac-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="f2cac-107">Methods</span></span>

| <span data-ttu-id="f2cac-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="f2cac-108">Method</span></span>           | <span data-ttu-id="f2cac-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f2cac-109">Return Type</span></span>    |<span data-ttu-id="f2cac-110">説明</span><span class="sxs-lookup"><span data-stu-id="f2cac-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f2cac-111">EducationSubmissionResource を取得する</span><span class="sxs-lookup"><span data-stu-id="f2cac-111">Get educationSubmissionResource</span></span>](../api/educationsubmissionresource-get.md) | [<span data-ttu-id="f2cac-112">educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="f2cac-112">educationSubmissionResource</span></span>](educationsubmissionresource.md) |<span data-ttu-id="f2cac-113">**EducationSubmissionResource**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f2cac-113">Read properties and relationships of an **educationSubmissionResource** object.</span></span>|
|[<span data-ttu-id="f2cac-114">Delete</span><span class="sxs-lookup"><span data-stu-id="f2cac-114">Delete</span></span>](../api/educationsubmissionresource-delete.md) | <span data-ttu-id="f2cac-115">None</span><span class="sxs-lookup"><span data-stu-id="f2cac-115">None</span></span> |<span data-ttu-id="f2cac-116">**EducationSubmissionResource**オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="f2cac-116">Delete an **educationSubmissionResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f2cac-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2cac-117">Properties</span></span>
| <span data-ttu-id="f2cac-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2cac-118">Property</span></span>     | <span data-ttu-id="f2cac-119">型</span><span class="sxs-lookup"><span data-stu-id="f2cac-119">Type</span></span>   |<span data-ttu-id="f2cac-120">説明</span><span class="sxs-lookup"><span data-stu-id="f2cac-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2cac-121">割り当て Resourceurl</span><span class="sxs-lookup"><span data-stu-id="f2cac-121">assignmentResourceUrl</span></span>|<span data-ttu-id="f2cac-122">String</span><span class="sxs-lookup"><span data-stu-id="f2cac-122">String</span></span>|<span data-ttu-id="f2cac-123">このリソースがコピーされた割り当てへのポインター。</span><span class="sxs-lookup"><span data-stu-id="f2cac-123">Pointer to the assignment from which this resource was copied.</span></span> <span data-ttu-id="f2cac-124">この値が null の場合、学生はリソースをアップロードしました。</span><span class="sxs-lookup"><span data-stu-id="f2cac-124">If this is null, the student uploaded the resource.</span></span>|
|<span data-ttu-id="f2cac-125">id</span><span class="sxs-lookup"><span data-stu-id="f2cac-125">id</span></span>|<span data-ttu-id="f2cac-126">String</span><span class="sxs-lookup"><span data-stu-id="f2cac-126">String</span></span>| <span data-ttu-id="f2cac-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f2cac-127">Read-only.</span></span>|
|<span data-ttu-id="f2cac-128">リソース</span><span class="sxs-lookup"><span data-stu-id="f2cac-128">resource</span></span>|[<span data-ttu-id="f2cac-129">educationResource</span><span class="sxs-lookup"><span data-stu-id="f2cac-129">educationResource</span></span>](educationresource.md)|<span data-ttu-id="f2cac-130">Resource オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="f2cac-130">Resource object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2cac-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f2cac-131">Relationships</span></span>
<span data-ttu-id="f2cac-132">なし</span><span class="sxs-lookup"><span data-stu-id="f2cac-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f2cac-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f2cac-133">JSON representation</span></span>

<span data-ttu-id="f2cac-134">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f2cac-134">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
