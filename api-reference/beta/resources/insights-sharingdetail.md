---
title: sharingdetail リソースの種類
description: '共有アイテムのプロパティを含む複合型。 '
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 4a2dc75ed2a62d7a67538bdef801bd97133fbd15
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333565"
---
# <a name="sharingdetail-resource-type"></a><span data-ttu-id="1d3ea-103">sharingdetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1d3ea-103">sharingDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d3ea-104">[共有](insights-shared.md)アイテムのプロパティを含む複合型。</span><span class="sxs-lookup"><span data-stu-id="1d3ea-104">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="1d3ea-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1d3ea-105">JSON representation</span></span>
<span data-ttu-id="1d3ea-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="1d3ea-106">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sharingDetail"
}-->
```json
{
  "sharedDateTime": "dateTimeOffset",
  "sharingSubject": "string",
  "sharingType": "string",
  "sharedBy": "insightIdentity",
  "resourceReference": "resourceReference"
}
```

## <a name="properties"></a><span data-ttu-id="1d3ea-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d3ea-107">Properties</span></span>

| <span data-ttu-id="1d3ea-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d3ea-108">Property</span></span>              | <span data-ttu-id="1d3ea-109">型</span><span class="sxs-lookup"><span data-stu-id="1d3ea-109">Type</span></span>          | <span data-ttu-id="1d3ea-110">説明</span><span class="sxs-lookup"><span data-stu-id="1d3ea-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="1d3ea-111">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d3ea-111">sharedDateTime</span></span>        | <span data-ttu-id="1d3ea-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d3ea-112">DateTimeOffset</span></span>| <span data-ttu-id="1d3ea-113">ファイルが最後に共有された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="1d3ea-113">The date and time the file was last shared.</span></span> <span data-ttu-id="1d3ea-114">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="1d3ea-114">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1d3ea-115">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="1d3ea-115">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="1d3ea-116">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1d3ea-116">Read-only.</span></span>  |
| <span data-ttu-id="1d3ea-117">sharingsubject</span><span class="sxs-lookup"><span data-stu-id="1d3ea-117">sharingSubject</span></span>        | <span data-ttu-id="1d3ea-118">String</span><span class="sxs-lookup"><span data-stu-id="1d3ea-118">String</span></span>          | <span data-ttu-id="1d3ea-119">ドキュメントが共有された件名。</span><span class="sxs-lookup"><span data-stu-id="1d3ea-119">The subject with which the document was shared.</span></span> |
| <span data-ttu-id="1d3ea-120">sharingtype</span><span class="sxs-lookup"><span data-stu-id="1d3ea-120">sharingType</span></span>             | <span data-ttu-id="1d3ea-121">String</span><span class="sxs-lookup"><span data-stu-id="1d3ea-121">String</span></span>        | <span data-ttu-id="1d3ea-122">ドキュメントの共有方法を指定します。これは、"リンク"、"添付ファイル"、"グループ"、"Site" で指定できます。</span><span class="sxs-lookup"><span data-stu-id="1d3ea-122">Determines the way the document was shared, can be by a "Link", "Attachment", "Group", "Site".</span></span>     |
| <span data-ttu-id="1d3ea-123">sharedBy</span><span class="sxs-lookup"><span data-stu-id="1d3ea-123">sharedBy</span></span>                | [<span data-ttu-id="1d3ea-124">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="1d3ea-124">insightIdentity</span></span>](insights-insightidentity.md)      | <span data-ttu-id="1d3ea-125">ドキュメントを共有したユーザー。</span><span class="sxs-lookup"><span data-stu-id="1d3ea-125">The user who shared the document.</span></span>  |
| <span data-ttu-id="1d3ea-126">sharingreference</span><span class="sxs-lookup"><span data-stu-id="1d3ea-126">sharingReference</span></span>        | [<span data-ttu-id="1d3ea-127">resourceReference</span><span class="sxs-lookup"><span data-stu-id="1d3ea-127">resourceReference</span></span>](insights-resourcereference.md)      |  |
