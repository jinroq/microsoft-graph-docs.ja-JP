---
title: scoredEmailAddress リソースの種類
description: スコアの付いたメール アドレスを表します。
ms.openlocfilehash: 9cdd33a6df9eefca0f7a00c5fe8b17832e0056d9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024282"
---
# <a name="scoredemailaddress-resource-type"></a><span data-ttu-id="ff27d-103">scoredEmailAddress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ff27d-103">scoredEmailAddress resource type</span></span>

<span data-ttu-id="ff27d-104">スコアの付いたメール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="ff27d-104">Represents a scored email address.</span></span>


## <a name="properties"></a><span data-ttu-id="ff27d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff27d-105">Properties</span></span>
| <span data-ttu-id="ff27d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff27d-106">Property</span></span>     | <span data-ttu-id="ff27d-107">型</span><span class="sxs-lookup"><span data-stu-id="ff27d-107">Type</span></span>   |<span data-ttu-id="ff27d-108">説明</span><span class="sxs-lookup"><span data-stu-id="ff27d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff27d-109">address</span><span class="sxs-lookup"><span data-stu-id="ff27d-109">address</span></span>|<span data-ttu-id="ff27d-110">文字列</span><span class="sxs-lookup"><span data-stu-id="ff27d-110">string</span></span>|<span data-ttu-id="ff27d-111">電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="ff27d-111">The email address.</span></span>|
|<span data-ttu-id="ff27d-112">relevanceScore</span><span class="sxs-lookup"><span data-stu-id="ff27d-112">relevanceScore</span></span>|<span data-ttu-id="ff27d-113">double</span><span class="sxs-lookup"><span data-stu-id="ff27d-113">double</span></span>|<span data-ttu-id="ff27d-p101">電子メール アドレスの関連性スコア。関連性スコアは他の返された結果に関連して、並べ替えキーとして使用されます。関連性スコア値が高いほど、関連性の高い結果に対応します。関連性は、ユーザーのコミュニケーションとコラボレーション パターン、およびビジネスのリレーションシップによって決定されます。</span><span class="sxs-lookup"><span data-stu-id="ff27d-p101">The relevance score of the email address. A relevance score is used as a sort key, in relation to the other returned results. A higher relevance score value corresponds to a more relevant result. Relevance is determined by the user’s communication and collaboration patterns and business relationships.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ff27d-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ff27d-118">JSON representation</span></span>

<span data-ttu-id="ff27d-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ff27d-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scoredEmailAddress"
}-->

```json
{
  "address": "string",
  "relevanceScore": 1024.0
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "scoredEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
