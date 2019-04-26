---
title: 種類の詳細リソースの種類
description: 使用されているアイテムのプロパティを含む複合型。 ユーザーによってリソースが最後にアクセス (表示) され、変更 (編集) された日時に関する情報。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: d8a8893f2c5fcb21e2e578eefa4cf5733782db07
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333534"
---
# <a name="usagedetails-resource-type"></a><span data-ttu-id="842bf-104">種類の詳細リソースの種類</span><span class="sxs-lookup"><span data-stu-id="842bf-104">usageDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="842bf-105">[使用され](insights-used.md)ているアイテムのプロパティを含む複合型。</span><span class="sxs-lookup"><span data-stu-id="842bf-105">Complex type containing properties of [Used](insights-used.md) items.</span></span> <span data-ttu-id="842bf-106">ユーザーによってリソースが最後にアクセス (表示) され、変更 (編集) された日時に関する情報。</span><span class="sxs-lookup"><span data-stu-id="842bf-106">Information on when the resource was last accessed (viewed) and modified (edited) by the user.</span></span>

## <a name="json-representation"></a><span data-ttu-id="842bf-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="842bf-107">JSON representation</span></span>

<span data-ttu-id="842bf-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="842bf-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.usageDetails"
}-->

```json
{
  "lastAccessedDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset"
}
```

## <a name="properties"></a><span data-ttu-id="842bf-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="842bf-109">Properties</span></span>

| <span data-ttu-id="842bf-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="842bf-110">Property</span></span>              | <span data-ttu-id="842bf-111">型</span><span class="sxs-lookup"><span data-stu-id="842bf-111">Type</span></span>          | <span data-ttu-id="842bf-112">説明</span><span class="sxs-lookup"><span data-stu-id="842bf-112">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="842bf-113">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="842bf-113">lastAccessedDateTime</span></span>                  | <span data-ttu-id="842bf-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="842bf-114">DateTimeOffset</span></span>        | <span data-ttu-id="842bf-115">リソースが最後にユーザーによってアクセスされた日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="842bf-115">The date and time the resource was last accessed by the user.</span></span> <span data-ttu-id="842bf-116">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="842bf-116">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="842bf-117">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="842bf-117">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="842bf-118">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="842bf-118">Read-only.</span></span>                      |
| <span data-ttu-id="842bf-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="842bf-119">lastModifiedDateTime</span></span>              | <span data-ttu-id="842bf-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="842bf-120">DateTimeOffset</span></span>        | <span data-ttu-id="842bf-121">ユーザーによってリソースが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="842bf-121">The date and time the resource was last modified by the user.</span></span> <span data-ttu-id="842bf-122">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="842bf-122">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="842bf-123">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="842bf-123">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="842bf-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="842bf-124">Read-only.</span></span>       |
