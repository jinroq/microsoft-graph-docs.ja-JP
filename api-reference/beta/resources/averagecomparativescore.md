---
title: " averageComparativeScore リソースの種類"
description: このリソースには、さまざまなスコープ (業界 (縦)、会社の座席のサイズというように、平均での平均値など) および (識別情報、データ、デバイス、アプリケーション、インフラストラクチャ) のコントロールの分類でさまざまなさまざまなデータが含まれています。
ms.openlocfilehash: 08e4ec60788b21476d8f1491ab5548c7a4ca2e01
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067776"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="fa0f2-103">averageComparativeScore リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fa0f2-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="fa0f2-104">このリソースには、さまざまなスコープ (業界 (縦)、会社の座席のサイズというように、平均での平均値など) および (識別情報、データ、デバイス、アプリケーション、インフラストラクチャ) のコントロールの分類でさまざまなさまざまなデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fa0f2-104">This resource contains various different scores based by different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

|<span data-ttu-id="fa0f2-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa0f2-105">Property</span></span> |<span data-ttu-id="fa0f2-106">型</span><span class="sxs-lookup"><span data-stu-id="fa0f2-106">Type</span></span> |<span data-ttu-id="fa0f2-107">説明</span><span class="sxs-lookup"><span data-stu-id="fa0f2-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="fa0f2-108">単位</span><span class="sxs-lookup"><span data-stu-id="fa0f2-108">basis</span></span>   |   <span data-ttu-id="fa0f2-109">String</span><span class="sxs-lookup"><span data-stu-id="fa0f2-109">String</span></span>  |   <span data-ttu-id="fa0f2-110">範囲の種類 (、AllTenants、合計座席数、IndustryTypes)。</span><span class="sxs-lookup"><span data-stu-id="fa0f2-110">Scope type (By AllTenants, TotalSeats, IndustryTypes).</span></span>  |
|   <span data-ttu-id="fa0f2-111">averageScore</span><span class="sxs-lookup"><span data-stu-id="fa0f2-111">averageScore</span></span>    |   <span data-ttu-id="fa0f2-112">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="fa0f2-112">Double</span></span>  | <span data-ttu-id="fa0f2-113">指定された基準内での平均スコアです。</span><span class="sxs-lookup"><span data-stu-id="fa0f2-113">Average score within specified basis.</span></span> |
|   <span data-ttu-id="fa0f2-114">deviceScore</span><span class="sxs-lookup"><span data-stu-id="fa0f2-114">deviceScore</span></span> |   <span data-ttu-id="fa0f2-115">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="fa0f2-115">Double</span></span>  | <span data-ttu-id="fa0f2-116">指定された基準内での平均スコアです。</span><span class="sxs-lookup"><span data-stu-id="fa0f2-116">Average score within specified basis.</span></span> |
|   <span data-ttu-id="fa0f2-117">dataScore</span><span class="sxs-lookup"><span data-stu-id="fa0f2-117">dataScore</span></span>   |   <span data-ttu-id="fa0f2-118">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="fa0f2-118">Double</span></span>  | <span data-ttu-id="fa0f2-119">指定された基準内での平均スコアです。</span><span class="sxs-lookup"><span data-stu-id="fa0f2-119">Average score within specified basis.</span></span> |
|   <span data-ttu-id="fa0f2-120">identityScore</span><span class="sxs-lookup"><span data-stu-id="fa0f2-120">identityScore</span></span>   |   <span data-ttu-id="fa0f2-121">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="fa0f2-121">Double</span></span>  | <span data-ttu-id="fa0f2-122">指定された基準内での平均スコアです。</span><span class="sxs-lookup"><span data-stu-id="fa0f2-122">Average score within specified basis.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fa0f2-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fa0f2-123">JSON representation</span></span>

<span data-ttu-id="fa0f2-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fa0f2-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.averageComparativeScore"
}-->

```json
{
  "basis": "String",
  "averageScore": "Double",
  "deviceScore": "Double",
  "dataScore": "Double",
  "identityScore": "Double"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "averageComparativeScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
