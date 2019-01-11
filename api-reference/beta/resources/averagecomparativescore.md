---
title: " averageComparativeScore リソースの種類"
description: このリソースには、さまざまなスコープ (業界 (縦)、会社の座席のサイズというように、平均での平均値など) および (識別情報、データ、デバイス、アプリケーション、インフラストラクチャ) のコントロールの分類でさまざまなさまざまなデータが含まれています。
localization_priority: Normal
ms.openlocfilehash: c32c1349edd70e80c1bf0fb12a36bd07e06ed39f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834595"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="f847c-103">averageComparativeScore リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f847c-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="f847c-104">このリソースには、さまざまなスコープ (業界 (縦)、会社の座席のサイズというように、平均での平均値など) および (識別情報、データ、デバイス、アプリケーション、インフラストラクチャ) のコントロールの分類でさまざまなさまざまなデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f847c-104">This resource contains various different scores based by different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

|<span data-ttu-id="f847c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f847c-105">Property</span></span> |<span data-ttu-id="f847c-106">種類</span><span class="sxs-lookup"><span data-stu-id="f847c-106">Type</span></span> |<span data-ttu-id="f847c-107">説明</span><span class="sxs-lookup"><span data-stu-id="f847c-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="f847c-108">単位</span><span class="sxs-lookup"><span data-stu-id="f847c-108">basis</span></span>   |   <span data-ttu-id="f847c-109">String</span><span class="sxs-lookup"><span data-stu-id="f847c-109">String</span></span>  |   <span data-ttu-id="f847c-110">範囲の種類 (、AllTenants、合計座席数、IndustryTypes)。</span><span class="sxs-lookup"><span data-stu-id="f847c-110">Scope type (By AllTenants, TotalSeats, IndustryTypes).</span></span>  |
|   <span data-ttu-id="f847c-111">averageScore</span><span class="sxs-lookup"><span data-stu-id="f847c-111">averageScore</span></span>    |   <span data-ttu-id="f847c-112">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="f847c-112">Double</span></span>  | <span data-ttu-id="f847c-113">指定された基準内での平均スコアです。</span><span class="sxs-lookup"><span data-stu-id="f847c-113">Average score within specified basis.</span></span> |
|   <span data-ttu-id="f847c-114">deviceScore</span><span class="sxs-lookup"><span data-stu-id="f847c-114">deviceScore</span></span> |   <span data-ttu-id="f847c-115">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="f847c-115">Double</span></span>  | <span data-ttu-id="f847c-116">指定された基準内での平均スコアです。</span><span class="sxs-lookup"><span data-stu-id="f847c-116">Average score within specified basis.</span></span> |
|   <span data-ttu-id="f847c-117">dataScore</span><span class="sxs-lookup"><span data-stu-id="f847c-117">dataScore</span></span>   |   <span data-ttu-id="f847c-118">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="f847c-118">Double</span></span>  | <span data-ttu-id="f847c-119">指定された基準内での平均スコアです。</span><span class="sxs-lookup"><span data-stu-id="f847c-119">Average score within specified basis.</span></span> |
|   <span data-ttu-id="f847c-120">identityScore</span><span class="sxs-lookup"><span data-stu-id="f847c-120">identityScore</span></span>   |   <span data-ttu-id="f847c-121">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="f847c-121">Double</span></span>  | <span data-ttu-id="f847c-122">指定された基準内での平均スコアです。</span><span class="sxs-lookup"><span data-stu-id="f847c-122">Average score within specified basis.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f847c-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f847c-123">JSON representation</span></span>

<span data-ttu-id="f847c-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f847c-124">The following is a JSON representation of the resource.</span></span>

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
