---
title: プラン/外部参照リソースの種類
description: '**plan/externalreference**リソースは、参照 (ファイル、URL などの添付ファイル) のメタデータを表します。 これは、externalreferences オブジェクトのプロパティと値のペアの値です。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 6d2bce70afbeee3848f3055530daf732afe8a2b5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344824"
---
# <a name="plannerexternalreference-resource-type"></a><span data-ttu-id="5bd47-104">プラン/外部参照リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5bd47-104">plannerExternalReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bd47-105">**plan/externalreference**リソースは、参照 (ファイル、URL などの添付ファイル) のメタデータを表します。</span><span class="sxs-lookup"><span data-stu-id="5bd47-105">The **plannerExternalReference** resource represents the metadata of a reference (attachments such as file, URL).</span></span> <span data-ttu-id="5bd47-106">これは、 [externalreferences オブジェクト](plannerexternalreferences.md)のプロパティと値のペアの値です。</span><span class="sxs-lookup"><span data-stu-id="5bd47-106">It is the value of property-value pairs in the [externalReferences object](plannerexternalreferences.md).</span></span>



## <a name="properties"></a><span data-ttu-id="5bd47-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5bd47-107">Properties</span></span>
| <span data-ttu-id="5bd47-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5bd47-108">Property</span></span>     | <span data-ttu-id="5bd47-109">型</span><span class="sxs-lookup"><span data-stu-id="5bd47-109">Type</span></span>   |<span data-ttu-id="5bd47-110">説明</span><span class="sxs-lookup"><span data-stu-id="5bd47-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5bd47-111">alias</span><span class="sxs-lookup"><span data-stu-id="5bd47-111">alias</span></span>|<span data-ttu-id="5bd47-112">String</span><span class="sxs-lookup"><span data-stu-id="5bd47-112">String</span></span>|<span data-ttu-id="5bd47-113">参照を記述する名前のエイリアス。</span><span class="sxs-lookup"><span data-stu-id="5bd47-113">A name alias to describe the reference.</span></span>|
|<span data-ttu-id="5bd47-114">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="5bd47-114">lastModifiedBy</span></span>|[<span data-ttu-id="5bd47-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="5bd47-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="5bd47-116">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5bd47-116">Read-only.</span></span> <span data-ttu-id="5bd47-117">これを最後に変更するユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="5bd47-117">User ID by which this is last modified.</span></span>|
|<span data-ttu-id="5bd47-118">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5bd47-118">lastModifiedDateTime</span></span>|<span data-ttu-id="5bd47-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bd47-119">DateTimeOffset</span></span>|<span data-ttu-id="5bd47-120">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="5bd47-120">Read-only.</span></span> <span data-ttu-id="5bd47-121">この時刻が最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="5bd47-121">Date and time at which this is last modified.</span></span> <span data-ttu-id="5bd47-122">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="5bd47-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5bd47-123">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5bd47-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5bd47-124">プレビューの優先度</span><span class="sxs-lookup"><span data-stu-id="5bd47-124">previewPriority</span></span>|<span data-ttu-id="5bd47-125">String</span><span class="sxs-lookup"><span data-stu-id="5bd47-125">String</span></span>|<span data-ttu-id="5bd47-126">タスクのプレビューとして参照が表示される相対的な優先順位を設定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="5bd47-126">Used to set the relative priority order in which the reference will be shown as a preview on the task.</span></span>|
|<span data-ttu-id="5bd47-127">type</span><span class="sxs-lookup"><span data-stu-id="5bd47-127">type</span></span>|<span data-ttu-id="5bd47-128">String</span><span class="sxs-lookup"><span data-stu-id="5bd47-128">String</span></span>|<span data-ttu-id="5bd47-129">参照の種類を記述するために使用します。</span><span class="sxs-lookup"><span data-stu-id="5bd47-129">Used to describe the type of the reference.</span></span> <span data-ttu-id="5bd47-130">種類は`PowerPoint`、、 `Word`、 `Excel`、 `Other`です。</span><span class="sxs-lookup"><span data-stu-id="5bd47-130">Types include: `PowerPoint`, `Word`, `Excel`, `Other`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5bd47-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5bd47-131">JSON representation</span></span>
<span data-ttu-id="5bd47-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5bd47-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerExternalReference"
}-->

```json
{
  "alias": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "previewPriority": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerExternalReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
