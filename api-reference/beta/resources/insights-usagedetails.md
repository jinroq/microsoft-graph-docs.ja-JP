---
title: usageDetails リソースの種類
description: 複合型を使用する項目のプロパティが含まれています。 リソースが最後にアクセスしたときに情報 (表示)、ユーザーが (編集) を変更します。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 04e064d5ebf8599466218722d89f46ececc5e58c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577488"
---
# <a name="usagedetails-resource-type"></a><span data-ttu-id="4eb2f-104">usageDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4eb2f-104">usageDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4eb2f-105">複合型が[使用されている](insights-used.md)アイテムのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="4eb2f-105">Complex type containing properties of [Used](insights-used.md) items.</span></span> <span data-ttu-id="4eb2f-106">リソースが最後にアクセスしたときに情報 (表示)、ユーザーが (編集) を変更します。</span><span class="sxs-lookup"><span data-stu-id="4eb2f-106">Information on when the resource was last accessed (viewed) and modified (edited) by the user.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4eb2f-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4eb2f-107">JSON representation</span></span>

<span data-ttu-id="4eb2f-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="4eb2f-108">Here is a JSON representation of the resource</span></span>
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

## <a name="properties"></a><span data-ttu-id="4eb2f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4eb2f-109">Properties</span></span>

| <span data-ttu-id="4eb2f-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4eb2f-110">Property</span></span>              | <span data-ttu-id="4eb2f-111">型</span><span class="sxs-lookup"><span data-stu-id="4eb2f-111">Type</span></span>          | <span data-ttu-id="4eb2f-112">説明</span><span class="sxs-lookup"><span data-stu-id="4eb2f-112">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="4eb2f-113">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="4eb2f-113">lastAccessedDateTime</span></span>                  | <span data-ttu-id="4eb2f-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4eb2f-114">DateTimeOffset</span></span>        | <span data-ttu-id="4eb2f-115">日付と時刻、リソースは、ユーザーが最後にアクセスしました。</span><span class="sxs-lookup"><span data-stu-id="4eb2f-115">The date and time the resource was last accessed by the user.</span></span> <span data-ttu-id="4eb2f-116">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="4eb2f-116">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4eb2f-117">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="4eb2f-117">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="4eb2f-118">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4eb2f-118">Read-only.</span></span>                      |
| <span data-ttu-id="4eb2f-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4eb2f-119">lastModifiedDateTime</span></span>              | <span data-ttu-id="4eb2f-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4eb2f-120">DateTimeOffset</span></span>        | <span data-ttu-id="4eb2f-121">日付と時刻、ユーザーによってリソースが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="4eb2f-121">The date and time the resource was last modified by the user.</span></span> <span data-ttu-id="4eb2f-122">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="4eb2f-122">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4eb2f-123">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="4eb2f-123">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="4eb2f-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4eb2f-124">Read-only.</span></span>       |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-usagedetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
