---
title: educationTerm リソースの種類
description: 用語。 これは学年度の指定された部分を示します。 educationClass 内で使用します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 36426a7e3f1fb79264a788d8af7e7768f5bae26a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032621"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="01522-105">educationTerm リソースの種類</span><span class="sxs-lookup"><span data-stu-id="01522-105">educationTerm resource type</span></span>

<span data-ttu-id="01522-106">用語。</span><span class="sxs-lookup"><span data-stu-id="01522-106">A term.</span></span> <span data-ttu-id="01522-107">これは学年度の指定された部分を示します。</span><span class="sxs-lookup"><span data-stu-id="01522-107">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="01522-108">[educationClass](educationclass.md) 内で使用します。</span><span class="sxs-lookup"><span data-stu-id="01522-108">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="01522-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="01522-109">Properties</span></span>
| <span data-ttu-id="01522-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="01522-110">Property</span></span>     | <span data-ttu-id="01522-111">型</span><span class="sxs-lookup"><span data-stu-id="01522-111">Type</span></span>   |<span data-ttu-id="01522-112">説明</span><span class="sxs-lookup"><span data-stu-id="01522-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01522-113">displayName</span><span class="sxs-lookup"><span data-stu-id="01522-113">displayName</span></span>| <span data-ttu-id="01522-114">String</span><span class="sxs-lookup"><span data-stu-id="01522-114">String</span></span>| <span data-ttu-id="01522-115">用語の表示名。</span><span class="sxs-lookup"><span data-stu-id="01522-115">Display name of the term.</span></span>| 
|<span data-ttu-id="01522-116">externalId</span><span class="sxs-lookup"><span data-stu-id="01522-116">externalId</span></span>|<span data-ttu-id="01522-117">String</span><span class="sxs-lookup"><span data-stu-id="01522-117">String</span></span>| <span data-ttu-id="01522-118">同期システム内の用語の ID。</span><span class="sxs-lookup"><span data-stu-id="01522-118">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="01522-119">startDate</span><span class="sxs-lookup"><span data-stu-id="01522-119">startDate</span></span>|<span data-ttu-id="01522-120">Date</span><span class="sxs-lookup"><span data-stu-id="01522-120">Date</span></span>|<span data-ttu-id="01522-121">用語の開始。</span><span class="sxs-lookup"><span data-stu-id="01522-121">Start of the term.</span></span>|
|<span data-ttu-id="01522-122">endDate</span><span class="sxs-lookup"><span data-stu-id="01522-122">endDate</span></span>|<span data-ttu-id="01522-123">Date</span><span class="sxs-lookup"><span data-stu-id="01522-123">Date</span></span>|<span data-ttu-id="01522-124">用語の終了。</span><span class="sxs-lookup"><span data-stu-id="01522-124">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="01522-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="01522-125">JSON representation</span></span>

<span data-ttu-id="01522-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="01522-126">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationTerm resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
