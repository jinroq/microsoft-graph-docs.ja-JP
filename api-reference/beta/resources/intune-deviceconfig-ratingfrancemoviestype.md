---
title: ratingFranceMoviesType 列挙型
description: 映画がフランスでのラベルの評価
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3b9220b5c4ba406aadda930eb355f3d472929a03
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957775"
---
# <a name="ratingfrancemoviestype-enum-type"></a><span data-ttu-id="7eda8-103">ratingFranceMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="7eda8-103">ratingFranceMoviesType enum type</span></span>

> <span data-ttu-id="7eda8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7eda8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7eda8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7eda8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7eda8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7eda8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7eda8-107">映画がフランスでのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="7eda8-107">Movies rating labels in France</span></span>
## <a name="members"></a><span data-ttu-id="7eda8-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="7eda8-108">Members</span></span>
|<span data-ttu-id="7eda8-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="7eda8-109">Member</span></span>|<span data-ttu-id="7eda8-110">値</span><span class="sxs-lookup"><span data-stu-id="7eda8-110">Value</span></span>|<span data-ttu-id="7eda8-111">説明</span><span class="sxs-lookup"><span data-stu-id="7eda8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7eda8-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="7eda8-112">allAllowed</span></span>|<span data-ttu-id="7eda8-113">0</span><span class="sxs-lookup"><span data-stu-id="7eda8-113">0</span></span>|<span data-ttu-id="7eda8-114">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="7eda8-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="7eda8-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="7eda8-115">allBlocked</span></span>|<span data-ttu-id="7eda8-116">1</span><span class="sxs-lookup"><span data-stu-id="7eda8-116">1</span></span>|<span data-ttu-id="7eda8-117">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="7eda8-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="7eda8-118">agesAbove10</span><span class="sxs-lookup"><span data-stu-id="7eda8-118">agesAbove10</span></span>|<span data-ttu-id="7eda8-119">2</span><span class="sxs-lookup"><span data-stu-id="7eda8-119">2</span></span>|<span data-ttu-id="7eda8-120">10 の分類には、10 未満の未成年にフィルムのスクリーニングが禁止されています。</span><span class="sxs-lookup"><span data-stu-id="7eda8-120">The 10 classification prohibits the screening of the film to minors under 10</span></span>|
|<span data-ttu-id="7eda8-121">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="7eda8-121">agesAbove12</span></span>|<span data-ttu-id="7eda8-122">3</span><span class="sxs-lookup"><span data-stu-id="7eda8-122">3</span></span>|<span data-ttu-id="7eda8-123">12 の分類には、未成年で 12 のフィルムのスクリーニングが禁止されています。</span><span class="sxs-lookup"><span data-stu-id="7eda8-123">The 12 classification prohibits the screening of the film to minors under 12</span></span>|
|<span data-ttu-id="7eda8-124">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="7eda8-124">agesAbove16</span></span>|<span data-ttu-id="7eda8-125">4</span><span class="sxs-lookup"><span data-stu-id="7eda8-125">4</span></span>|<span data-ttu-id="7eda8-126">16 の分類には、未成年の 16 のフィルムのスクリーニングが禁止されています。</span><span class="sxs-lookup"><span data-stu-id="7eda8-126">The 16 classification prohibits the screening of the film to minors under 16</span></span>|
|<span data-ttu-id="7eda8-127">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="7eda8-127">agesAbove18</span></span>|<span data-ttu-id="7eda8-128">5</span><span class="sxs-lookup"><span data-stu-id="7eda8-128">5</span></span>|<span data-ttu-id="7eda8-129">18 の分類には、18 才未満の未成年に審査が禁止されています。</span><span class="sxs-lookup"><span data-stu-id="7eda8-129">The 18 classification prohibits the screening to minors under 18</span></span>|





