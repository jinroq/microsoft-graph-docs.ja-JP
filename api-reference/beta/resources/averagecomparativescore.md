---
title: " averageComparativeScore リソースの種類"
description: このリソースには、さまざまな範囲 (たとえば、業種別の平均、企業の座席サイズ別の平均)、コントロールカテゴリ (id、データ、デバイス、アプリ、インフラストラクチャ) に基づいて、さまざまなスコアが含まれています。
localization_priority: Normal
ms.openlocfilehash: c32c1349edd70e80c1bf0fb12a36bd07e06ed39f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535439"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="13bae-103">averageComparativeScore リソースの種類</span><span class="sxs-lookup"><span data-stu-id="13bae-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="13bae-104">このリソースには、さまざまな範囲 (たとえば、業種別の平均、企業の座席サイズ別の平均)、コントロールカテゴリ (id、データ、デバイス、アプリ、インフラストラクチャ) に基づいて、さまざまなスコアが含まれています。</span><span class="sxs-lookup"><span data-stu-id="13bae-104">This resource contains various different scores based by different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

|<span data-ttu-id="13bae-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13bae-105">Property</span></span> |<span data-ttu-id="13bae-106">型</span><span class="sxs-lookup"><span data-stu-id="13bae-106">Type</span></span> |<span data-ttu-id="13bae-107">説明</span><span class="sxs-lookup"><span data-stu-id="13bae-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="13bae-108">だけ</span><span class="sxs-lookup"><span data-stu-id="13bae-108">basis</span></span>   |   <span data-ttu-id="13bae-109">String</span><span class="sxs-lookup"><span data-stu-id="13bae-109">String</span></span>  |   <span data-ttu-id="13bae-110">範囲の種類 (alltenants、totalseats、IndustryTypes)。</span><span class="sxs-lookup"><span data-stu-id="13bae-110">Scope type (By AllTenants, TotalSeats, IndustryTypes).</span></span>  |
|   <span data-ttu-id="13bae-111">averageScore</span><span class="sxs-lookup"><span data-stu-id="13bae-111">averageScore</span></span>    |   <span data-ttu-id="13bae-112">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="13bae-112">Double</span></span>  | <span data-ttu-id="13bae-113">指定された基準内の平均スコア。</span><span class="sxs-lookup"><span data-stu-id="13bae-113">Average score within specified basis.</span></span> |
|   <span data-ttu-id="13bae-114">デバイスコア</span><span class="sxs-lookup"><span data-stu-id="13bae-114">deviceScore</span></span> |   <span data-ttu-id="13bae-115">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="13bae-115">Double</span></span>  | <span data-ttu-id="13bae-116">指定された基準内の平均スコア。</span><span class="sxs-lookup"><span data-stu-id="13bae-116">Average score within specified basis.</span></span> |
|   <span data-ttu-id="13bae-117">datascore</span><span class="sxs-lookup"><span data-stu-id="13bae-117">dataScore</span></span>   |   <span data-ttu-id="13bae-118">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="13bae-118">Double</span></span>  | <span data-ttu-id="13bae-119">指定された基準内の平均スコア。</span><span class="sxs-lookup"><span data-stu-id="13bae-119">Average score within specified basis.</span></span> |
|   <span data-ttu-id="13bae-120">「id」</span><span class="sxs-lookup"><span data-stu-id="13bae-120">identityScore</span></span>   |   <span data-ttu-id="13bae-121">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="13bae-121">Double</span></span>  | <span data-ttu-id="13bae-122">指定された基準内の平均スコア。</span><span class="sxs-lookup"><span data-stu-id="13bae-122">Average score within specified basis.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="13bae-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="13bae-123">JSON representation</span></span>

<span data-ttu-id="13bae-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="13bae-124">The following is a JSON representation of the resource.</span></span>

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
