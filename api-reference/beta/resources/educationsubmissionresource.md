---
title: educationSubmissionResource リソースの種類
description: '提出書類に使用するリソースのラッパーです。 ラッパーは、この課題からコピーされた場合、割り当てリソースにポインターを追加します。  '
author: dipakboyed
ms.openlocfilehash: bfbf2f522106f5a1e2033898cbb2702223d3e241
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361559"
---
# <a name="educationsubmissionresource-resource-type"></a><span data-ttu-id="c9a27-104">educationSubmissionResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c9a27-104">educationSubmissionResource resource type</span></span>

> <span data-ttu-id="c9a27-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c9a27-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9a27-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9a27-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c9a27-107">提出書類に使用するリソースのラッパーです。</span><span class="sxs-lookup"><span data-stu-id="c9a27-107">A wrapper around a resource for use on a submission.</span></span> <span data-ttu-id="c9a27-108">ラッパーは、この課題からコピーされた場合、割り当てリソースにポインターを追加します。</span><span class="sxs-lookup"><span data-stu-id="c9a27-108">The wrapper adds a pointer to the assignment resource if this was copied from the assignment.</span></span>  


## <a name="methods"></a><span data-ttu-id="c9a27-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="c9a27-109">Methods</span></span>

| <span data-ttu-id="c9a27-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="c9a27-110">Method</span></span>           | <span data-ttu-id="c9a27-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c9a27-111">Return Type</span></span>    |<span data-ttu-id="c9a27-112">説明</span><span class="sxs-lookup"><span data-stu-id="c9a27-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c9a27-113">EducationSubmissionResource を取得します。</span><span class="sxs-lookup"><span data-stu-id="c9a27-113">Get educationSubmissionResource</span></span>](../api/educationsubmissionresource-get.md) | [<span data-ttu-id="c9a27-114">educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="c9a27-114">educationSubmissionResource</span></span>](educationsubmissionresource.md) |<span data-ttu-id="c9a27-115">**EducationSubmissionResource**オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c9a27-115">Read properties and relationships of an **educationSubmissionResource** object.</span></span>|
|[<span data-ttu-id="c9a27-116">Delete</span><span class="sxs-lookup"><span data-stu-id="c9a27-116">Delete</span></span>](../api/educationsubmissionresource-delete.md) | <span data-ttu-id="c9a27-117">なし</span><span class="sxs-lookup"><span data-stu-id="c9a27-117">None</span></span> |<span data-ttu-id="c9a27-118">**EducationSubmissionResource**オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="c9a27-118">Delete an **educationSubmissionResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c9a27-119">Properties</span><span class="sxs-lookup"><span data-stu-id="c9a27-119">Properties</span></span>
| <span data-ttu-id="c9a27-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9a27-120">Property</span></span>     | <span data-ttu-id="c9a27-121">種類</span><span class="sxs-lookup"><span data-stu-id="c9a27-121">Type</span></span>   |<span data-ttu-id="c9a27-122">説明</span><span class="sxs-lookup"><span data-stu-id="c9a27-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9a27-123">assignmentResourceUrl</span><span class="sxs-lookup"><span data-stu-id="c9a27-123">assignmentResourceUrl</span></span>|<span data-ttu-id="c9a27-124">String</span><span class="sxs-lookup"><span data-stu-id="c9a27-124">String</span></span>|<span data-ttu-id="c9a27-125">このリソースのコピー元の割り当てへのポインター。</span><span class="sxs-lookup"><span data-stu-id="c9a27-125">Pointer to the assignment from which this resource was copied.</span></span> <span data-ttu-id="c9a27-126">これが null の場合、受講者は、リソースをアップロードします。</span><span class="sxs-lookup"><span data-stu-id="c9a27-126">If this is null, the student uploaded the resource.</span></span>|
|<span data-ttu-id="c9a27-127">id</span><span class="sxs-lookup"><span data-stu-id="c9a27-127">id</span></span>|<span data-ttu-id="c9a27-128">String</span><span class="sxs-lookup"><span data-stu-id="c9a27-128">String</span></span>| <span data-ttu-id="c9a27-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c9a27-129">Read-only.</span></span>|
|<span data-ttu-id="c9a27-130">resource</span><span class="sxs-lookup"><span data-stu-id="c9a27-130">resource</span></span>|[<span data-ttu-id="c9a27-131">educationResource</span><span class="sxs-lookup"><span data-stu-id="c9a27-131">educationResource</span></span>](educationresource.md)|<span data-ttu-id="c9a27-132">リソース オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="c9a27-132">Resource object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9a27-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c9a27-133">Relationships</span></span>
<span data-ttu-id="c9a27-134">なし</span><span class="sxs-lookup"><span data-stu-id="c9a27-134">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c9a27-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c9a27-135">JSON representation</span></span>

<span data-ttu-id="c9a27-136">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c9a27-136">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationSubmissionResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->