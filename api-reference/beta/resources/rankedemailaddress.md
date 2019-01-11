---
title: rankedEmailAddress リソースの種類
description: ランクの電子メール アドレスを表します。
localization_priority: Normal
ms.openlocfilehash: bb3b906929bddcb52a57a478647000e7e16fa0be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818516"
---
# <a name="rankedemailaddress-resource-type"></a><span data-ttu-id="ccf20-103">rankedEmailAddress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ccf20-103">rankedEmailAddress resource type</span></span>

> <span data-ttu-id="ccf20-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ccf20-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ccf20-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ccf20-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ccf20-106">ランクの電子メール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="ccf20-106">Represents a ranked email address.</span></span>


## <a name="properties"></a><span data-ttu-id="ccf20-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ccf20-107">Properties</span></span>
| <span data-ttu-id="ccf20-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ccf20-108">Property</span></span>     | <span data-ttu-id="ccf20-109">種類</span><span class="sxs-lookup"><span data-stu-id="ccf20-109">Type</span></span>   |<span data-ttu-id="ccf20-110">説明</span><span class="sxs-lookup"><span data-stu-id="ccf20-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ccf20-111">address</span><span class="sxs-lookup"><span data-stu-id="ccf20-111">address</span></span>|<span data-ttu-id="ccf20-112">文字列</span><span class="sxs-lookup"><span data-stu-id="ccf20-112">string</span></span>|<span data-ttu-id="ccf20-113">電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="ccf20-113">The email address.</span></span>|
|<span data-ttu-id="ccf20-114">rank</span><span class="sxs-lookup"><span data-stu-id="ccf20-114">rank</span></span>|<span data-ttu-id="ccf20-115">double</span><span class="sxs-lookup"><span data-stu-id="ccf20-115">double</span></span>|<span data-ttu-id="ccf20-116">電子メール アドレスのランキングです。</span><span class="sxs-lookup"><span data-stu-id="ccf20-116">The rank of the email address.</span></span> <span data-ttu-id="ccf20-117">ランクは、他の返される結果に関連して、並べ替えキーとして使用されます。</span><span class="sxs-lookup"><span data-stu-id="ccf20-117">A rank is used as a sort key, in relation to the other returned results.</span></span> <span data-ttu-id="ccf20-118">上位の値は、関連性の高い結果に対応します。</span><span class="sxs-lookup"><span data-stu-id="ccf20-118">A higher rank value corresponds to a more relevant result.</span></span> <span data-ttu-id="ccf20-119">関連性は、通信、コラボレーション、取引関係のシグナルによって決定されます。</span><span class="sxs-lookup"><span data-stu-id="ccf20-119">Relevance is determined by communication, collaboration, and business relationship signals.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ccf20-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ccf20-120">JSON representation</span></span>

<span data-ttu-id="ccf20-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ccf20-121">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "rankedEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
