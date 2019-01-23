---
title: ratingFranceMoviesType 列挙型
description: 映画がフランスでのラベルの評価
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3b1948b2eca2075925ba2597dfda6c5e52b7817c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408153"
---
# <a name="ratingfrancemoviestype-enum-type"></a><span data-ttu-id="ab30b-103">ratingFranceMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="ab30b-103">ratingFranceMoviesType enum type</span></span>

> <span data-ttu-id="ab30b-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ab30b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ab30b-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab30b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab30b-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ab30b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab30b-107">映画がフランスでのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="ab30b-107">Movies rating labels in France</span></span>

## <a name="members"></a><span data-ttu-id="ab30b-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ab30b-108">Members</span></span>
|<span data-ttu-id="ab30b-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="ab30b-109">Member</span></span>|<span data-ttu-id="ab30b-110">値</span><span class="sxs-lookup"><span data-stu-id="ab30b-110">Value</span></span>|<span data-ttu-id="ab30b-111">説明</span><span class="sxs-lookup"><span data-stu-id="ab30b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab30b-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="ab30b-112">allAllowed</span></span>|<span data-ttu-id="ab30b-113">0</span><span class="sxs-lookup"><span data-stu-id="ab30b-113">0</span></span>|<span data-ttu-id="ab30b-114">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="ab30b-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="ab30b-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="ab30b-115">allBlocked</span></span>|<span data-ttu-id="ab30b-116">1</span><span class="sxs-lookup"><span data-stu-id="ab30b-116">1</span></span>|<span data-ttu-id="ab30b-117">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="ab30b-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="ab30b-118">agesAbove10</span><span class="sxs-lookup"><span data-stu-id="ab30b-118">agesAbove10</span></span>|<span data-ttu-id="ab30b-119">2</span><span class="sxs-lookup"><span data-stu-id="ab30b-119">2</span></span>|<span data-ttu-id="ab30b-120">10 の分類には、10 未満の未成年にフィルムのスクリーニングが禁止されています。</span><span class="sxs-lookup"><span data-stu-id="ab30b-120">The 10 classification prohibits the screening of the film to minors under 10</span></span>|
|<span data-ttu-id="ab30b-121">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="ab30b-121">agesAbove12</span></span>|<span data-ttu-id="ab30b-122">3</span><span class="sxs-lookup"><span data-stu-id="ab30b-122">3</span></span>|<span data-ttu-id="ab30b-123">12 の分類には、未成年で 12 のフィルムのスクリーニングが禁止されています。</span><span class="sxs-lookup"><span data-stu-id="ab30b-123">The 12 classification prohibits the screening of the film to minors under 12</span></span>|
|<span data-ttu-id="ab30b-124">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="ab30b-124">agesAbove16</span></span>|<span data-ttu-id="ab30b-125">4</span><span class="sxs-lookup"><span data-stu-id="ab30b-125">4</span></span>|<span data-ttu-id="ab30b-126">16 の分類には、未成年の 16 のフィルムのスクリーニングが禁止されています。</span><span class="sxs-lookup"><span data-stu-id="ab30b-126">The 16 classification prohibits the screening of the film to minors under 16</span></span>|
|<span data-ttu-id="ab30b-127">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="ab30b-127">agesAbove18</span></span>|<span data-ttu-id="ab30b-128">5</span><span class="sxs-lookup"><span data-stu-id="ab30b-128">5</span></span>|<span data-ttu-id="ab30b-129">18 の分類には、18 才未満の未成年に審査が禁止されています。</span><span class="sxs-lookup"><span data-stu-id="ab30b-129">The 18 classification prohibits the screening to minors under 18</span></span>|




