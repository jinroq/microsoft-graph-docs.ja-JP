---
title: ratingFranceTelevisionType 列挙型
description: フランスのテレビのコンテンツの規制ラベル
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 45e55109a9f749c869ede07132be5b9264f890a9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403652"
---
# <a name="ratingfrancetelevisiontype-enum-type"></a><span data-ttu-id="5c2ba-103">ratingFranceTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="5c2ba-103">ratingFranceTelevisionType enum type</span></span>

> <span data-ttu-id="5c2ba-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5c2ba-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5c2ba-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c2ba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5c2ba-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5c2ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c2ba-107">フランスのテレビのコンテンツの規制ラベル</span><span class="sxs-lookup"><span data-stu-id="5c2ba-107">TV content rating labels in France</span></span>

## <a name="members"></a><span data-ttu-id="5c2ba-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="5c2ba-108">Members</span></span>
|<span data-ttu-id="5c2ba-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="5c2ba-109">Member</span></span>|<span data-ttu-id="5c2ba-110">値</span><span class="sxs-lookup"><span data-stu-id="5c2ba-110">Value</span></span>|<span data-ttu-id="5c2ba-111">説明</span><span class="sxs-lookup"><span data-stu-id="5c2ba-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c2ba-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="5c2ba-112">allAllowed</span></span>|<span data-ttu-id="5c2ba-113">0</span><span class="sxs-lookup"><span data-stu-id="5c2ba-113">0</span></span>|<span data-ttu-id="5c2ba-114">既定値、すべてのテレビ番組コンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="5c2ba-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="5c2ba-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="5c2ba-115">allBlocked</span></span>|<span data-ttu-id="5c2ba-116">1</span><span class="sxs-lookup"><span data-stu-id="5c2ba-116">1</span></span>|<span data-ttu-id="5c2ba-117">任意のテレビ番組コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="5c2ba-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="5c2ba-118">agesAbove10</span><span class="sxs-lookup"><span data-stu-id="5c2ba-118">agesAbove10</span></span>|<span data-ttu-id="5c2ba-119">2</span><span class="sxs-lookup"><span data-stu-id="5c2ba-119">2</span></span>|<span data-ttu-id="5c2ba-120">-10 クラス分けは 10 未満の子供にはお勧めできません。</span><span class="sxs-lookup"><span data-stu-id="5c2ba-120">The -10 classification is not recommended for children under 10</span></span>|
|<span data-ttu-id="5c2ba-121">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="5c2ba-121">agesAbove12</span></span>|<span data-ttu-id="5c2ba-122">3</span><span class="sxs-lookup"><span data-stu-id="5c2ba-122">3</span></span>|<span data-ttu-id="5c2ba-123">-12 分類が 12 未満の子供にお勧めできません。</span><span class="sxs-lookup"><span data-stu-id="5c2ba-123">The -12 classification is not recommended for children under 12</span></span>|
|<span data-ttu-id="5c2ba-124">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="5c2ba-124">agesAbove16</span></span>|<span data-ttu-id="5c2ba-125">4</span><span class="sxs-lookup"><span data-stu-id="5c2ba-125">4</span></span>|<span data-ttu-id="5c2ba-126">-16 のクラス分けは 16 の子にはお勧めできません。</span><span class="sxs-lookup"><span data-stu-id="5c2ba-126">The -16 classification is not recommended for children under 16</span></span>|
|<span data-ttu-id="5c2ba-127">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="5c2ba-127">agesAbove18</span></span>|<span data-ttu-id="5c2ba-128">5</span><span class="sxs-lookup"><span data-stu-id="5c2ba-128">5</span></span>|<span data-ttu-id="5c2ba-129">-18 の分類は 18 才未満の方のためお勧めできません。</span><span class="sxs-lookup"><span data-stu-id="5c2ba-129">The -18 classification is not recommended for persons under 18</span></span>|




