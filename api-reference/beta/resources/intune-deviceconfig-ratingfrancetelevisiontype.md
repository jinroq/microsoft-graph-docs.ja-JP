---
title: ratingFranceTelevisionType 列挙型
description: フランスのテレビのコンテンツの規制ラベル
author: tfitzmac
ms.openlocfilehash: f202b2e942e36e7c13052643a31ee0a984723f5d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312216"
---
# <a name="ratingfrancetelevisiontype-enum-type"></a><span data-ttu-id="e20d2-103">ratingFranceTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="e20d2-103">ratingFranceTelevisionType enum type</span></span>

> <span data-ttu-id="e20d2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e20d2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e20d2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e20d2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e20d2-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e20d2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e20d2-107">フランスのテレビのコンテンツの規制ラベル</span><span class="sxs-lookup"><span data-stu-id="e20d2-107">TV content rating labels in France</span></span>
## <a name="members"></a><span data-ttu-id="e20d2-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e20d2-108">Members</span></span>
|<span data-ttu-id="e20d2-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="e20d2-109">Member</span></span>|<span data-ttu-id="e20d2-110">値</span><span class="sxs-lookup"><span data-stu-id="e20d2-110">Value</span></span>|<span data-ttu-id="e20d2-111">説明</span><span class="sxs-lookup"><span data-stu-id="e20d2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e20d2-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="e20d2-112">allAllowed</span></span>|<span data-ttu-id="e20d2-113">0</span><span class="sxs-lookup"><span data-stu-id="e20d2-113">0</span></span>|<span data-ttu-id="e20d2-114">既定値、すべてのテレビ番組コンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="e20d2-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="e20d2-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="e20d2-115">allBlocked</span></span>|<span data-ttu-id="e20d2-116">1</span><span class="sxs-lookup"><span data-stu-id="e20d2-116">1</span></span>|<span data-ttu-id="e20d2-117">任意のテレビ番組コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="e20d2-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="e20d2-118">agesAbove10</span><span class="sxs-lookup"><span data-stu-id="e20d2-118">agesAbove10</span></span>|<span data-ttu-id="e20d2-119">2</span><span class="sxs-lookup"><span data-stu-id="e20d2-119">2</span></span>|<span data-ttu-id="e20d2-120">-10 クラス分けは 10 未満の子供にはお勧めできません。</span><span class="sxs-lookup"><span data-stu-id="e20d2-120">The -10 classification is not recommended for children under 10</span></span>|
|<span data-ttu-id="e20d2-121">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="e20d2-121">agesAbove12</span></span>|<span data-ttu-id="e20d2-122">3</span><span class="sxs-lookup"><span data-stu-id="e20d2-122">3</span></span>|<span data-ttu-id="e20d2-123">-12 分類が 12 未満の子供にお勧めできません。</span><span class="sxs-lookup"><span data-stu-id="e20d2-123">The -12 classification is not recommended for children under 12</span></span>|
|<span data-ttu-id="e20d2-124">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="e20d2-124">agesAbove16</span></span>|<span data-ttu-id="e20d2-125">4</span><span class="sxs-lookup"><span data-stu-id="e20d2-125">4</span></span>|<span data-ttu-id="e20d2-126">-16 のクラス分けは 16 の子にはお勧めできません。</span><span class="sxs-lookup"><span data-stu-id="e20d2-126">The -16 classification is not recommended for children under 16</span></span>|
|<span data-ttu-id="e20d2-127">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="e20d2-127">agesAbove18</span></span>|<span data-ttu-id="e20d2-128">5</span><span class="sxs-lookup"><span data-stu-id="e20d2-128">5</span></span>|<span data-ttu-id="e20d2-129">-18 の分類は 18 才未満の方のためお勧めできません。</span><span class="sxs-lookup"><span data-stu-id="e20d2-129">The -18 classification is not recommended for persons under 18</span></span>|




