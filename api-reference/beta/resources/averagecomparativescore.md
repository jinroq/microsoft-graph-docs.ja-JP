---
title: " averageComparativeScore リソースの種類"
description: このリソースには、さまざまな範囲 (たとえば、業種別の平均、企業の座席サイズ別の平均)、コントロールカテゴリ (Id、データ、デバイス、アプリ、インフラストラクチャ) に基づいて、さまざまなスコアが含まれています。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3e2256e7edefd0670bb697ec6d89c9fb80a5beeb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013151"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="fe0df-103">averageComparativeScore リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fe0df-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="fe0df-104">このリソースには、さまざまな範囲 (たとえば、業種別の平均、企業の座席サイズ別の平均)、コントロールカテゴリ (Id、データ、デバイス、アプリ、インフラストラクチャ) に基づいて、さまざまなスコアが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fe0df-104">This resource contains various different scores based by different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

|<span data-ttu-id="fe0df-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe0df-105">Property</span></span> |<span data-ttu-id="fe0df-106">型</span><span class="sxs-lookup"><span data-stu-id="fe0df-106">Type</span></span> |<span data-ttu-id="fe0df-107">説明</span><span class="sxs-lookup"><span data-stu-id="fe0df-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="fe0df-108">だけ</span><span class="sxs-lookup"><span data-stu-id="fe0df-108">basis</span></span>   |   <span data-ttu-id="fe0df-109">String</span><span class="sxs-lookup"><span data-stu-id="fe0df-109">String</span></span>  |   <span data-ttu-id="fe0df-110">範囲の種類 (AllTenants、TotalSeats、IndustryTypes)。</span><span class="sxs-lookup"><span data-stu-id="fe0df-110">Scope type (By AllTenants, TotalSeats, IndustryTypes).</span></span>  |
|   <span data-ttu-id="fe0df-111">averageScore</span><span class="sxs-lookup"><span data-stu-id="fe0df-111">averageScore</span></span>    |   <span data-ttu-id="fe0df-112">2 行分</span><span class="sxs-lookup"><span data-stu-id="fe0df-112">Double</span></span>  | <span data-ttu-id="fe0df-113">指定された基準内の平均スコア。</span><span class="sxs-lookup"><span data-stu-id="fe0df-113">Average score within specified basis.</span></span> |
|   <span data-ttu-id="fe0df-114">デバイスコア</span><span class="sxs-lookup"><span data-stu-id="fe0df-114">deviceScore</span></span> |   <span data-ttu-id="fe0df-115">2 行分</span><span class="sxs-lookup"><span data-stu-id="fe0df-115">Double</span></span>  | <span data-ttu-id="fe0df-116">指定された基準内の平均スコア。</span><span class="sxs-lookup"><span data-stu-id="fe0df-116">Average score within specified basis.</span></span> |
|   <span data-ttu-id="fe0df-117">dataScore</span><span class="sxs-lookup"><span data-stu-id="fe0df-117">dataScore</span></span>   |   <span data-ttu-id="fe0df-118">2 行分</span><span class="sxs-lookup"><span data-stu-id="fe0df-118">Double</span></span>  | <span data-ttu-id="fe0df-119">指定された基準内の平均スコア。</span><span class="sxs-lookup"><span data-stu-id="fe0df-119">Average score within specified basis.</span></span> |
|   <span data-ttu-id="fe0df-120">「Id」</span><span class="sxs-lookup"><span data-stu-id="fe0df-120">identityScore</span></span>   |   <span data-ttu-id="fe0df-121">2 行分</span><span class="sxs-lookup"><span data-stu-id="fe0df-121">Double</span></span>  | <span data-ttu-id="fe0df-122">指定された基準内の平均スコア。</span><span class="sxs-lookup"><span data-stu-id="fe0df-122">Average score within specified basis.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fe0df-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fe0df-123">JSON representation</span></span>

<span data-ttu-id="fe0df-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fe0df-124">The following is a JSON representation of the resource.</span></span>

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
