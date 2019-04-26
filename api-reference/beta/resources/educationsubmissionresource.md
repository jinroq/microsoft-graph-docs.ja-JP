---
title: educationSubmissionResource リソースの種類
description: '提出物で使用するためにリソースをラップするラッパー。 ラッパーは、割り当てからコピーされた場合、割り当てリソースへのポインターを追加します。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b96607a0d37a3ec8af0f6ff0bad61215d6e9008c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340591"
---
# <a name="educationsubmissionresource-resource-type"></a><span data-ttu-id="bbe31-104">educationSubmissionResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bbe31-104">educationSubmissionResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbe31-105">提出物で使用するためにリソースをラップするラッパー。</span><span class="sxs-lookup"><span data-stu-id="bbe31-105">A wrapper around a resource for use on a submission.</span></span> <span data-ttu-id="bbe31-106">ラッパーは、割り当てからコピーされた場合、割り当てリソースへのポインターを追加します。</span><span class="sxs-lookup"><span data-stu-id="bbe31-106">The wrapper adds a pointer to the assignment resource if this was copied from the assignment.</span></span>  


## <a name="methods"></a><span data-ttu-id="bbe31-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="bbe31-107">Methods</span></span>

| <span data-ttu-id="bbe31-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="bbe31-108">Method</span></span>           | <span data-ttu-id="bbe31-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bbe31-109">Return Type</span></span>    |<span data-ttu-id="bbe31-110">説明</span><span class="sxs-lookup"><span data-stu-id="bbe31-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bbe31-111">educationSubmissionResource を取得する</span><span class="sxs-lookup"><span data-stu-id="bbe31-111">Get educationSubmissionResource</span></span>](../api/educationsubmissionresource-get.md) | [<span data-ttu-id="bbe31-112">educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="bbe31-112">educationSubmissionResource</span></span>](educationsubmissionresource.md) |<span data-ttu-id="bbe31-113">**educationSubmissionResource**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bbe31-113">Read properties and relationships of an **educationSubmissionResource** object.</span></span>|
|[<span data-ttu-id="bbe31-114">削除</span><span class="sxs-lookup"><span data-stu-id="bbe31-114">Delete</span></span>](../api/educationsubmissionresource-delete.md) | <span data-ttu-id="bbe31-115">なし</span><span class="sxs-lookup"><span data-stu-id="bbe31-115">None</span></span> |<span data-ttu-id="bbe31-116">**educationSubmissionResource**オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="bbe31-116">Delete an **educationSubmissionResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="bbe31-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bbe31-117">Properties</span></span>
| <span data-ttu-id="bbe31-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bbe31-118">Property</span></span>     | <span data-ttu-id="bbe31-119">型</span><span class="sxs-lookup"><span data-stu-id="bbe31-119">Type</span></span>   |<span data-ttu-id="bbe31-120">説明</span><span class="sxs-lookup"><span data-stu-id="bbe31-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bbe31-121">割り当て resourceurl</span><span class="sxs-lookup"><span data-stu-id="bbe31-121">assignmentResourceUrl</span></span>|<span data-ttu-id="bbe31-122">String</span><span class="sxs-lookup"><span data-stu-id="bbe31-122">String</span></span>|<span data-ttu-id="bbe31-123">このリソースがコピーされた割り当てへのポインター。</span><span class="sxs-lookup"><span data-stu-id="bbe31-123">Pointer to the assignment from which this resource was copied.</span></span> <span data-ttu-id="bbe31-124">この値が null の場合、学生はリソースをアップロードしました。</span><span class="sxs-lookup"><span data-stu-id="bbe31-124">If this is null, the student uploaded the resource.</span></span>|
|<span data-ttu-id="bbe31-125">id</span><span class="sxs-lookup"><span data-stu-id="bbe31-125">id</span></span>|<span data-ttu-id="bbe31-126">String</span><span class="sxs-lookup"><span data-stu-id="bbe31-126">String</span></span>| <span data-ttu-id="bbe31-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bbe31-127">Read-only.</span></span>|
|<span data-ttu-id="bbe31-128">リソース</span><span class="sxs-lookup"><span data-stu-id="bbe31-128">resource</span></span>|[<span data-ttu-id="bbe31-129">educationResource</span><span class="sxs-lookup"><span data-stu-id="bbe31-129">educationResource</span></span>](educationresource.md)|<span data-ttu-id="bbe31-130">Resource オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="bbe31-130">Resource object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bbe31-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bbe31-131">Relationships</span></span>
<span data-ttu-id="bbe31-132">なし</span><span class="sxs-lookup"><span data-stu-id="bbe31-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="bbe31-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bbe31-133">JSON representation</span></span>

<span data-ttu-id="bbe31-134">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bbe31-134">The following is a JSON representation of the resource.</span></span>

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
