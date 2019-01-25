---
title: rankedEmailAddress リソースの種類
description: ランクの電子メール アドレスを表します。
localization_priority: Normal
ms.openlocfilehash: 938afc0de208fd3cdbd0cfec299d01ada9d4f592
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510009"
---
# <a name="rankedemailaddress-resource-type"></a><span data-ttu-id="176d4-103">rankedEmailAddress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="176d4-103">rankedEmailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="176d4-104">ランクの電子メール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="176d4-104">Represents a ranked email address.</span></span>


## <a name="properties"></a><span data-ttu-id="176d4-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="176d4-105">Properties</span></span>
| <span data-ttu-id="176d4-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="176d4-106">Property</span></span>     | <span data-ttu-id="176d4-107">型</span><span class="sxs-lookup"><span data-stu-id="176d4-107">Type</span></span>   |<span data-ttu-id="176d4-108">説明</span><span class="sxs-lookup"><span data-stu-id="176d4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="176d4-109">address</span><span class="sxs-lookup"><span data-stu-id="176d4-109">address</span></span>|<span data-ttu-id="176d4-110">string</span><span class="sxs-lookup"><span data-stu-id="176d4-110">string</span></span>|<span data-ttu-id="176d4-111">電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="176d4-111">The email address.</span></span>|
|<span data-ttu-id="176d4-112">rank</span><span class="sxs-lookup"><span data-stu-id="176d4-112">rank</span></span>|<span data-ttu-id="176d4-113">double</span><span class="sxs-lookup"><span data-stu-id="176d4-113">double</span></span>|<span data-ttu-id="176d4-114">電子メール アドレスのランキングです。</span><span class="sxs-lookup"><span data-stu-id="176d4-114">The rank of the email address.</span></span> <span data-ttu-id="176d4-115">ランクは、他の返される結果に関連して、並べ替えキーとして使用されます。</span><span class="sxs-lookup"><span data-stu-id="176d4-115">A rank is used as a sort key, in relation to the other returned results.</span></span> <span data-ttu-id="176d4-116">上位の値は、関連性の高い結果に対応します。</span><span class="sxs-lookup"><span data-stu-id="176d4-116">A higher rank value corresponds to a more relevant result.</span></span> <span data-ttu-id="176d4-117">関連性は、通信、コラボレーション、取引関係のシグナルによって決定されます。</span><span class="sxs-lookup"><span data-stu-id="176d4-117">Relevance is determined by communication, collaboration, and business relationship signals.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="176d4-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="176d4-118">JSON representation</span></span>

<span data-ttu-id="176d4-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="176d4-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rankedEmailAddress"
}-->

```json
{
  "address": "string",
  "rank": 1024
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "rankedEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/rankedemailaddress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
