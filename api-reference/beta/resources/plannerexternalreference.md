---
title: plannerExternalReference リソースの種類
description: '**PlannerExternalReference**リソース (ファイル、URL などの添付ファイル) の参照のメタデータを表します。 ExternalReferences オブジェクトのプロパティと値のペアの値です。'
ms.openlocfilehash: ad892b5e9f9a741e7a4994c509ac704ad1ca62a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067401"
---
# <a name="plannerexternalreference-resource-type"></a><span data-ttu-id="a7a61-104">plannerExternalReference リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a7a61-104">plannerExternalReference resource type</span></span>

> <span data-ttu-id="a7a61-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a7a61-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7a61-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7a61-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a7a61-p103">**plannerExternalReference** リソースは、参照 (ファイル、URL などの添付ファイル) のメタデータを表します。[externalReferences オブジェクト](plannerexternalreferences.md)のプロパティ/値の組の値です。</span><span class="sxs-lookup"><span data-stu-id="a7a61-p103">The **plannerExternalReference** resource represents the metadata of a reference (attachments such as file, URL). It is the value of property-value pairs in the [externalReferences object](plannerexternalreferences.md).</span></span>



## <a name="properties"></a><span data-ttu-id="a7a61-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7a61-109">Properties</span></span>
| <span data-ttu-id="a7a61-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7a61-110">Property</span></span>     | <span data-ttu-id="a7a61-111">型</span><span class="sxs-lookup"><span data-stu-id="a7a61-111">Type</span></span>   |<span data-ttu-id="a7a61-112">説明</span><span class="sxs-lookup"><span data-stu-id="a7a61-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a7a61-113">alias</span><span class="sxs-lookup"><span data-stu-id="a7a61-113">alias</span></span>|<span data-ttu-id="a7a61-114">String</span><span class="sxs-lookup"><span data-stu-id="a7a61-114">String</span></span>|<span data-ttu-id="a7a61-115">参照を記述するエイリアス名。</span><span class="sxs-lookup"><span data-stu-id="a7a61-115">A name alias to describe the reference.</span></span>|
|<span data-ttu-id="a7a61-116">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="a7a61-116">lastModifiedBy</span></span>|[<span data-ttu-id="a7a61-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="a7a61-117">identitySet</span></span>](identityset.md)|<span data-ttu-id="a7a61-p104">読み取り専用です。これを最後に変更したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="a7a61-p104">Read-only. User ID by which this is last modified.</span></span>|
|<span data-ttu-id="a7a61-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7a61-120">lastModifiedDateTime</span></span>|<span data-ttu-id="a7a61-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7a61-121">DateTimeOffset</span></span>|<span data-ttu-id="a7a61-p105">読み取り専用です。これを最後に変更した日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a7a61-p105">Read-only. Date and time at which this is last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a7a61-126">previewPriority</span><span class="sxs-lookup"><span data-stu-id="a7a61-126">previewPriority</span></span>|<span data-ttu-id="a7a61-127">String</span><span class="sxs-lookup"><span data-stu-id="a7a61-127">String</span></span>|<span data-ttu-id="a7a61-128">タスクのプレビューとして参照が表示される、相対的な優先順位を設定するのに使用されます。</span><span class="sxs-lookup"><span data-stu-id="a7a61-128">Used to set the relative priority order in which the reference will be shown as a preview on the task.</span></span>|
|<span data-ttu-id="a7a61-129">type</span><span class="sxs-lookup"><span data-stu-id="a7a61-129">type</span></span>|<span data-ttu-id="a7a61-130">String</span><span class="sxs-lookup"><span data-stu-id="a7a61-130">String</span></span>|<span data-ttu-id="a7a61-p106">参照の種類を記述するのに使用されます。次の種類が含まれます: `PowerPoint`、`Word`、`Excel`、`Other`。</span><span class="sxs-lookup"><span data-stu-id="a7a61-p106">Used to describe the type of the reference. Types include: `PowerPoint`, `Word`, `Excel`, `Other`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a7a61-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a7a61-133">JSON representation</span></span>
<span data-ttu-id="a7a61-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a7a61-134">Here is a JSON representation of the resource.</span></span>

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