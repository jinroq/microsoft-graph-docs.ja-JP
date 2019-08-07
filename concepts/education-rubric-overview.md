---
title: 教育機関ルーブリックの概要
description: ルーブリックは、効果的で広く使用されている課題の評価方法で、Microsoft Graph の教育機関 API によってサポートされています。
author: mmast-msft
localization_priority: Priority
ms.prod: education
ms.openlocfilehash: 56b9bcdf32036361fb92fe372952c94d09d8dc57
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173084"
---
# <a name="education-rubric-overview"></a><span data-ttu-id="7af51-103">教育機関ルーブリックの概要</span><span class="sxs-lookup"><span data-stu-id="7af51-103">Education rubric overview</span></span>

<span data-ttu-id="7af51-104">ルーブリックは、効果的で広く使用されている課題の評価方法で、Microsoft Graph の教育機関 API によってサポートされています。</span><span class="sxs-lookup"><span data-stu-id="7af51-104">Rubrics are an effective and widely-used way of grading assignments, and the education API in Microsoft Graph supports them.</span></span>

<span data-ttu-id="7af51-105">評価ルーブリックは、次のような*品質*、*レベル*、*基準*のマトリックスです。</span><span class="sxs-lookup"><span data-stu-id="7af51-105">A grading rubric is a matrix of *qualities*, *levels*, and *criteria*, as follows:</span></span>

| | <span data-ttu-id="7af51-106">レベル</span><span class="sxs-lookup"><span data-stu-id="7af51-106">Level</span></span> | <span data-ttu-id="7af51-107">レベル</span><span class="sxs-lookup"><span data-stu-id="7af51-107">Level</span></span> |
|:--|:--|:--|
| <span data-ttu-id="7af51-108">品質</span><span class="sxs-lookup"><span data-stu-id="7af51-108">Quality</span></span> | <span data-ttu-id="7af51-109">基準</span><span class="sxs-lookup"><span data-stu-id="7af51-109">Criterion</span></span> | <span data-ttu-id="7af51-110">基準</span><span class="sxs-lookup"><span data-stu-id="7af51-110">Criterion</span></span> |
| <span data-ttu-id="7af51-111">品質</span><span class="sxs-lookup"><span data-stu-id="7af51-111">Quality</span></span> | <span data-ttu-id="7af51-112">基準</span><span class="sxs-lookup"><span data-stu-id="7af51-112">Criterion</span></span> | <span data-ttu-id="7af51-113">基準</span><span class="sxs-lookup"><span data-stu-id="7af51-113">Criterion</span></span> |

<span data-ttu-id="7af51-114">評価ルーブリックの例は、次のとおりです:</span><span class="sxs-lookup"><span data-stu-id="7af51-114">An example of a grading rubric might be:</span></span>

| | <span data-ttu-id="7af51-115">良い</span><span class="sxs-lookup"><span data-stu-id="7af51-115">Good</span></span> | <span data-ttu-id="7af51-116">悪い</span><span class="sxs-lookup"><span data-stu-id="7af51-116">Poor</span></span> |
|:--|:--|:--|
| <span data-ttu-id="7af51-117">主張</span><span class="sxs-lookup"><span data-stu-id="7af51-117">Argument</span></span> | <span data-ttu-id="7af51-118">エッセイの主張に、説得力があります。</span><span class="sxs-lookup"><span data-stu-id="7af51-118">The essay's argument is persuasive.</span></span> | <span data-ttu-id="7af51-119">エッセイの主張に、筋が通っていません。</span><span class="sxs-lookup"><span data-stu-id="7af51-119">The essay's argument does not make sense.</span></span> |
| <span data-ttu-id="7af51-120">スペルと文法</span><span class="sxs-lookup"><span data-stu-id="7af51-120">Definitions in the Spelling and Grammar panes</span></span> | <span data-ttu-id="7af51-121">エッセイのスペルと文法は正しく、ほとんどまたは全く誤りがありません。</span><span class="sxs-lookup"><span data-stu-id="7af51-121">The essay uses proper spelling and grammar with few or no errors.</span></span> | <span data-ttu-id="7af51-122">エッセイには、多くのスペルや文法の誤りがあります。</span><span class="sxs-lookup"><span data-stu-id="7af51-122">The essay has numerous errors in spelling and/or grammar.</span></span> |

<span data-ttu-id="7af51-123">ルーブリックを使用した評価には、ルーブリックの各*品質*に対して 1 つの*レベル*を選択する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7af51-123">Grading using a rubric involves selecting one *level* for each *quality* in the rubric.</span></span>

<span data-ttu-id="7af51-124">ルーブリックには、各レベルに関連付けられたポイントと、各品質に関連付けられた重みが*あります*。</span><span class="sxs-lookup"><span data-stu-id="7af51-124">A rubric *may* have points associated with each level, and a weight associated with each quality.</span></span>  <span data-ttu-id="7af51-125">存在する場合、重みは最大で 100 になります。</span><span class="sxs-lookup"><span data-stu-id="7af51-125">If present, weights must add up to 100.</span></span>

| | <span data-ttu-id="7af51-126">良い (2 ポイント)</span><span class="sxs-lookup"><span data-stu-id="7af51-126">Good (2 points)</span></span> | <span data-ttu-id="7af51-127">悪い (1 ポイント)</span><span class="sxs-lookup"><span data-stu-id="7af51-127">Poor (1 point)</span></span> |
|:--|:--|:--|
| <span data-ttu-id="7af51-128">主張 (重み 50)</span><span class="sxs-lookup"><span data-stu-id="7af51-128">Argument (weight 50)</span></span> | <span data-ttu-id="7af51-129">エッセイの主張に、説得力があります。</span><span class="sxs-lookup"><span data-stu-id="7af51-129">The essay's argument is persuasive.</span></span> | <span data-ttu-id="7af51-130">エッセイの主張に、筋が通っていません。</span><span class="sxs-lookup"><span data-stu-id="7af51-130">The essay's argument does not make sense.</span></span> |
| <span data-ttu-id="7af51-131">スペルと文法 (重み 50)</span><span class="sxs-lookup"><span data-stu-id="7af51-131">Spelling and Grammar (weight 50)</span></span> | <span data-ttu-id="7af51-132">エッセイのスペルと文法は正しく、ほとんどまたは全く誤りがありません。</span><span class="sxs-lookup"><span data-stu-id="7af51-132">The essay uses proper spelling and grammar with few or no errors.</span></span> | <span data-ttu-id="7af51-133">エッセイには、多くのスペルや文法の誤りがあります。</span><span class="sxs-lookup"><span data-stu-id="7af51-133">The essay has numerous errors in spelling and/or grammar.</span></span> |

## <a name="api-reference"></a><span data-ttu-id="7af51-134">API リファレンス</span><span class="sxs-lookup"><span data-stu-id="7af51-134">API reference</span></span>

<span data-ttu-id="7af51-135">ルーブリックの使用を開始するには、[Microsoft Graph ベータ版の educationRubric リソースおよび関連メソッド](/graph/api/resources/educationrubric?view=graph-rest-beta)から始めます。</span><span class="sxs-lookup"><span data-stu-id="7af51-135">To begin using rubrics, start with the [educationRubric resource in Microsoft Graph beta](/graph/api/resources/educationrubric?view=graph-rest-beta) and associated methods.</span></span>





 

