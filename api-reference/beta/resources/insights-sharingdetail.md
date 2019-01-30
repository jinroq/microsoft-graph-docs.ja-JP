---
title: sharingDetail リソースの種類
description: '共有アイテムのプロパティを格納する複合型。 '
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 3fff669b2b337e9566cd41a7cd5eb5ab73a84944
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643350"
---
# <a name="sharingdetail-resource-type"></a><span data-ttu-id="5ec52-103">sharingDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5ec52-103">sharingDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ec52-104">[共有](insights-shared.md)アイテムのプロパティを格納する複合型。</span><span class="sxs-lookup"><span data-stu-id="5ec52-104">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="5ec52-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5ec52-105">JSON representation</span></span>
<span data-ttu-id="5ec52-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="5ec52-106">Here is a JSON representation of the resource</span></span>

```json
{
  "sharedDateTime": "dateTimeOffset",
  "sharingSubject": "string",
  "sharingType": "string",
  "sharedBy": "insightIdentity",
  "resourceReference": "resourceReference"
}
```

## <a name="properties"></a><span data-ttu-id="5ec52-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5ec52-107">Properties</span></span>

| <span data-ttu-id="5ec52-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5ec52-108">Property</span></span>              | <span data-ttu-id="5ec52-109">型</span><span class="sxs-lookup"><span data-stu-id="5ec52-109">Type</span></span>          | <span data-ttu-id="5ec52-110">説明</span><span class="sxs-lookup"><span data-stu-id="5ec52-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="5ec52-111">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ec52-111">sharedDateTime</span></span>        | <span data-ttu-id="5ec52-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ec52-112">DateTimeOffset</span></span>| <span data-ttu-id="5ec52-113">日付と時刻、ファイルが最後に共有します。</span><span class="sxs-lookup"><span data-stu-id="5ec52-113">The date and time the file was last shared.</span></span> <span data-ttu-id="5ec52-114">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="5ec52-114">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5ec52-115">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="5ec52-115">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="5ec52-116">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5ec52-116">Read-only.</span></span>  |
| <span data-ttu-id="5ec52-117">sharingSubject</span><span class="sxs-lookup"><span data-stu-id="5ec52-117">sharingSubject</span></span>        | <span data-ttu-id="5ec52-118">String</span><span class="sxs-lookup"><span data-stu-id="5ec52-118">String</span></span>          | <span data-ttu-id="5ec52-119">ドキュメントを共有している情報カテゴリです。</span><span class="sxs-lookup"><span data-stu-id="5ec52-119">The subject with which the document was shared.</span></span> |
| <span data-ttu-id="5ec52-120">sharingType</span><span class="sxs-lookup"><span data-stu-id="5ec52-120">sharingType</span></span>             | <span data-ttu-id="5ec52-121">String</span><span class="sxs-lookup"><span data-stu-id="5ec52-121">String</span></span>        | <span data-ttu-id="5ec52-122">方法、ドキュメントが共有されていた、「リンク」、「添付ファイル」、「グループ」、「サイト」であることができますを決定します。</span><span class="sxs-lookup"><span data-stu-id="5ec52-122">Determines the way the document was shared, can be by a "Link", "Attachment", "Group", "Site".</span></span>     |
| <span data-ttu-id="5ec52-123">sharedBy</span><span class="sxs-lookup"><span data-stu-id="5ec52-123">sharedBy</span></span>                | [<span data-ttu-id="5ec52-124">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="5ec52-124">insightIdentity</span></span>](insights-insightidentity.md)      | <span data-ttu-id="5ec52-125">ドキュメントを共有するユーザーです。</span><span class="sxs-lookup"><span data-stu-id="5ec52-125">The user who shared the document.</span></span>  |
| <span data-ttu-id="5ec52-126">sharingReference</span><span class="sxs-lookup"><span data-stu-id="5ec52-126">sharingReference</span></span>        | [<span data-ttu-id="5ec52-127">resourceReference</span><span class="sxs-lookup"><span data-stu-id="5ec52-127">resourceReference</span></span>](insights-resourcereference.md)      |  |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-sharingdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
