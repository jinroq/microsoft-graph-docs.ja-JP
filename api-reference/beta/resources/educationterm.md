---
title: educationTerm リソースの種類
description: 用語。 これは学年度の指定された部分を示します。 educationClass 内で使用します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b5cfe363922fe466eef7a7333ce81249311b4063
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527564"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="978a7-105">educationTerm リソースの種類</span><span class="sxs-lookup"><span data-stu-id="978a7-105">educationTerm resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="978a7-106">用語。</span><span class="sxs-lookup"><span data-stu-id="978a7-106">A term.</span></span> <span data-ttu-id="978a7-107">これは学年度の指定された部分を示します。</span><span class="sxs-lookup"><span data-stu-id="978a7-107">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="978a7-108">[educationClass](educationclass.md) 内で使用します。</span><span class="sxs-lookup"><span data-stu-id="978a7-108">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="978a7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="978a7-109">Properties</span></span>
| <span data-ttu-id="978a7-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="978a7-110">Property</span></span>     | <span data-ttu-id="978a7-111">型</span><span class="sxs-lookup"><span data-stu-id="978a7-111">Type</span></span>   |<span data-ttu-id="978a7-112">説明</span><span class="sxs-lookup"><span data-stu-id="978a7-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="978a7-113">displayName</span><span class="sxs-lookup"><span data-stu-id="978a7-113">displayName</span></span>| <span data-ttu-id="978a7-114">String</span><span class="sxs-lookup"><span data-stu-id="978a7-114">String</span></span>| <span data-ttu-id="978a7-115">用語の表示名。</span><span class="sxs-lookup"><span data-stu-id="978a7-115">Display name of the term.</span></span>| 
|<span data-ttu-id="978a7-116">externalId</span><span class="sxs-lookup"><span data-stu-id="978a7-116">externalId</span></span>|<span data-ttu-id="978a7-117">String</span><span class="sxs-lookup"><span data-stu-id="978a7-117">String</span></span>| <span data-ttu-id="978a7-118">同期システム内の用語の ID。</span><span class="sxs-lookup"><span data-stu-id="978a7-118">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="978a7-119">startDate</span><span class="sxs-lookup"><span data-stu-id="978a7-119">startDate</span></span>|<span data-ttu-id="978a7-120">Date</span><span class="sxs-lookup"><span data-stu-id="978a7-120">Date</span></span>|<span data-ttu-id="978a7-121">用語の開始。</span><span class="sxs-lookup"><span data-stu-id="978a7-121">Start of the term.</span></span>|
|<span data-ttu-id="978a7-122">endDate</span><span class="sxs-lookup"><span data-stu-id="978a7-122">endDate</span></span>|<span data-ttu-id="978a7-123">Date</span><span class="sxs-lookup"><span data-stu-id="978a7-123">Date</span></span>|<span data-ttu-id="978a7-124">用語の終了。</span><span class="sxs-lookup"><span data-stu-id="978a7-124">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="978a7-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="978a7-125">JSON representation</span></span>

<span data-ttu-id="978a7-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="978a7-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTerm"
}-->

```json
{
  "displayName": "String",
  "externalId": "String",
  "startDate": "Date",
  "endDate": "Date"
}
```

<!-- uuid: 4e9d671f-3068-4e09-aba2-b39e81a0e452
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationTerm resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationterm.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
