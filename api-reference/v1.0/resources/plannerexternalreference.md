---
title: plannerExternalReference リソースの種類
description: '**PlannerExternalReference**リソース (ファイル、URL などの添付ファイル) の参照のメタデータを表します。 ExternalReferences オブジェクトのプロパティと値のペアの値です。'
ms.openlocfilehash: a9d53b487fd2ca6584af934c55388ee66b2071d2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020606"
---
# <a name="plannerexternalreference-resource-type"></a><span data-ttu-id="c1f47-104">plannerExternalReference リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c1f47-104">plannerExternalReference resource type</span></span>

<span data-ttu-id="c1f47-p102">**plannerExternalReference** リソースは、参照 (ファイル、URL などの添付ファイル) のメタデータを表します。[externalReferences オブジェクト](plannerexternalreferences.md)のプロパティ/値の組の値です。</span><span class="sxs-lookup"><span data-stu-id="c1f47-p102">The **plannerExternalReference** resource represents the metadata of a reference (attachments such as file, URL). It is the value of property-value pairs in the [externalReferences object](plannerexternalreferences.md).</span></span>



## <a name="properties"></a><span data-ttu-id="c1f47-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1f47-107">Properties</span></span>
| <span data-ttu-id="c1f47-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1f47-108">Property</span></span>     | <span data-ttu-id="c1f47-109">型</span><span class="sxs-lookup"><span data-stu-id="c1f47-109">Type</span></span>   |<span data-ttu-id="c1f47-110">説明</span><span class="sxs-lookup"><span data-stu-id="c1f47-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1f47-111">alias</span><span class="sxs-lookup"><span data-stu-id="c1f47-111">alias</span></span>|<span data-ttu-id="c1f47-112">String</span><span class="sxs-lookup"><span data-stu-id="c1f47-112">String</span></span>|<span data-ttu-id="c1f47-113">参照を記述するエイリアス名。</span><span class="sxs-lookup"><span data-stu-id="c1f47-113">A name alias to describe the reference.</span></span>|
|<span data-ttu-id="c1f47-114">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="c1f47-114">lastModifiedBy</span></span>|[<span data-ttu-id="c1f47-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="c1f47-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="c1f47-p103">読み取り専用です。これを最後に変更したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="c1f47-p103">Read-only. User ID by which this is last modified.</span></span>|
|<span data-ttu-id="c1f47-118">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1f47-118">lastModifiedDateTime</span></span>|<span data-ttu-id="c1f47-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1f47-119">DateTimeOffset</span></span>|<span data-ttu-id="c1f47-p104">読み取り専用です。これを最後に変更した日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c1f47-p104">Read-only. Date and time at which this is last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c1f47-124">previewPriority</span><span class="sxs-lookup"><span data-stu-id="c1f47-124">previewPriority</span></span>|<span data-ttu-id="c1f47-125">String</span><span class="sxs-lookup"><span data-stu-id="c1f47-125">String</span></span>|<span data-ttu-id="c1f47-126">タスクのプレビューとして参照が表示される、相対的な優先順位を設定するのに使用されます。</span><span class="sxs-lookup"><span data-stu-id="c1f47-126">Used to set the relative priority order in which the reference will be shown as a preview on the task.</span></span>|
|<span data-ttu-id="c1f47-127">type</span><span class="sxs-lookup"><span data-stu-id="c1f47-127">type</span></span>|<span data-ttu-id="c1f47-128">String</span><span class="sxs-lookup"><span data-stu-id="c1f47-128">String</span></span>|<span data-ttu-id="c1f47-p105">参照の種類を記述するのに使用されます。次の種類が含まれます: `PowerPoint`、`Word`、`Excel`、`Other`。</span><span class="sxs-lookup"><span data-stu-id="c1f47-p105">Used to describe the type of the reference. Types include: `PowerPoint`, `Word`, `Excel`, `Other`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c1f47-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c1f47-131">JSON representation</span></span>
<span data-ttu-id="c1f47-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c1f47-132">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerExternalReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->