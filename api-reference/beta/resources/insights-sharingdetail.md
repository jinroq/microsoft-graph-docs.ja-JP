---
title: sharingDetail リソースの種類
description: '共有アイテムのプロパティを含む複合型。 '
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: c62fc11c668a5175e0dafa9bdf4c937fecbef798
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005717"
---
# <a name="sharingdetail-resource-type"></a><span data-ttu-id="fdd68-103">sharingDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fdd68-103">sharingDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdd68-104">[共有](insights-shared.md)アイテムのプロパティを含む複合型。</span><span class="sxs-lookup"><span data-stu-id="fdd68-104">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="fdd68-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fdd68-105">JSON representation</span></span>
<span data-ttu-id="fdd68-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="fdd68-106">Here is a JSON representation of the resource</span></span>
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

## <a name="properties"></a><span data-ttu-id="fdd68-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fdd68-107">Properties</span></span>

| <span data-ttu-id="fdd68-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fdd68-108">Property</span></span>              | <span data-ttu-id="fdd68-109">型</span><span class="sxs-lookup"><span data-stu-id="fdd68-109">Type</span></span>          | <span data-ttu-id="fdd68-110">説明</span><span class="sxs-lookup"><span data-stu-id="fdd68-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="fdd68-111">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="fdd68-111">sharedDateTime</span></span>        | <span data-ttu-id="fdd68-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdd68-112">DateTimeOffset</span></span>| <span data-ttu-id="fdd68-113">ファイルが最後に共有された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="fdd68-113">The date and time the file was last shared.</span></span> <span data-ttu-id="fdd68-114">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="fdd68-114">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fdd68-115">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="fdd68-115">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="fdd68-116">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fdd68-116">Read-only.</span></span>  |
| <span data-ttu-id="fdd68-117">sharingSubject</span><span class="sxs-lookup"><span data-stu-id="fdd68-117">sharingSubject</span></span>        | <span data-ttu-id="fdd68-118">String</span><span class="sxs-lookup"><span data-stu-id="fdd68-118">String</span></span>          | <span data-ttu-id="fdd68-119">ドキュメントが共有された件名。</span><span class="sxs-lookup"><span data-stu-id="fdd68-119">The subject with which the document was shared.</span></span> |
| <span data-ttu-id="fdd68-120">sharingType</span><span class="sxs-lookup"><span data-stu-id="fdd68-120">sharingType</span></span>             | <span data-ttu-id="fdd68-121">String</span><span class="sxs-lookup"><span data-stu-id="fdd68-121">String</span></span>        | <span data-ttu-id="fdd68-122">ドキュメントの共有方法を指定します。これは、"リンク"、"添付ファイル"、"グループ"、"Site" で指定できます。</span><span class="sxs-lookup"><span data-stu-id="fdd68-122">Determines the way the document was shared, can be by a "Link", "Attachment", "Group", "Site".</span></span>     |
| <span data-ttu-id="fdd68-123">sharedBy</span><span class="sxs-lookup"><span data-stu-id="fdd68-123">sharedBy</span></span>                | [<span data-ttu-id="fdd68-124">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="fdd68-124">insightIdentity</span></span>](insights-insightidentity.md)      | <span data-ttu-id="fdd68-125">ドキュメントを共有したユーザー。</span><span class="sxs-lookup"><span data-stu-id="fdd68-125">The user who shared the document.</span></span>  |
| <span data-ttu-id="fdd68-126">sharingReference</span><span class="sxs-lookup"><span data-stu-id="fdd68-126">sharingReference</span></span>        | [<span data-ttu-id="fdd68-127">resourceReference</span><span class="sxs-lookup"><span data-stu-id="fdd68-127">resourceReference</span></span>](insights-resourcereference.md)      |  |
