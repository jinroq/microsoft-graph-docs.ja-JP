---
title: rankedemailaddress リソースの種類
description: ランク付けされた電子メールアドレスを表します。
localization_priority: Normal
ms.openlocfilehash: 938afc0de208fd3cdbd0cfec299d01ada9d4f592
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563272"
---
# <a name="rankedemailaddress-resource-type"></a><span data-ttu-id="a654f-103">rankedemailaddress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a654f-103">rankedEmailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a654f-104">ランク付けされた電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="a654f-104">Represents a ranked email address.</span></span>


## <a name="properties"></a><span data-ttu-id="a654f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a654f-105">Properties</span></span>
| <span data-ttu-id="a654f-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a654f-106">Property</span></span>     | <span data-ttu-id="a654f-107">型</span><span class="sxs-lookup"><span data-stu-id="a654f-107">Type</span></span>   |<span data-ttu-id="a654f-108">説明</span><span class="sxs-lookup"><span data-stu-id="a654f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a654f-109">address</span><span class="sxs-lookup"><span data-stu-id="a654f-109">address</span></span>|<span data-ttu-id="a654f-110">string</span><span class="sxs-lookup"><span data-stu-id="a654f-110">string</span></span>|<span data-ttu-id="a654f-111">電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="a654f-111">The email address.</span></span>|
|<span data-ttu-id="a654f-112">rank</span><span class="sxs-lookup"><span data-stu-id="a654f-112">rank</span></span>|<span data-ttu-id="a654f-113">double</span><span class="sxs-lookup"><span data-stu-id="a654f-113">double</span></span>|<span data-ttu-id="a654f-114">電子メールアドレスのランク。</span><span class="sxs-lookup"><span data-stu-id="a654f-114">The rank of the email address.</span></span> <span data-ttu-id="a654f-115">ランクは、他の返された結果に対して並べ替えキーとして使用されます。</span><span class="sxs-lookup"><span data-stu-id="a654f-115">A rank is used as a sort key, in relation to the other returned results.</span></span> <span data-ttu-id="a654f-116">上位の値は、関連性の高い結果に対応します。</span><span class="sxs-lookup"><span data-stu-id="a654f-116">A higher rank value corresponds to a more relevant result.</span></span> <span data-ttu-id="a654f-117">関連性は、通信、コラボレーション、取引関係のシグナルによって決定されます。</span><span class="sxs-lookup"><span data-stu-id="a654f-117">Relevance is determined by communication, collaboration, and business relationship signals.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a654f-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a654f-118">JSON representation</span></span>

<span data-ttu-id="a654f-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a654f-119">Here is a JSON representation of the resource.</span></span>

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
