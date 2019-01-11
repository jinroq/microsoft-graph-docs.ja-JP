---
title: ratingFranceMoviesType 列挙型
description: 映画がフランスでのラベルの評価
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 591d13f6f1b291334606d24c2d6b9cd5d48f2a3d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894223"
---
# <a name="ratingfrancemoviestype-enum-type"></a><span data-ttu-id="f1cb8-103">ratingFranceMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="f1cb8-103">ratingFranceMoviesType enum type</span></span>

> <span data-ttu-id="f1cb8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f1cb8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1cb8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1cb8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1cb8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f1cb8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1cb8-107">映画がフランスでのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="f1cb8-107">Movies rating labels in France</span></span>
## <a name="members"></a><span data-ttu-id="f1cb8-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f1cb8-108">Members</span></span>
|<span data-ttu-id="f1cb8-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="f1cb8-109">Member</span></span>|<span data-ttu-id="f1cb8-110">値</span><span class="sxs-lookup"><span data-stu-id="f1cb8-110">Value</span></span>|<span data-ttu-id="f1cb8-111">説明</span><span class="sxs-lookup"><span data-stu-id="f1cb8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1cb8-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="f1cb8-112">allAllowed</span></span>|<span data-ttu-id="f1cb8-113">0</span><span class="sxs-lookup"><span data-stu-id="f1cb8-113">0</span></span>|<span data-ttu-id="f1cb8-114">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="f1cb8-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="f1cb8-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="f1cb8-115">allBlocked</span></span>|<span data-ttu-id="f1cb8-116">1</span><span class="sxs-lookup"><span data-stu-id="f1cb8-116">1</span></span>|<span data-ttu-id="f1cb8-117">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="f1cb8-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="f1cb8-118">agesAbove10</span><span class="sxs-lookup"><span data-stu-id="f1cb8-118">agesAbove10</span></span>|<span data-ttu-id="f1cb8-119">2</span><span class="sxs-lookup"><span data-stu-id="f1cb8-119">2</span></span>|<span data-ttu-id="f1cb8-120">10 の分類には、10 未満の未成年にフィルムのスクリーニングが禁止されています。</span><span class="sxs-lookup"><span data-stu-id="f1cb8-120">The 10 classification prohibits the screening of the film to minors under 10</span></span>|
|<span data-ttu-id="f1cb8-121">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="f1cb8-121">agesAbove12</span></span>|<span data-ttu-id="f1cb8-122">3</span><span class="sxs-lookup"><span data-stu-id="f1cb8-122">3</span></span>|<span data-ttu-id="f1cb8-123">12 の分類には、未成年で 12 のフィルムのスクリーニングが禁止されています。</span><span class="sxs-lookup"><span data-stu-id="f1cb8-123">The 12 classification prohibits the screening of the film to minors under 12</span></span>|
|<span data-ttu-id="f1cb8-124">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="f1cb8-124">agesAbove16</span></span>|<span data-ttu-id="f1cb8-125">4</span><span class="sxs-lookup"><span data-stu-id="f1cb8-125">4</span></span>|<span data-ttu-id="f1cb8-126">16 の分類には、未成年の 16 のフィルムのスクリーニングが禁止されています。</span><span class="sxs-lookup"><span data-stu-id="f1cb8-126">The 16 classification prohibits the screening of the film to minors under 16</span></span>|
|<span data-ttu-id="f1cb8-127">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="f1cb8-127">agesAbove18</span></span>|<span data-ttu-id="f1cb8-128">5</span><span class="sxs-lookup"><span data-stu-id="f1cb8-128">5</span></span>|<span data-ttu-id="f1cb8-129">18 の分類には、18 才未満の未成年に審査が禁止されています。</span><span class="sxs-lookup"><span data-stu-id="f1cb8-129">The 18 classification prohibits the screening to minors under 18</span></span>|





