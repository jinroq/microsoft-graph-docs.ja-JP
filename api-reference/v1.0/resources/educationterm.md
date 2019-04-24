---
title: educationTerm リソースの種類
description: 用語。 これは学年度の指定された部分を示します。 educationClass 内で使用します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 9c26565b552471fe2601d8e3cb629fd933d72937
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463699"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="54f63-105">educationTerm リソースの種類</span><span class="sxs-lookup"><span data-stu-id="54f63-105">educationTerm resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54f63-106">用語。</span><span class="sxs-lookup"><span data-stu-id="54f63-106">A term.</span></span> <span data-ttu-id="54f63-107">これは学年度の指定された部分を示します。</span><span class="sxs-lookup"><span data-stu-id="54f63-107">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="54f63-108">[educationClass](educationclass.md) 内で使用します。</span><span class="sxs-lookup"><span data-stu-id="54f63-108">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="54f63-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54f63-109">Properties</span></span>
| <span data-ttu-id="54f63-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54f63-110">Property</span></span>     | <span data-ttu-id="54f63-111">型</span><span class="sxs-lookup"><span data-stu-id="54f63-111">Type</span></span>   |<span data-ttu-id="54f63-112">説明</span><span class="sxs-lookup"><span data-stu-id="54f63-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="54f63-113">displayName</span><span class="sxs-lookup"><span data-stu-id="54f63-113">displayName</span></span>| <span data-ttu-id="54f63-114">String</span><span class="sxs-lookup"><span data-stu-id="54f63-114">String</span></span>| <span data-ttu-id="54f63-115">用語の表示名。</span><span class="sxs-lookup"><span data-stu-id="54f63-115">Display name of the term.</span></span>| 
|<span data-ttu-id="54f63-116">externalId</span><span class="sxs-lookup"><span data-stu-id="54f63-116">externalId</span></span>|<span data-ttu-id="54f63-117">String</span><span class="sxs-lookup"><span data-stu-id="54f63-117">String</span></span>| <span data-ttu-id="54f63-118">同期システム内の用語の ID。</span><span class="sxs-lookup"><span data-stu-id="54f63-118">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="54f63-119">startDate</span><span class="sxs-lookup"><span data-stu-id="54f63-119">startDate</span></span>|<span data-ttu-id="54f63-120">Date</span><span class="sxs-lookup"><span data-stu-id="54f63-120">Date</span></span>|<span data-ttu-id="54f63-121">用語の開始。</span><span class="sxs-lookup"><span data-stu-id="54f63-121">Start of the term.</span></span>|
|<span data-ttu-id="54f63-122">endDate</span><span class="sxs-lookup"><span data-stu-id="54f63-122">endDate</span></span>|<span data-ttu-id="54f63-123">Date</span><span class="sxs-lookup"><span data-stu-id="54f63-123">Date</span></span>|<span data-ttu-id="54f63-124">用語の終了。</span><span class="sxs-lookup"><span data-stu-id="54f63-124">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="54f63-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="54f63-125">JSON representation</span></span>

<span data-ttu-id="54f63-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="54f63-126">The following is a JSON representation of the resource.</span></span>

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
