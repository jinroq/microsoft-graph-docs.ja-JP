---
title: educationTerm リソースの種類
description: 用語。 これは学年度の指定された部分を示します。 educationClass 内で使用します。
author: mmast-msft
ms.openlocfilehash: 31925f336dbb0ce0f83ffd6b36b38e7a0916cdb5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303452"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="af8e9-105">educationTerm リソースの種類</span><span class="sxs-lookup"><span data-stu-id="af8e9-105">educationTerm resource type</span></span>

> <span data-ttu-id="af8e9-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="af8e9-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="af8e9-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af8e9-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="af8e9-108">用語。</span><span class="sxs-lookup"><span data-stu-id="af8e9-108">A term.</span></span> <span data-ttu-id="af8e9-109">これは学年度の指定された部分を示します。</span><span class="sxs-lookup"><span data-stu-id="af8e9-109">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="af8e9-110">[educationClass](educationclass.md) 内で使用します。</span><span class="sxs-lookup"><span data-stu-id="af8e9-110">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="af8e9-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="af8e9-111">Properties</span></span>
| <span data-ttu-id="af8e9-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="af8e9-112">Property</span></span>     | <span data-ttu-id="af8e9-113">種類</span><span class="sxs-lookup"><span data-stu-id="af8e9-113">Type</span></span>   |<span data-ttu-id="af8e9-114">説明</span><span class="sxs-lookup"><span data-stu-id="af8e9-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af8e9-115">displayName</span><span class="sxs-lookup"><span data-stu-id="af8e9-115">displayName</span></span>| <span data-ttu-id="af8e9-116">String</span><span class="sxs-lookup"><span data-stu-id="af8e9-116">String</span></span>| <span data-ttu-id="af8e9-117">用語の表示名。</span><span class="sxs-lookup"><span data-stu-id="af8e9-117">Display name of the term.</span></span>| 
|<span data-ttu-id="af8e9-118">externalId</span><span class="sxs-lookup"><span data-stu-id="af8e9-118">externalId</span></span>|<span data-ttu-id="af8e9-119">String</span><span class="sxs-lookup"><span data-stu-id="af8e9-119">String</span></span>| <span data-ttu-id="af8e9-120">同期システム内の用語の ID。</span><span class="sxs-lookup"><span data-stu-id="af8e9-120">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="af8e9-121">startDate</span><span class="sxs-lookup"><span data-stu-id="af8e9-121">startDate</span></span>|<span data-ttu-id="af8e9-122">Date</span><span class="sxs-lookup"><span data-stu-id="af8e9-122">Date</span></span>|<span data-ttu-id="af8e9-123">用語の開始。</span><span class="sxs-lookup"><span data-stu-id="af8e9-123">Start of the term.</span></span>|
|<span data-ttu-id="af8e9-124">endDate</span><span class="sxs-lookup"><span data-stu-id="af8e9-124">endDate</span></span>|<span data-ttu-id="af8e9-125">Date</span><span class="sxs-lookup"><span data-stu-id="af8e9-125">Date</span></span>|<span data-ttu-id="af8e9-126">用語の終了。</span><span class="sxs-lookup"><span data-stu-id="af8e9-126">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="af8e9-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="af8e9-127">JSON representation</span></span>

<span data-ttu-id="af8e9-128">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="af8e9-128">The following is a JSON representation of the resource.</span></span>

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