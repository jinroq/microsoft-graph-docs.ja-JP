---
title: 種類の詳細リソースの種類
description: 使用されているアイテムのプロパティを含む複合型。 ユーザーによってリソースが最後にアクセス (表示) され、変更 (編集) された日時に関する情報。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 4df15bf635785aba054d52beb89b5ac04d48d3d3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551296"
---
# <a name="usagedetails-resource-type"></a><span data-ttu-id="34f0e-104">種類の詳細リソースの種類</span><span class="sxs-lookup"><span data-stu-id="34f0e-104">usageDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34f0e-105">[使用され](insights-used.md)ているアイテムのプロパティを含む複合型。</span><span class="sxs-lookup"><span data-stu-id="34f0e-105">Complex type containing properties of [Used](insights-used.md) items.</span></span> <span data-ttu-id="34f0e-106">ユーザーによってリソースが最後にアクセス (表示) され、変更 (編集) された日時に関する情報。</span><span class="sxs-lookup"><span data-stu-id="34f0e-106">Information on when the resource was last accessed (viewed) and modified (edited) by the user.</span></span>

## <a name="json-representation"></a><span data-ttu-id="34f0e-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="34f0e-107">JSON representation</span></span>

<span data-ttu-id="34f0e-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="34f0e-108">Here is a JSON representation of the resource</span></span>

```json
{
  "lastAccessedDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset"
}
```

## <a name="properties"></a><span data-ttu-id="34f0e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34f0e-109">Properties</span></span>

| <span data-ttu-id="34f0e-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34f0e-110">Property</span></span>              | <span data-ttu-id="34f0e-111">型</span><span class="sxs-lookup"><span data-stu-id="34f0e-111">Type</span></span>          | <span data-ttu-id="34f0e-112">説明</span><span class="sxs-lookup"><span data-stu-id="34f0e-112">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="34f0e-113">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="34f0e-113">lastAccessedDateTime</span></span>                  | <span data-ttu-id="34f0e-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34f0e-114">DateTimeOffset</span></span>        | <span data-ttu-id="34f0e-115">リソースが最後にユーザーによってアクセスされた日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="34f0e-115">The date and time the resource was last accessed by the user.</span></span> <span data-ttu-id="34f0e-116">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="34f0e-116">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="34f0e-117">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="34f0e-117">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="34f0e-118">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="34f0e-118">Read-only.</span></span>                      |
| <span data-ttu-id="34f0e-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34f0e-119">lastModifiedDateTime</span></span>              | <span data-ttu-id="34f0e-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34f0e-120">DateTimeOffset</span></span>        | <span data-ttu-id="34f0e-121">ユーザーによってリソースが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="34f0e-121">The date and time the resource was last modified by the user.</span></span> <span data-ttu-id="34f0e-122">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="34f0e-122">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="34f0e-123">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="34f0e-123">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="34f0e-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="34f0e-124">Read-only.</span></span>       |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-usagedetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
