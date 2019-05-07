---
title: averageComparativeScore リソースの種類
description: 異なる範囲に基づいてさまざまなスコアが含まれています。
localization_priority: Normal
author: preetikr
ms.openlocfilehash: 59faa1c3dcf3f7f2b70807a74878dab796ae4d54
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629328"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="87637-103">averageComparativeScore リソースの種類</span><span class="sxs-lookup"><span data-stu-id="87637-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="87637-104">さまざまな範囲に基づいてさまざまなスコアが格納されています (たとえば、業種別の平均、企業座席の平均サイズなど)。また、コントロールカテゴリ (Id、データ、デバイス、アプリ、インフラストラクチャ) に基づいています。</span><span class="sxs-lookup"><span data-stu-id="87637-104">Contains various different scores based on different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

## <a name="properties"></a><span data-ttu-id="87637-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="87637-105">Properties</span></span>

|<span data-ttu-id="87637-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="87637-106">Property</span></span> |<span data-ttu-id="87637-107">型</span><span class="sxs-lookup"><span data-stu-id="87637-107">Type</span></span> |<span data-ttu-id="87637-108">説明</span><span class="sxs-lookup"><span data-stu-id="87637-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="87637-109">だけ</span><span class="sxs-lookup"><span data-stu-id="87637-109">basis</span></span>|<span data-ttu-id="87637-110">String</span><span class="sxs-lookup"><span data-stu-id="87637-110">String</span></span>|<span data-ttu-id="87637-111">範囲の種類。</span><span class="sxs-lookup"><span data-stu-id="87637-111">Scope type.</span></span> <span data-ttu-id="87637-112">使用可能な値: `AllTenants`、`TotalSeats`、`IndustryTypes`。</span><span class="sxs-lookup"><span data-stu-id="87637-112">The possible values are: `AllTenants`, `TotalSeats`, `IndustryTypes`.</span></span>|
|<span data-ttu-id="87637-113">averageScore</span><span class="sxs-lookup"><span data-stu-id="87637-113">averageScore</span></span>|<span data-ttu-id="87637-114">2 行分</span><span class="sxs-lookup"><span data-stu-id="87637-114">Double</span></span>|<span data-ttu-id="87637-115">指定された基準内の平均スコア。</span><span class="sxs-lookup"><span data-stu-id="87637-115">Average score within specified basis.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="87637-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="87637-116">JSON representation</span></span>

<span data-ttu-id="87637-117">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="87637-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.averageComparativeScore"
}-->

```json
{
  "basis": "String",
  "averageScore": "Double"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "averageComparativeScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
